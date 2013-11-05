---
layout: post
title: "Improving Recognition in TeleForm"
author: "Sy Kaufax"
description: "Overcoming limitations in constrained print and comb fields."
category: "TeleForm"
tags: [TeleForm, Form Processing, Scripting]
---
{% include JB/setup %}

Have you ever found yourself wishing that TeleForm had more flexibility in its format options? The standard options for alphanumeric templates do not allow you to <em>"fine tune"</em> when there is more than one valid format. For example: a valid PO number can start with an alpha followed by a number or another alpha. Using the standard format, you would set the template value to "AXNNNN". While this works, recognition will not be as good as it could be.

####Consider stacking fields
To narrow down the possible formats you can create two fields and stack one on top of the other. Finally, add a field on top of those two without any format. Set field 1 to template "AANNNN" and field 2 "ANNNNN". From there, write a simple script that executes in form_evalute.

<script src="https://gist.github.com/sykaufax/7313211.js"></script>

