---
title: "How to add Chrome Browser's Tirex Game to Electron Browser?"
description: "...."
pubDate: "2019-01-17"
categories: 
  - "archived"
---

[![](/images/How-to-add-Chrome-Browsers-Tirex-Game-to-Electron-Browser.jpg)](https://2.bp.blogspot.com/-S0C1olbBKis/XECSkUFGtOI/AAAAAAAAIJQ/_leRMbpq1zwBSo2xYSlmVj-ufIQVim2-QCLcBGAs/s1600/How-to-add-Chrome-Browser%2527s-Tirex-Game-to-Electron-Browser.jpg)

  

In the previous tutorial we added the ability of storing and viewing bookmarks in the Electron Browser. If you missed that tutorial, I do recommend you to [read it here](https://www.buddhilive.com/2019/01/how-to-add-bookmarks-in-electron-web.html).

  

In this tutorial we are going to add a cool feature. You all know the Tirex dinosaur game that shows up in the Google Chrome browser when you are offline. Well we going to add that in to our Electron Browser. First I would like to thank to [The Code Post](https://www.thecodepost.org/internet/play-hidden-t-rex-game-offline-chrome/) for sharing the source code of this cool offline game.

  

Go to **"electronbrowser.js"** and add the following variable in the _"//Initializing the components"_ section

  

  

Then click below the comment _"//Load Tirex game when failed to load"_ to add the following code;

  
  

Go to _"//Event Listeners"_ and this code.

  
  

Now we need the "Tirex Dinosaur Game". Create a HTML file in the "Starter" folder and name it **"tirex.html"** and add the following code.

  
  

Great! Now it's time to try this. Make sure you are offline before you run the application at this moment. Well, since you are offline now, you will be redirected to the "Tirex Dinosaur Game". Press space and start playing the "Tirex Dinosaur Game" as same as on Chrome browser.

  

[![](/images/tirex_game.png)](https://1.bp.blogspot.com/-s3gIT9xrNPs/XECTzb7GemI/AAAAAAAAIJc/McyB409olZwJ_oLGTtw_41ZEUC9gbk8BwCLcBGAs/s1600/tirex_game.png)

  
  

> [Next Tutorial: Adding DevTools to Electron Browser](https://www.buddhilive.com/2019/01/how-to-add-devtools-to-electron-browser.html)
