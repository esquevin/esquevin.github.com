---
layout: post
title: "input range sucks, and how to improve them"
description: ""
category: 
tags: [angular]
head: |
    <link rel="stylesheet" href="/css/master.css" type="text/css" media="screen" title="no title" charset="utf-8">
    <script src="//cdnjs.cloudflare.com/ajax/libs/angular.js/1.2.20/angular.js" type="text/javascript" charset="utf-8"></script>
---
{% include JB/setup %}


Here is an input range :
<form>
    <input type="range" name="bla" min="0" max="100" step="10"/>
</form>

It gives you very little feedback, and doesn't allow you to know which value you picked, what the boundaries are or anything.

We can improve them by implementing custom behavior & style.


