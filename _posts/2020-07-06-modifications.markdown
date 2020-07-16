---
layout: post
title: Modifying Expectations
date: 2020-07-06 13:32:20 +0300
description:  # Add post description (optional)
img: how-to-start.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Outreachy, Opensource]
---
Hey! So we are back again, and this week's topic is "Modifying Expectations". When we begin working on a project we have a very vague idea in mind of what exactly we'll be doing. It's an idea in it's initial stages. The contribution period gives you a chance to get to know a project better. You familiarise yourself with the code, the issues, the mentors and community and that's when the seed of idea is sown. You start recognising the bigger issues, and think of the best possible solutions. With each step, the idea takes shape. Finally at the end of the one month long, or possible longer contribution period, you write a proposal. Your proposal is a collection of all these issues and your solutions. But very often, we need to modify the plans.  Maybe your project turned out to be more complicated than you or your mentor anticipated. Maybe you needed to learn some concepts before you could tackle project tasks. Maybe the community documention wasn't up-to-date or was wrong. Maybe the issues that you recognised were not as high priority as the one your mentor mentioned, or maybe they were not required at all. Maybe what you thought of as bug, is not what it seems :P
![Bug or feature?]({{site.baseurl}}/assets/img/bugfeature.png)

## Original Project Timeline

My original project timeline had three phases:
1. Bug finding and fixing
2. Making modifications to existing features
3. Adding new features and custom insert modules

When I started working, after a conversation with the team and mentors, the project plan changed majorly for me. I had overlooked a large part of the need of this project and admittedly, my proposal was more about what I wanted to see the Editor as by the end of the internship. 

## Modified Project Plan

Keeping in mind the needs of the community and the having a long sighted vision for this project, some major changes were:
For the maintainability and ease of contribution:  
* Adding a linting tool
* Adding a test suite   
* Adding a workflow so that users can report bugs     
And shooting down a few ideas to make the project more realistic. The pace also changed because of the presence of the team and the covid outbreak.

## My accomplishments so far

So far I've worked on two feature modifications:
1. Adding a decenter feature to the existing center alignment feature.
2. Changing heading back to plain text.

In the development refinement:
1. Integrating jest puppeteer for UI testing.
2. Defining basic implementation tests for some features like bold, italic, heading, center alignment and title.
3. Updating node versions
4. Minor bug fixes

## Project goals that take longer than expected

The issues that made my work slower and took more time than anticipated were definiltely the bug fixes. With adding a new feature or implementing a change, you have a defined set of operations in mind. But bug fixes are unpredictable. You first trace down the bug to find the code that breaks, then try to understand the intended implementation of the code and the actual implementation. Once the difference is highlighted, it is easier to pinpoint the exact part which needs work. And finally you try to make it work as intended. What follows is rigorous testing. 

## What would you do differently if you were starting the project over?

This was a very interesting question asked by the outreachy organizers. If given the chance there's not much I could or would change. I started with a slow pace and faced some major issues at a point of time, but the mentors' support helped me get back on track. At times I had to go through articles over articles to fix some minor errors. But over the past one and a half month, I've gained better debugging skills, a more open mindset for discussions, more confidence in my abilities and an experience of a lifetime.

We're close to releasing the next version of Editor as a team and I couldn't be more excited. As of right now, there is more debugging, testing, refinement and feature implementations in store for me. 