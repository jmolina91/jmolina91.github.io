---
layout: post
title: "The five ideals in software development"
date: 2020-03-22
desc: "Explanation of the five ideals that Maxine, the main character of The Unicorn Projects, tries to accomplish in her company Parts Unlimited"
keywords: "Software, Development"
categories: [software development]
tags: [sw, delivery, teams, performance]
icon: icon-html
---
## Introduction
Nowadays, still a lot of companies struggle to deliver software quickly and efficiently, and you ,as a developer, might be wondering why this is happening in your organization as well.

In today's posts we will talk about the Five Ideals that are explained in "The Unicorn Project". Those ideals are five aspects that your company needs to implement in all the teams so that, on one side, the customer features that you develop are the ones that the customers actually need and, on the other side, that they are delivered in a flow manner.

For each ideal we will explain what is the current problem we might be facing and how to properly address it with real examples. Let's check it out!

## The First ideal: Locality and Simplicity
Locality in our organizations allows teams to make decisions without having to communicate and coordinate with people outside the team. For that to be possible, the simpler your system is, the easier would be for your team to own it.

### The problem
Imagine that you want to develop a feature in your product to display new customer information in the Customer Backoffice and for that you need an endpoint in the backend to query the data, the API needs to retrieve information from a new column that needs to be created into the database to store this value and, of course, all this needs to be tested and deployed. 

When there is no Locality, it might happen that every team owns one piece of this process, meaning that the frontend developer needs to wait for the backend developer, who is in the Backend Team, to provide the endpoint, that at the same time needs to wait for the Database Team to create a new column in the database. Then, you send your artifact to QA Team to test it and finally to the Devops Team to deploy it to production.

Communicating to all these people is not only exhausting, but also most of those people will be waiting for another team to finish something, which at the it ends ends up in delaying the implementation of the feature.

### The solution
If we want to reduce the communication between teams, instead of splitting the teams by area of expertise, we should split them by the domain area they work on, or bounded contexts ,as **Domain-Driven Design** (DDD) (link) explains. Let's assume that the company we were talking about was a financial company, the Customer Backoffice team should be in charge of delivering value when it comes to showing the proper data to the customer and the current status of their loans, whereas the Merchant Backoffice team should be a completely independent team in charge of allowing the merchant to properly operate.

Another imporant aspect to achieve Locality is to have **Cross-Functional teams** where every team has enough people to deliver the proper value, not only developers, but also product people or even domain experts. Like this, there is no need to request for help externally and the time that the team needs to wait gets reduced, and therefore, the delivery happens faster.

## The Second ideal: Focus, Flow and Joy
Focus, Flow and Joy refer to how challenging and interesting your daily work is.
### The problem
Have you ever seen yourself blindly working on small pieces of the whole, only seeing the outcomes of your work after three more teams have finished and during a deployment when everything blows up? Or, have you ever worked in tasks that take two weeks or one month to complete? These situations, most likely, will make you feel bored or fustrated which could derive in lower motivation and therefore slow delivery.

On the other hand, we do not perform repetitive tasks as engineers, but instead, we resolve different complex problems almost every day. However, you might have been in organizations where there was no space for learning and growing your capabilities which lead to a non-enjoyable environemnt.

### The solution
Working in **small-batches** where you can see the value of what you are developing by deploying to production very often without depending to anyone else and also reducing the **Work In Progress** (WIP) cause a feeling of satisfaction and therefore high motivation which is known as **Flow**(link) state.

In order for the engineers to feel challenged and grow their skills it is necessary to provide them a space for learning with **trainings, workshops or talks** within your company. Talk to 
your CTO or your lead and convince them to invest time and money to improve developers skills; the company will benefit from it in a mid/long-term and people will be happier.

## The Third ideal: Improvement of Daily Work

### The problem

### The solution

## The Fourth ideal: Psychological Safety
Psychological Safety is about making it safe for everyone in the company to talk about problems without being afraid of being punished for making a mistake.

### The problem
In one of the companies I worked at, we had a Post-mortem(link) about an incident that ocurred that made us loose some money. Once the issue was fixed, the CTO put together everyone that could be involved in the outage (developers, sysadmins and product people) and ask who made the mistake. The person who made it did not say anything at first becuase they were afraid of being punished, but after some days they confessed. What did the company do? Fire them! 

If you were an empoloyeee of this company your very first though would be: "If I mess it up at some point I am not going to say anything because I don't want to loose my job" which means that employee stop being honest with company. 

However, when an outage like the one mentioned above happens, you need to find a way to prevent it from not happening again, and that needs honesty from people to talk in front of everyone else assuming they made a mistake and explain openly what and how everyhing happened to find a propre solution.

### The solution

## The Fifth ideal: Customer focus
### The problem

### The solution

## Conclusion