---
layout: post
title: "Setting up Selenium in Visual Studio Code on MacOs with Apple Chip M1"
date: 2021-11-03 19:08:30 -0400
categories: QA
tags: [Selenium]
years: ['2021']
comments: true
---

# What do I need beforehand?

- [Visual Studio Code][Visual Studio Code] or also known as VS Code
- Latest Java version from [Oracle][Oracle] 
- Java Extension Pack in VS Code
- [Selenium][Selenium] WebDriver
- [ChromeDriver][ChromeDriver] 


## Let's start with Visual Studio Code

I installed [Visual Studio Code][Visual Studio Code] when I first got this laptop long ago, because I read that it is the best text editor to have and it is already an IDE. An IDE is short for `integerated development environment` and it allows different developer tools to work together. It debugs and do many other wonderful things.

I don't remember exactly the steps of installing visual code, but I think it should be simple. Click on this [Visual Studio Code][Visual Studio Code] and scroll all way down to the bottom until you see this image:

![VS-ARM](/public/img/VS-ARM.png)

Click on `Apple Silicon` to install the VS Code, <strong>again this is for MacBook Pro with chip `Apple M1` </strong> or what I usually see `ARM 64` for different downloads.

## The next step, download Java for MacOS M1 Chip

The thing to know, MacBook Pro with Apple M1 chip doesn't come with Java, so we will need to download Java from [Oracle][Oracle]. I created a short video clip below of how to install Java quickly

<iframe width="420" height="315" src="https://youtu.be/ABbsylwIlF4" frameborder="0"></iframe>


[Visual Studio Code]:https://code.visualstudio.com/
[Oracle]:https://www.oracle.com/index.html
[Selenium]:https://selenium.dev
[ChromeDriver]:https://chromedriver.chromium.org/downloads
