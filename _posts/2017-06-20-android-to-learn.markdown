---
layout: post
title:  "Android 常用方法总结!"
date:   2017-06-20 19:11:03 +0800
categories: jekyll update
---

字符串链接：支持SpannableString
public static CharSequence concat(CharSequence... text)
使用：TextUtils.concat("Hello"," ","World!").toString(); -----> Hello World!

判断字符串中是否是纯数字：
public static boolean concat(CharSequence str);

android.webkit.URLUtil

android.text.format.DateUtils
格式化日期格式：

public static String formatDateTime(Context context,long millis,int flags);
使用：formatDateTime（context，millis，DateUtils.FORMAT_SHOW_YEAR|
DateUtils.FORMAT_SHOW_DATE|
DateUtils.FORMAT_SHOW_WEEKDAY|
DateUtils.FORMAT_SHOW_TIME|）
输出：2016年1月16日星期五 12:40

判断日期是否是今天：
public static boolean isToday（long when）；

返回今天，昨天，日期
public static CharSequence getRelativeTimeSpanString（long startTime）；

