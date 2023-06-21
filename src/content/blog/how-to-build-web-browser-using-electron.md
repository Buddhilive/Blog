---
title: "How to Build a Web Browser Using Electron?"
description: "...."
pubDate: "2019-01-17"
categories: 
  - "archived"
---

[![](/images/How-to-Build-a-Web-Browser-Using-Electron.jpg)](https://1.bp.blogspot.com/-OReAvfCtfbs/XECHQzhY3bI/AAAAAAAAIIM/R8F7t4Z5oXETOUQ9rm-exh3I40-yKN67gCLcBGAs/s1600/How-to-Build-a-Web-Browser-Using-Electron.jpg)

In this tutorial I'm going to show you how to make a simple web browser using Electron and JavaScript.

### What is Electron

Electron is a software framework created by GitHub to build cross platform desktop applications using JavaScript. That means, now you can create cross platform (Windows, Linux, MacOS) desktop apllications using HTML and JavaScript.

Electron uses Chromium to render applications. So can develop any application using JavaScript to run on desktop. With the power of Chromium, you can access all DOM APIs and Node.js APIs as well.

### Electron Webview

Electron Webview is the component we use to build this web browser. Electron webview is similar to Chromium webview which can do rendering, navigation and even event routing.

If you are new to Electron, I strongly recommend you to [read this Getting Started guide.](https://electronjs.org/docs/tutorial/first-app)

### Start Building the Browser

Clone or download the project from [GitHub](https://github.com/Buddhilive/Electron-Browser).

You can see there are two folders in the project **"Starter"** and **"Completed"**. **"Completed"** folder contains the completed browser project while **"Starter"** folder contain the basic browser template where you can add code by yourself referring this tutorial. So you will be able to understand how the browser work and how to use Electron to build a cross platform desktop application.

Now go to "Starter" folder. You can see **"index.html"**, **"main.js"** and **"package.json"** files. You may know this files when you go through the Electron [Getting Started guide](https://electronjs.org/docs/tutorial/first-app).

Open command line and change your directory to "Starter" folder and run **_"npm install"_** to install the required dependencies. Then launch the app using _'**electron .**'_ command, you can see the browser template which loads Google home page. All other buttons doesn't work at the moment. From this point, we are going to add functions to these buttons to get the basic functionality of a web browser.

[![](/images/browser.png)](https://4.bp.blogspot.com/-cEgv29QiWcw/XECH4QqnFeI/AAAAAAAAIIU/U4FMjG3xR6YRvzAebZbPT02-CP3T0Ra8gCLcBGAs/s1600/browser.png)

This browser project is influenced by this [blog post](https://blog.jscrambler.com/building-a-web-browser-using-electron/) and is continued to develop adding more features.

> [Next: How to add Navigation Capabilities to Electron Browser?](https://www.buddhilive.com/2019/01/adding-navigation-capabilities-to.html)
