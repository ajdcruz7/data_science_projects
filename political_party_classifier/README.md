# Political Party Classifier

Using NLP to predict the political party of a politician. 

## Abstract

This 5 week Capstone project was the final project delivered for my General Assembly Data Science Immersive programme. The project involved scraping transcripts of parliamentary debates then using NLP techniques such as Count Vectorization and term frequency-inverse document frequency (TF-IDF), along with a myriad of classification models to predict the political party of a politician in the House of Commons. Once I had addressed the large class imbalance I achieved my best scores using a Logistic Regression model. 

My class split was 65/28/7, and I achieved an accuracy score of 79%, an improvement of 14% on baseline, and AUPRC of 0.942, 0.748 and 0.557 respectively for each of the classes, which is a better measure of success for my model due to the class imbalance.


## Overview

This project was undertaken as part of my study for the 12 week General Assembly Data Science Immersive. The aim for the project was two-fold. First, to gain experience following a typical data science workflow. Second, to practice using various tools and techniques learnt on the course to tackle a problem with real world application. 

### The problem 

The British political landscape is complex and for someone seeking to understand more about politics the barrier to entry can be unnecessarily high due to a number of factors. 

Firstly, although there is access directly to view political debates and anyone can watch sessions from the Houses of Parliament, the nature of these debates and political sessions can be off-putting and hard to understand for example the language used can be confusing. 

The next source of information would be the media. British print media have long held political allegiances and often your political opinions would dictate the paper you read, not the other way around. Now, with the prevalence of digital media and social media, the lines have become blurred. Articles, videos and headlines have the ability to influence us and without knowledge of the author’s bias, this can become dangerous. 

### The Solution

I propose that a tool could be created that would be able to provide a viewer with the political bias of a piece of media before they consume that media, thus allowing them to be more informed and less susceptible to influence. 

### This project

For this project I will be presenting a proof-of-concept by using a data obtained by scraping debates from the House of Commons, which I can easily label with the political party of each MP. 
The transcripts of each speech was vectorised using Count Vectorisation and TF-IDF, before being run through various classification models that were used to predict the party of the politician. 

### Conclusions and Limitations

The models were able to predict with a good degree of accuracy, when a speaker belonged to the Conservative party however the models were less effective at predicting other parties. 
This was due to the class imbalance in the data, which was a result of where the data was collected from and over what time period (5 years). 

Collecting data from only the last 5 years meant that the data represented a situation with only the Conservatives in power, and the results were perhaps more reflective of incumbent vs opposition than left vs right wing. 

Parliamentary language used in the debates meant that the models are less applicable to the use case in the media. 

Many of the limitations of this project can be solved by collecting data from more diverse sources. 
By collecting data from MP Twitter Accounts, Blogs, Digital Media with clear political orientation and other easily labeled data, I would be able to address the class imbalance by ensuring that I have balanced classes, I would not have the problems with parliamentary language and the models would be more fit for purpose (predicting bias in news articles). 

### Next steps

Repeat the project with more diverse data

Turn the problem into a binary classification Left/Right

Create a web based application to provide predictions for passages of text. 

