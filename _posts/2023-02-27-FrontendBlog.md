---
layout: post
title: Frontend Code
description: This is the frontend blog, showing the code for the program functionality.
toc: true
permalink: /FE
categories: [markdown, Week 24]
---

# Frontend Features

## Garbage Data:
![]({{site.baseurl}}/images/UpdatedForm.png)

This is the code for the form where a person inputs their username after a snake game is over. The UI helps solve garbage inputs by automatically inputting the user's score. This helps to prevent cheating or inputting letters(which isn't a score).

## Create:
![]({{site.baseurl}}/images/CreateFrontend.png)

This code helps fetch the API from the deployed flask server and creates the user after inputting information into the form.

## Read:
![]({{site.baseurl}}/images/ReadFrontend1.png)
![]({{site.baseurl}}/images/ReadFrontend2.png)
![]({{site.baseurl}}/images/ReadFrontend3.png)

This code fetches the API from the deployed server and displays the data in a table. The data displayed is sorted from the highest scorer to the lowest scorer, and only the top 5 scorers are displayed.