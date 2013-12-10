---
layout: post
title: "ApplicationXtender Foreign File Name Extraction"
description: "Get the original file name of the foreign file from the .bin stored in AX."
category: "ApplicationXtender"
tags: [ApplicationXtender]
comments: true
---
{% include JB/setup %}
Several projects have come across our desk where the customer needed to know the original file name of a document stored in AX. The AX database does not store the mime type of documents, so when you have a foreign file stored in AX, there is no way outside of the viewer to know what it is. When you have integrated other applications with AX, this poses a problem. Your client app may not be able to use the AX file viewer OCX; a web application is such a scenario. If you have access to the path to the bin file, you can use this handy function to return the original name of the AX foreign file.

<script src="https://gist.github.com/sykaufax/7897493.js"></script>


