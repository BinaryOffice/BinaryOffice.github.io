---
layout: post
title: "Improving Recognition in TeleForm"
author: "Sy Kaufax"
description: "Overcoming limitations in field validation in TeleForm."
category: "TeleForm"
tags: ["TeleForm", "Form Processing", "Scripting"]
comments: false
---
{% include JB/setup %}
Building on the concept outlined in the [last post](/teleform/2013/11/04/improving-recognition-in-teleform/), we offer another tip to improve field validation: regular expressions. Most people who have dabbled with scripting should have heard of regular expressions, if not, here is a brief summary:
> In computing, a regular expression (abbreviated regex or regexp) is a sequence of characters that forms a search pattern, mainly for use in pattern matching with strings, or string matching, i.e. "find and replace"-like operations. - [Wikipedia](http://en.wikipedia.org/wiki/Regular_expression)


While it is true that TeleForm has no "built-in" support for regular expressions, a few lines of script can remedy this shortcoming. Every windows computer should have Microsoft's VBScript [RegEx object](http://msdn.microsoft.com/en-us/library/ms974570.aspx), so it is simple to call from VBA. There are many online regex validator/testers on the web, but for this example we will use [regexpal]([http://regexpal.com/](http://regexpal.com/)).

Let's say that we have a field whose valid value is AX1234B or XBP1234. The regular expression would be: (^AX1234B$)|(^XBP1234$). Add the following code to your form script, changing "My_Field_Name" with the name of the field you're interested in.

<script src="https://gist.github.com/sykaufax/7314115.js">
</script>



