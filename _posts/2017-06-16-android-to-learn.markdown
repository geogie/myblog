---
layout: post
title:  "Android 适配"
date:   2017-06-16 19:11:03 +0800
categories: android
---
{% highlight bash lineno %}
遇到代码中设置action bar 的crash问题
{% endhighlight %}
{% highlight ruby %}
highlight 对于api<=19的手机
方案1：
if (Build.VERSION.SDK_INT > Build.VERSION_CODES.KITKAT) {
    getWindow().requestFeature(Window.FEATURE_ACTION_BAR);
}
方案2：
requestWindowFeature(Window.FEATURE_NO_TITLE);
{% endhighlight %}
