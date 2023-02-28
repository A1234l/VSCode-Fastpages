---
layout: post
title: CPT Written Response Draft
description: This is the written response for the CPT project. This is just a draft.
toc: true
permalink: /CPTBlogProjectSubmission
categories: [markdown, CPT, Week 24]
---

## Video
Video is found here: [Video](https://youtu.be/NtKtnrTTgis)

# Written Response

## 3a.
### 3.a.i.
The purpose of the program is to provide a competitive gaming environment for all users.

### 3.a.ii.
After finishing the snake game by hitting the wall or the snake itself, a form is displayed to allow the user to input their username. After the form is complete, the data is added into the database and is displayed on the leaderboard.

### 3.a.iii.
After the snake game is over, the user inputs a three-letter username. The score is automatically inputted for the user. The outcome of the program is a table of the five top scorers, displaying the username, score, and date of the game.

### 3.b.i.
![]({{site.baseurl}}/images/CreateFrontend.png)

### 3.b.ii.
![]({{site.baseurl}}/images/POST3.png)

### 3.b.iii.
The variable, or constant is body is the name of the dictionary.

### 3.b.iv.
The variable body obtains the data values from the username input and the score, representing the details of the user's profile. 

### 3.b.v.
The dictionary in the variable body helps to create separate, distinct packets of information specifically for one user. Without the use of this dictionary, the database would not be able to distinguish which score corresponds to which username. This can make the program code harder to create as there would have to be a separate, more complex algorithm which manually sorts the data already present in the database.

### 3.c.i.
![]({{site.baseurl}}/images/addrowfunction.png)

### 3.c.ii.
![]({{site.baseurl}}/images/CPTNew.png)

### 3.c.iii.
The procedure add_row() adds a row on the table of the leaderboard, and displays the username, score, and date based on the user's inputs and the data from the API. This helps to display the data from user inputs onto the leaderboard so that other users are able to see the top scorers of the game.

### 3.c.iv.
The algorithm fetches the API using its URL to execute the GET method. It then checks that a successful fetch will be guaranteed, and if it is, then a response is carried out. An if statement is used to check if the response has an error with reading the database. If there is an error, an error message is displayed on the table of the leaderboard, and the entire function fetching the API is stopped. However, if there is no error, the algorithm proceeds to check that the response contains JSON data. If it does contain JSON data, the algorithm proceeds to sort the users, where the highest scoring user is displayed first and the lowest scoring user is displayed last. Next, a for loop is used so that only the top 5 scoring users are displayed onto the leaderboard, and their profiles are displayed by calling the add_row() function. Finally, the algorithm checks for any fetch errors, and if there is a fetch error, an error message is displayed onto the table of the leaderboard.

### 3.d.i.
**First Call:**
The first call is when the user clicks on the leaderboard website, which calls the function that fetches the API with a functional URL.

**Second Call:**
The second call is when the user clicks on the leaderboard website, which calls the function that fetches the API while the URL is down.'

**Condition(s) tested by first call:**
The first call checks the errors and successfully determines that there are no errors with fetching the data. As a result, the data from the user input is sorted based on the user's score using the response.json().then() command.

**Condition(s) tested by second call:**
The second call checks fetch errors using the .catch() command. Since the URL to the API is down, a fetch error will prompt the .catch() command to function.

**Results of first call:**
The first call displays the user onto the leaderboard given that it is a top five scorer.

**Results of the second call:**
An error message is displayed on the leaderboard and no user data is displayed.