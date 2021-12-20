---
layout: post
title:  "Object initializer spaces"
date:   2021-12-20 12:31:00 +0000
categories: csharp resharper
---

If you're using ReSharper and StyleCop in your solution you may have come across the issue that ReSharper removes spaces between the braces in the object initializer syntax. This causes the compiler to emit warnings SA1012 and SA1013. To change this behaviour you need only change a setting in the ReSharper control panel. Which I will describe below:

## How to
1. Go to Extensions -> ReSharper -> Options -> Code Editing -> C# -> Spaces
2. Check 'Within single-line-expression braces' under the 'Around braces' dropdown menu
3. Save

### Before

{% highlight csharp %}
var obj = new MyClass {MyProperty = "Hello, World!"};
{% endhighlight %}

### After

{% highlight csharp %}
var obj = new MyClass { MyProperty = "Hello, World!" };
{% endhighlight %}