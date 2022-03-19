## GHACTIONS TEST- My NUS Project

## About Me
<img src="https://user-images.githubusercontent.com/98994112/159111464-5ab4087a-33d6-4919-bf79-6c47fef82405.jpg" width=20% height=20%>

I am a Corporate Banker and I haver ZERO IT/ Programming knowledge. However, I'll be joining a Digibank soon, and hope to contribute and make a difference by applying my knowledge during projects participation. 
* [LinkedIn Profile] (https://www.linkedin.com/in/priscillialau/)

## My Learning Objectives from GHACTIONS TEST- Challenge what I am clueless! 

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
- Configure integration with your username, and this will connect to Telegram 

6) Connecting to Telegram Successfully
- Give permission to IFTTT bot on Telegram to connect with your account. 
- Create a New Channel on Telegram; ensure channel is selected in IFTTT and calibrate the message structure in IFTTT. Make sure IFTTT is an administrator in the channel. 
- Type: /connect_channel to IFTTT bot on Telegram 
- Confirm the channelname by typing it. 
- Obtain confirmation on successful connection! 

7) Headed to IFTT webhook page and clicked documentations to get a unique IFTTT Webhook URL @ https://ifttt.com/maker_webhooks
8) Updated the CURL function in the YML file with key changes made to the "event" and "unique IFTTT Webhook url link"
9) Tested it out by committing changes on Readme/ YML/ add a new file, etc. Workflow was successfully fired and a message was triggered on Telegram!

![image](https://user-images.githubusercontent.com/98994112/159111322-f83109d2-95bb-4cba-bb4d-89084b441390.png)


## What was difficult? 
1) I will not be able to do this without an available application source code that works. 
2) Not realising the need for webhooks. 
3) Not understanding the source code and why a committed change was not triggering anything until a classmate helped out and things started to make sense
4) Initially, I encountered several connections issue/ no message is 'triggered', so I started troubleshooting:
- Did I ensure that integration with Telegram is successful? 
- Did I choose the right channel in IFTTT? --> I forgot to select the correct channel initially!
- Did I name your event correctly in your CURL function? --> There was a typo on my event name! 
- Is my IFTTT Webhook link correct? 
- Is there some typo on my CURL functions? --> This was the case!
- Last resort, ask a friend! 

## What else did I try? 
- Prior to this, i forked several repositories on the marketplace where I was exposed to connection to Heroku. 
- In one instance, I successfully forked and executed an application code that works- Forwards message from a Channel to another Telegram Group. 
- However, when I tried to commit changes, there was nothing to "fire" and hence no workflow created in Github Actions. I did not understand the code and how Github Actions worked and hence, project was scrapped. 
-  Learning journey: Do not blindly copy quotes without understanding the mechanism. 

## Outcome 1- The Commit Changes worked!!!
## Outcome 2- The bot works and a message was really sent!!! (after 10million trial and error)
## Outcome 3- I learnt how to add images to ReadMe files and used html to shrink the image size too! 
