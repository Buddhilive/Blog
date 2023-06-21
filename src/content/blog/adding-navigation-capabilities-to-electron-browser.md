---
title: "Adding Navigation Capabilities to Electron Browser"
description: "...."
pubDate: "2019-01-17"
categories: 
  - "archived"
---

[![](/images/Adding-Navigation-Capabilities-to-Electron-Browser.jpg)](https://1.bp.blogspot.com/-yTtiGffn3II/XECKM2yxVAI/AAAAAAAAIIg/tPg3oQKDHLUlQxOwqjx33H2hSlJxtoMLACLcBGAs/s1600/Adding-Navigation-Capabilities-to-Electron-Browser.jpg)

  

In the previous tutorial we discussed about Electron and the Electron Web Browser we are going to create. If you haven't read the previous tutorial, I recommend you to [read it here.](https://www.buddhilive.com/2019/01/how-to-build-web-browser-using-electron.html)

  

Now we are having a browser template which can load a web page using Electron webview. In this tutorial we are going to add some navigation capabilities to this browser. At this level the buttons on the browser doesn't work. We are going to add some code to make them work.

  

Now in the "Starter" folder you can see a file called **"electronbrowser.js"**. This is the file that will handle the functionalities of the browser. Open this file in your favorite text editor (mine is Adobe Brackets). You can see some initializing of variables there and some commented lines. Click below the comment _"//Navigation Functions"_ and add this code. Those are inbuild navigation methods available for Electron webview.

  

  

  

  

Now click under the comment _"//Event Listeners"_ and add the following code.  
  
  

  

  

Now if you run the application using **_"electron ."_** you can see the back, forward, refresh and home buttons are working. But there's a problem. The address bar of the browser doesn't show up the URL of the current page. fix it with this code. Click under comment _"//Show URL of the web page"_ and add this code.  
  
  

  

  

Now go to the event listeners below and add this code  
  
  

  

  

If you run the application now, you can see the address bar is showing the URL of the current web page. Not only that, we must be able to visit a URL that we type in the address bar. For that to happen click below comment _"//Load URL from the textbox"_ and add the following code;  
  
  

  

  

Then go to the event listeners below and add this code;  
  
  

  

  

At last for this chapter of the tutorial, we are going to add the below codes to indicate that the web page is still loading;

  

Under comment _"//Loading Status"_  

  

  

Under comment _"//Event Listeners"_  

  

  

[![](/images/navigation.png)](https://2.bp.blogspot.com/-BB50FhNMELM/XECN8x-lW7I/AAAAAAAAIIs/70l5V-kENRwsrHy_z61ixJdPfHxqro7LQCLcBGAs/s1600/navigation.png)

  

> [Next tutorial: Adding Bookmarks in Electron Browser](https://www.buddhilive.com/2019/01/how-to-add-bookmarks-in-electron-web.html)
