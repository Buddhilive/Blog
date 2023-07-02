---
title: "Moving Camera with the Player – GDevelop"
description: "...."
pubDate: "2020-04-24"
categories: 
  - "archived"
---

[![](/images/00_GDevelop_Tutorial_for_beginners.PNG)](https://1.bp.blogspot.com/-ooaAnBJVIVI/XpyZp6wIMkI/AAAAAAAALFU/W0VAzxGoDhUpYFr_B7oKG-MB85uJSOmIwCPcBGAYYCw/s1600/00_GDevelop_Tutorial_for_beginners.PNG)

  
  

In the [previous lesson](https://www.buddhilive.com/2020/04/flipping-objects-in-gdevelop.html), we learned how to flip an object in GDevelop. In this lesson we are going to learn how to set up camera to follow the player. As you all know, in platformer games, the player moves long way beyond the screen. So always the camera is focused on the player. Otherwise we won’t see the player when it moves beyond the screen. So the main focus point of the camera is player. This can be achieved very easily in GDevelop.

### Step 1

Add new empty event. We don’t need a condition for this event. We only need to add an action here. Now go to add action and search for **“Center the camera on an object”.** Select “Bob” as the object. Because “Bob” is our player. Leave the other settings as defaults. Click **OK** to add the action.

  

[![](/images/31.Center+the+camera+on+an+object.PNG)](https://1.bp.blogspot.com/--0f2avg7NgQ/XqMs1Y7ObZI/AAAAAAAALNw/5ZPpsvptIEIhXV1ANHfZb6GHBS1Iaa2PgCLcBGAsYHQ/s1600/31.Center+the+camera+on+an+object.PNG)

  

And that’s it. It’s simple. Your event should look like this

  

[![](/images/32.event.PNG)](https://1.bp.blogspot.com/-VeKZ453mc-0/XqMtPam4XgI/AAAAAAAALN4/1Xfp8JiLqjAFaksA2kCltryIKuZDt8DXQCLcBGAsYHQ/s1600/32.event.PNG)

  

Ok, you may be wondering how my screenshots went dark. Well, there’s a dark mode available in GDevelop. If you like to activate it, go to _File > Preferences_ from the menu. Then in the popup, under _PREFERENCES_ tab set the _UI Theme_ to **Dark** and _Code editor Theme (this is optional)_ to **Visual Studio Dark.** Close the popup and you have dark theme activated GDevelop.  
  

[![](/images/33.dark-them-for-gdevelop.PNG)](https://1.bp.blogspot.com/-x7Zo2SZCObU/XqMtfsaJe6I/AAAAAAAALOA/HaNV8sKWpowZwP6c-qp7biNE37n9lv84wCLcBGAsYHQ/s1600/33.dark-them-for-gdevelop.PNG)

  

In the [next tutorial](https://www.buddhilive.com/2020/05/adding-jump-through-platforms-gdevelop.html), we will learn how to create a “Jump Through” platform.  
  

Feel free to ask any question regarding this lesson in the comment section below.
