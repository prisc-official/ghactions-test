## This is a ghactions test for my NUS project.

## About Me

I am a Corporate Banker and I haver ZERO IT/ Programming knowledge. 

## My Learning Objectives

1) To replicate an existing application code for future deployment. 
2) To make changes on the repository which will trigger a message to Telegram on committed changes.  

## Steps I've undertaken

1) Forked Professor Uli's Github repository - ghactions-test 
2) Made changes and observed that the GH Actions and workflows were updated accordingly. However, no TG message was sent. 
3) Got help from a fellow NUS classmate, who shared that I need to do a webhook. 
4) Learnt how to use webhooks/ IFTTT @ https://hevodata.com/learn/ifttt-webhook/#:~:text=Users%20can%20implement%20a%20Webhook,Webhooks%20using%20simple%20Web%20Requests
5) Created an account on IFTTT https://ifttt.com/  
- Choose a "webhook service" (IF)
- Created an Event Name - which "sendsTGmessage_onchange"
- Choose to integrate it to Telegram (THEN THAT)

6) Head to IFTT webhook page and click documentations to get a unique IFTTT Webhook URL @ https://ifttt.com/maker_webhooks
7) Updated the CURL function in the YML file with key changes made to the "event" and "unique IFTTT Webhook url link"
8) Ensure integration with Telegram is successful


## Outcome 1- The bot works!!!

## Outcome 2- The Commit Changes worked!!!

## What was difficult? 
Getting an application source code that works and being able to understand it's purpose. 


## What didn't work? 
- Uli's ghaction. 
- Pushing new commits to the repository to trigger a workflow that does something with your code and trigger a notification to Telegram. 

