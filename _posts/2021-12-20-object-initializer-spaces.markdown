---
layout: post
title:  "Object initializer spaces"
date:   2021-12-20 12:31:00 +0000
categories: csharp
---

## Before

{% highlight csharp %}
var obj = new MyClass {MyProperty="Hello, World!"};
{% endhighlight %}

## After

{% highlight csharp %}
var obj = new MyClass { MyProperty="Hello, World!" };
{% endhighlight %}

## How to
1. Go to Extensions -> ReSharper -> Options -> Code Editing -> C# -> Spaces
2. Check 'Within single-line-expression braces' under the 'Around braces' dropdown menu
3. Save