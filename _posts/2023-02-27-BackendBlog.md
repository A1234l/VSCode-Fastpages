---
layout: post
title: Backend CRUD Blog Achievements
description: This is the backend achievements blog, showing evidence of working Create, Read, Update, and Delete.
toc: true
permalink: /BE
categories: [markdown, Week 24]
---

## Code from the Backend

#### Create:
![]({{site.baseurl}}/images/POST3.png)
Creating a user profile uses the POST method. There are multiple error conditions handled in the code. If the username inputted does not have 3 characters, an error message is displayed. If the score has no digits, an error message is displayed. Finally, if there is a format error for the date, then an error message is again displayed.

#### Read:
![]({{site.baseurl}}/images/GET.png)
The person is able to read the data from the API using the GET method. This code helps display all the data from the API.

#### Update:
![]({{site.baseurl}}/images/PUT.png)
Updating a profile uses the PUT method. The username to be updated is inputted, and the score is updated to the newly inputted score.

#### Delete:
![]({{site.baseurl}}/images/DELETE.png)
Deleting a profile uses the DELETE method. An ID number is inputted, and the profile with the corresponding ID number is deleted.

# Demonstration of working CRUD using postman:
https://youtu.be/NO75rgn60ZQ
