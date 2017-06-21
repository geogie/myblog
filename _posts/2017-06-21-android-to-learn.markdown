---
layout: post
title:  "Android throw Exception"
date:   2017-06-16 19:11:03 +0800
categories: android
---
{% highlight bash lineno %}
throw new IllegalStateException("Content View height is too small");//下面不会执行了，并且直接crash闪退
{% endhighlight %}
{% highlight ruby %}
场景：
Stack<Activity> activityStack;
activityStack.lastElement()；／／出现闪退
解决：
try {
    activity = activityStack.lastElement();
} catch (NoSuchElementException e) {
    e.printStackTrace();
}
{% endhighlight %}
