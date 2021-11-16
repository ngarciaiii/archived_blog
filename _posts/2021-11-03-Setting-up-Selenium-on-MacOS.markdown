---
layout: post
title: "Setting up Selenium in Visual Studio Code on MacOs with Apple Chip M1"
date: 2021-11-03 19:08:30 -0400
categories: QA
tags: [Selenium]
years: ['2021']
comments: true
---

I use MacBook Pro 2020 with chip Apple M1, and was not sure if it is compatible with Selenium, a QA automation testing tool. I also would like to use it with Visual Studio Code, a popular choice of text editior and IDE. I had to google up and this website below is the best choice to follow through. 

https://funnelgarden.com/setup-selenium-with-java-on-visual-studio-code/


# What do I need beforehand?

- [Visual Studio Code][Visual Studio Code] or also known as VS Code
- Latest Java version from [Oracle][Oracle] 
- Java Extension Pack in VS Code
- [Selenium][Selenium] WebDriver
- [ChromeDriver][ChromeDriver] 


## 1) Let's start with Visual Studio Code

I installed [Visual Studio Code][Visual Studio Code] when I first got this laptop awhile ago, because I read that it is the best text editor to have and it is already an IDE, or `integerated development environment`. It allows different developer tools to work together. It debugs and does many other wonderful things.

I don't remember exactly the steps of installing Visual Studio Code, but I think it should be simple. Click on this [Visual Studio Code][Visual Studio Code] and scroll all way down to the bottom until you see this image:

![VS-ARM](/public/img/VS-ARM.png)

Click on `Apple Silicon` to install the VS Code, <strong>again this is for MacBook Pro with chip `Apple M1` </strong> or what I usually see `ARM 64` for different downloads.

## 2) The next step, download Java for MacOS M1 Chip

The thing to know, MacBook Pro with Apple M1 chip doesn't come with Java, you could check by typing `java -version` in terminal. So we will need to download Java from [Oracle][Oracle]. I created a short video clip below of how to install Java quickly. I already installed and don't want to reinstall. Just follow through without cancelling unless you feel necessary.

<iframe width="560" height="315" src="https://www.youtube.com/embed/ABbsylwIlF4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
 <br>
After installing Java SDK, open up terminal and then type either `java -version` or `javac -version` and it should show the version. `Javac` is java complier.  I forgot to add, it is possble to open up terminal in Visual Studio Code. I use terminals in Visual Studio Code to stay focused on whatever the projects I am working on. Visual Studio Code is changing things, more conventional. 

## 3) Add Java Extension Pack in VS Code







[Visual Studio Code]:https://code.visualstudio.com/
[Oracle]:https://www.oracle.com/index.html
[Selenium]:https://selenium.dev
[ChromeDriver]:https://chromedriver.chromium.org/downloads
