---
layout: page
title: Project Plan for CPT
description: CPT Planning for project.
toc: true
permalink: /CPTProjectPlan
categories: [markdown, Week 20]
---

# Outline write up for Collegeboard
> I will be using the API database and frontend table for the write up. The API database involves a game history.

## Row 1: Purpose and function
Purpose: To provide a user-friendly interaction through competition.

### Video Plan:
I first finish playing a quick round of snake, input into the table, and then go to the page with the leaderboard. The input will be the table, the output will be the leaderboard. The program functionalty could be on postman? I'm not extremely sure about how to show the functionality. So video is still under development.

## Row 2: Data Abstraction
- First code segment will show the list json_ready in the class ScoreListAPI in score.py in api folder.
- The second code segment will be right below the list and will show all code below where it says `return jsonify(json_ready)`.
- The data in this list contains all the data for the scores and profile entered.

## Row 3: Managing Complexity
- Manages complexity by auto-generating all of the data into one single list
- If this list didn't exist, then all of the data entered would have to be processed individually which requires an huge amount of unnecessary code

## Row 4: Procedural Abstraction
- All the procedures(functions) lack a proper parameter. However, I would choose the create(self) function in model folder in scores.py as the first code segment.
- I will also show it being called in api folder in score.py in line 37 and in the if user: statement.
- Contributes to overall functionality because it helps create the data entered in the table in a json format.

## Row 5: Algorithm Implementation
- I would add the def initScores() code segment in model folder in scores.py
- Function creates test database and tables, users are inputted with the parameters, and put into a list. For loop is used to add the data to the table. Try and except statements are also used.

## Row 6: Testing
- Calls: One is to input the data in the table, the other is to delete one row of data
- Conditions: create() function used for creating new data, delete() function to delete the existing data.
- Result: Describe changes to the table.

**Note: Our project lacks enough things for at least four different CPT projects. There are ideas to create more games that are underway, but have not been fully implemented yet.**