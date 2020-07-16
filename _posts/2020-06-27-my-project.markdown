---
layout: post
title: Think About Your Audience
date: 2020-06-27 00:00:00 +0400
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: mac.jpg # Add image post (optional)
tags: [Productivity, Software] # add tag
---

I'm an intern at PublicLab and I'm working on the PublicLab Editor. The name of my project is *Fortification of the Editor and adding custom insert modules*.

### PublicLab

The Public Laboratory for Open Technology and Science is a non-profit organization that facilitates collaborative, open source environmental research in a model known as Community Science. It supports communities facing environmental justice issues in a do it yourself approach to environmental monitoring and advocacy. People share research notes, ask questions to learn about and solve environmental problems on their own. Public Lab is a big community with a lot of projects 

### Public Lab Editor

On the Editor you can share research notes, activities, ask questions, post events and even share blogs! The Editor this SoC season comprises a team of four, two outreachy and two gsoc interns. The Editor has two modes, a *wysiwyg* (what you see is what you get) rich text mode and a *markdown* mode. Breaking down the Editor,
1. The first part is the **Title Module**
2. The second part is the **Main Image Module** which adds a header image to the post.
3. Next is the **Map Module** which adds a user specific location to get a better idea of the Environmental aspects of the loaction of the writer.
4. After that is the **Body** where the content goes.
5. Lastly there is a **Tagging Module** where related works can be referenced.

Since I'm an avid reader, occassional writer and deeply interested in technological advancements, I was very excited to work on this project. And once I started working, the ever positive community input made it even better.

### Fortification of the Editor and adding custom insert modules

The work started with fixing bugs and working on the existing functionality in the first phase. The Editor is built on the Woofmark library, which is no longer actively maintained, and is full of bugs. We identified the many bugs resulting in a bad editing experience for users of PublicLab.org. These included the instances in which the code breaks. It could be due to conversion from one mode to another or a functionality which fails for a particular case. For fixing bugs, the first step is to trace the bug and find the point at which it breaks and in developing fixes for them, at either the woofmark library level and within our own Editor project. 

A team mate of mine, worked on creating an visual interface in the project where users who are not familiar with github can report issues/ bugs using screenshots, detailed description and GIFs. 

The second phase focused expanding the Editor’s functionality by creating simple and intuitive ways to add advanced content to posts, such as maps, tables, and lists of content from elsewhere on the PublicLab.org website.These inline inserts are managed in a “short-code” syntax. One such task is to introduce an interactive mapping between UI and these shortcode syntax.

The Editor is built on a modular system, and this new work involves developing a new module which allows new content to be selected using a menu or other visual interface. The user will be able to configure and insert their selection and make changes or tweaks to already-added inserts. 

Another important part of the project is development process refinement. Development process refinement is, as the name suggests, about adding features that refines development process. This part included adding tests, linting tool and coverage tracking. This makes the maintainability and ease of contribution facile. This introduced consistency in the coding style, wrt linting. Adding tests ensured that the new features being added do not break the exsisting features.

Last but definitely not the least was UI refinement for the Editor. Every UI change introduced or feature added is done keeping in mind the views and requirements of the community.

### My Task

Since explaining the complete project at one go could be a little tough, I'll tell you about the recent task I completed in detail.

My task was to integrate jest, puppeteer and jest-puppeteer in the project for UI testing in a headless browser. Headless testing is a way of running browser UI tests without the head, which in this case means that there’s no browser UI, no GUI of any sorts. One of the biggest reasons for using a headless browser/carrying out headless testing is performance, since it lets you run tests more quickly in a real browser environment. It is a lightweight, less resource intensive and scripted automation that executes quickly.

I first read about the jest and puppeteer from their official documentation. And then read about jest-puppeteer. My approach is usually to get a basic of gist of how things work and start coding right away rather than going through the entire documentation. And then learn to deal with the errors as I go, which is not at all recommended since I end up going back to the documentation again and again to get a solid grasp of the concepts. You should follow the method that you deem right. 

`Package.json` is the file in your project that lists all the required dependencies. For adding new dependencies you could either use the terminal `npm install ....` or add it in the file along with the version and then run npm install. After installing the dependencies I wrote a sample test learning from a blog. Once I got the tests running, I wrote a config file. 

Config file, in my case `jest.config.js` and `jest-puppeteer.config.js`, sets up the test environment. Once that is done, I wrote tests in small parts. Since a big file makes it difficult to trace the error, write and check as you go. My first test was to click the bold button and find the desired output in the body. When this didn't work I checked if I could find the bold button on the page. When that passed I checked the ouput after clicking the button using screenshot feature. Once I saw that `**strong text**` was added in the page, I used `console.log()` to check the value of the entire body. When it finally worked upto this point did I add the condition to look for the string and compare the result. 

Ta Da! It's done. But it wasn't as easy as it seemed. I then proceeded to write the complex tests.

### Think about Your Audience

Similar to the theme of this post was an introduction that we received from our mentors when we first began working on this project. Sharing a few points, I hope this might help you understand the project that you plan to work on in the future better.  

* Think of your project as a product    
The project, like a product, has a user base (consumers). When you write a proposal or plan to work on a project, think of it as a user. What are the changes that a user would prioritise/want.

* Ask for community input   
Whenever you plan to implement a new feature, run it through the community first. Be vocal and expressive about your opinions and open minded to the views that the share, There's always something to learn from experiences.

* Write structured code   
This is something I learned from personal experiences after making more than a few mistakes. The future devs that will contribute to this project, aren't they your audience too? Follow a consistent coding style. Preferably see how the community works. Linting is a must. Add a test for any new feature. And anything else you learn along the way!

> Happy Coding!
