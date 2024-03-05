# PixieBrixForQuizzyNews
Documentation of my PixieBrix project on behalf of Quizzy.News

**Goal**: Create a user-friendly frontend/GUI for daily news quiz generation and editing so that we can pass the content into our Quizzy.News news game app

**Tools**: 
+ PixieBrix, a “human-in-the-loop” automation tool that lives in Chrome extensions and can generate a user-initiated flow of actions ranging from http and ChatGPT requests to interactions with third-party software; automation flows are referred to as “mods”
+ NewsAPI, a source for news headlines
+ Firebase, our storage system for generated quiz content

**Steps**:
+ Request news articles from NewsAPI using sources from the political center, as ranked by AllSides.com (I chose Newsweek)
+ Use ChatGPT to generate a quiz from those articles
  + The quiz has five multiple-choice questions
  + There are three choices per question
  + Choices are 5 words or less so they look nice on the quiz frontend
+ The data includes a source object with news source, title, and url for later use
+ Create the frontend to display/edit/approve the ChatGPT response
+ Submit final quiz to Firebase (with an approved:true property)

+ ## See the PDF in the repo for screenshots of the mod itself!##
