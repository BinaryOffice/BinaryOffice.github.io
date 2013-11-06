---
layout: post
title: "Advanced PageLinking in TeleForm"
description: "Additional techniques to link on multiple fields"
category: "TeleForm"
tags: [TeleForm, Scripting, Forms Processing]
comments: true
---
{% include JB/setup %}
Page linking in TeleForm is pretty straight forward when you have one field to link on. However, many form processes require more complex linking. Perhaps you want to link on three fields, or, maybe you need your link field to be in different places on each page. There is no clear way to do this within the Designer, so how can it be accomplished?
###Create a page link field with processing turned off
TeleForm will link pages based on the value in the page link field, and it does not need to be "read" from the form. By creating a page link that is decoupled from form fields, you are able to populate it with whatever values you want. In this way, you do not change the way TeleForm works, but you do add flexibility.
####Use Case
You have a two page form with an account number and filing date. You want to link page one with page two based on these fields. You also need these fields in different places on the form for design reasons.
<img alt="Form Page 1" src="../img/Page_link_form_page_1.png" height="75%"/>

If you have upgraded ApplicationXtender to 6.5 or above and found that the included export for TeleForm no longer works, fear not, we have a supported replacement. It requires that the ApplicationXtender document manager be installed on the TeleForm workstation (Reader and Designer) and uses the supported AX API. If you would like more information, please leave a comment or call us at <a href="tel:+14809706900">480-970-6900</a>, select the option for Tech Support and a TeleForm/ApplicationXtender expert will be happy to help.

![Agent screen shot](http://techblog.binaryoffice.com/img/ax_connect_agent.png)