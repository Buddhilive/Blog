---
title: "How to Add Bookmarks in Electron Web Browser?"
description: "...."
pubDate: "2019-01-17"
categories: 
  - "archived"
---

[![](/images/How-to-Add-Bookmarks-in-Electron-Web-Browser.jpg)](https://2.bp.blogspot.com/-lGCu9xLEbzw/XECO_K5lSWI/AAAAAAAAII4/yC1KdTZvbe43Hwt-N7riZQ1875ZIlWv3QCLcBGAs/s1600/How-to-Add-Bookmarks-in-Electron-Web-Browser.jpg)

  

In the previous tutorial we added navigation capabilities to our Electron Web Browser. If you missed that tutorial, you can [read it here](https://www.buddhilive.com/2019/01/adding-navigation-capabilities-to.html).

  

In this tutorial, we are going to add bookmark function to our Electron Web Browser. Open the **electronbrowser.js** file and go to _"//Initializing the components"_ and add these variables below;

  

  

  

  

Then click below comment _"//Add a bookmark"_ and add the following code. In this code we collect the URL, title and the favicon of the web page we are going to bookmark and then save it to a JSON array in the JSON file called "**bookmarks.json"** (which is already located in the Starter folder). If you open it, you can see there three bookmarks already stored as an example.  
  
  

  

  

And then go to _"//Event Listeners"_ and add the following code below.  
  
  

  

  

Now we need to see the bookmarks we stored and visit them. For that we are going to create a HTML page with a HTML table which will show the bookmarks we've stored. That means we are going to populate the HTML table with JSON data.

  

First create a HTML file in the "Starter" folder and name it "**bookmarks.html**" and insert this code in to that file;  
  
  

  

  

Then create a JavaScript file named **"loadbookmarks.js"** in the "Starter" folder and insert the following code;  
  
  

  

  

Again go back to **electronbrowser.js** file and click under the comment _"//Go to Bookmarks page"_ to add the following code;  
  
  

  

  

And don't forget to add this code in the _"//Event Listeners"_ section;  
  
  

  

  

Now you can run the application and navigate to a web page, and bookmark it. To view your stored bookmarks click the "More" icon at the top right corner of the browser to find "Bookmarks" menu item and click on it. You will be directed to the **"bookmarks.html"** page displaying the stored bookmarks.  
  

[![](/images/bookmarks.png)](https://1.bp.blogspot.com/-0ZhOrhRUilE/XECRX5GTcRI/AAAAAAAAIJE/6xDc7GB5xwcKkzmn91BhEbqQQgP1FFkYwCLcBGAs/s1600/bookmarks.png)

  

  

> [Next Tutorial: What happens when you are offline?](https://www.buddhilive.com/2019/01/how-to-add-chrome-browsers-tirex-game.html)
