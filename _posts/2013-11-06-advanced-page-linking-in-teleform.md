---
layout: post
title: "Advanced Page Linking in TeleForm"
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

<img alt="Form Page 1" src="/img/page_link_form_page_1.png" height="25%"/>
<img alt="Form Page 2" src="/img/page_link_form_page_2.png" height="25%"/>

We have added an image zone called "pl" at the bottom of the page and set recognition to "none". With a little bit of script, we have the pages linking on the fields we want.

<script src="https://gist.github.com/sykaufax/7344837.js">
</script>

[Download the tempate](https://github.com/BinaryOffice/AdvancedTeleFormPageLink/archive/master.zip)