# Build a Chatbot with Amazon Lex

**Author:** Gilbert Emodi  
**Email:** zemodi99@gmail.com

---

![Image](http://learn.nextwork.org/ecstatic_beige_calm_tarapirohe/uploads/aws-ai-lex1_505be5b8)

---

## Introducing Today's Project!

### What is Amazon Lex?

Amazon Lex is a service for building conversational interfaces using voice and text. It leverages AI and NLP to create chatbots and virtual assistants. It's useful for automating customer support, streamlining workflows, and integrating with AWS serv

### How I used Amazon Lex in this project

We used Amazon Lex to set up a chatbot

### One thing I didn't expect in this project was...

I didn't expect how granular you can get with this service.

### This project took me...

It took me under an hour to comeplete this project. I just wanted to 

---

## Setting up a Lex chatbot

I created my chatbot from scratch with Amazon Lex. Setting it up took me no more than 5 minutes, using mostly default settings.

While creating my chatbot, I also created a role with basic permissions because Amazon Lex needs the permission to call other AWS service. Later in this project I'll be integrating Lex with a Lambda function

In terms of the intent classification confidence score, I kept the default value of "0.40". This means there should at least be a 40% match between the user's input and the intent I programmed, for my Banker bot to respond accordingly.

![Image](http://learn.nextwork.org/ecstatic_beige_calm_tarapirohe/uploads/aws-ai-lex1_97dc2351)

---

## Intents

Intents are what the user is trying to achieve in their conversation with the chatbot. For example, checking a bank account balance; booking a hotel; ordering food. A chat bot is defined by the intents that it supports.

I created my first intent "WelcomeIntent" to greet users at the start of the chatbot conversation when they say "Hello" or any variation of a greeting.

![Image](http://learn.nextwork.org/ecstatic_beige_calm_tarapirohe/uploads/aws-ai-lex1_505be5b8)

---

## FallbackIntent

I launched and tested my chatbot, which could respond successfully if I enter "Hello", "Hi", or "Help Me" and a closing response i.e. how the chatbot will respond.

My chatbot returned the error message 'Intent FallbackIntent is fulfilled' when I entered "Good Morning" This error message occurred because that phrase was not programmed in to the "Sample Utterances" during set up of the chatbot.

![Image](http://learn.nextwork.org/ecstatic_beige_calm_tarapirohe/uploads/aws-ai-lex1_505be5b8)

---

## Configuring FallbackIntent

FallbackIntent is a default intent in every chatbot that gets triggered when the chatbot does not recognize the user's goal/purpose.

I wanted to configure "FallbackIntent" because the default closing response to the user is not easily understandable.

---

## Variations

To configure FallbackIntent, I had to create my own closing response in the intent's set up page. "Sorry I am having trouble understanding..."

I also added variations! What this means for an end user is they get to see different forms of my chatbot's response. This is done to give a bit of uniqueness and more of a human feel.

![Image](http://learn.nextwork.org/ecstatic_beige_calm_tarapirohe/uploads/aws-ai-lex1_c4fc89af)

---

## Initial Responses

As an extension for this project, I'm setting up initial responses, which are greetings or confirmations your chatbot sends right after it figures out your user's intent.
I've set up initial responses for greetings

The initial response messages I set up are "Hmmm this is interesting..." and "One moment..." For the user, this means they sent a message and the chatbot couldn't decipher the user's intent with at least 40% accuracy.

![Image](http://learn.nextwork.org/ecstatic_beige_calm_tarapirohe/uploads/aws-ai-lex1_09bcb9701)

---

---
