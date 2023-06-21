---
title: "Adding Coins and Score System – GDevelop"
description: "...."
pubDate: "2020-05-03"
categories: 
  - "archived"
---

[![](/images/00_GDevelop_Tutorial_for_beginners.PNG)](https://1.bp.blogspot.com/-ooaAnBJVIVI/XpyZp6wIMkI/AAAAAAAALFU/W0VAzxGoDhUpYFr_B7oKG-MB85uJSOmIwCPcBGAYYCw/s1600/00_GDevelop_Tutorial_for_beginners.PNG)  

  

In the [previous lesson](https://www.buddhilive.com/2020/05/adding-background-objects-to-game.html) we learned to add background objects and then we design and develop the platform furthermore. In this tutorial, we are going to learn how to add collectible items and a score system. Here we are going to add some coins as the collectible items and we are going to give points when the player collects them.

  

We are going to add a _Sprite Object_. Go to _assets folder > coin_ and add all the images to the animation. Enable loop option to keep the animation playing continuously. Name the object as “Coin”.

  

[![](/images/43.coin.PNG)](https://1.bp.blogspot.com/-cQClkdyo1oE/Xq79ePk4OyI/AAAAAAAALUo/EvxGj_Q1M-wWOxOz7tynasoCXiACoVZ7ACLcBGAsYHQ/s1600/43.coin.PNG)

  

Now drag and drop the coin on to the canvas. Adjust the size that fits to the scene. Now as we did in the previous tutorial, you can clone the object by press and holding Ctrl (Cmd on Mac) while dragging. And to keep the coins align, press and hold shift while you are moving the cloned coin object. This will help you to move the cloned coin in the same axis of the original coin, thus aligning the coins properly. Place few coins in random places in your scene.  
  

Now here we come to the logic part. When the player hits a coin, that coin should disappear and at the same time the player gets points. Let’s see how it is done through events. First, we’ll delete the coin whenever the player hits it. Go to Event editor and add a new empty event. Now go to add condition and search and select **“Collision”.** (Note: there are few types of collision conditions. What we use here is “Common conditions for all Objects/Collision” condition). Select first object as “Bob” and the second object as “Coin” and click **OK.**  
  

[![](/images/44.coin.PNG)](https://1.bp.blogspot.com/-tB7dAiJ7DxI/Xq79xvuoFyI/AAAAAAAALUw/b9POzJ0YJ4Y25oUDxD7Tb4sfIpL9TRXBwCLcBGAsYHQ/s1600/44.coin.PNG)

  

Now go to actions and search and select **“Delete an object”.** Select “Coin” as the object and click **OK.** Now let’s play a sound when the coin disappears. We need to add another action right below the delete action. Go to action and search and select **“Play a sound”.** Click **Choose anew audio file** from the _Choose the audio file to use_ drop down menu. Navigate to our _assets folder > audio > coin.wav_ and add the audio file. Make sure _Repeat the sound_option is set to “No”. Keep other settings as it is and click **OK.**

  

[![](/images/45.coin.PNG)](https://1.bp.blogspot.com/-E9H6RvspBpo/Xq7-Fvu_0OI/AAAAAAAALU4/Vw56kCal4nYaLhIFNGYrAsOrcC1w-ZsQwCLcBGAsYHQ/s1600/45.coin.PNG)

  

  

[![](/images/46.coin.PNG)](https://1.bp.blogspot.com/-OxmfB971R_c/Xq7-_6uYvVI/AAAAAAAALVE/T6AC3C6A33MA3J31NHMvgHf8rritUxadQCLcBGAsYHQ/s1600/46.coin.PNG)

  
Hit the preview button to preview the changes we did so far. Next, we need to give points when a coin is collected, and we need to display the total points the player scored. We need to store the score to display it. For that we need variables. Variables are used to store information. It’s like a potion of memory for computers. If you are familiar with programming you already know what a variable is. If you have no experience in programming, don’t worry, that doesn’t matter much.  
  

There are three types of variable we use in GDevelop. According to official GDevelop documentation;  
  

> - _**Object variables** are private variables, specific to each instance of an object. This means that each instance can store its very own values, without them being shared with the other instances. It can, for example, be useful if we want to change the life of each enemy._
> 
> - _**Scene variables** (the most used ones) are variables attached to a scene. This means that their values are not shared with other scenes in our game. It is useful to store information only relevant to the currently played scene. For example, the life of the player or a score._
> 
> - _**Global variables**, as the name suggests, are global in the whole game. Values are shared with all scenes in the entire game. It is useful if we would like to store information that we want to share between all scenes such as the amount of bullet or amount of money the player has._

  

  

What we are going to use here is a **Scene Variable.** Normally you don’t need to create a variable at the beginning. You can create one and use it on the spot. Go to action in the same event we created for deleting coin. Search and select **“Value of a scene variable”.**Click the button next to **Variable** drop down (drop down must be empty as we have not defined any variable yet). This will open the “Scene Variables” popup window. Currently it is empty as we have not created any variable yet. Click the **+** button to add a new variable. Set the variable name as “Score”. Set the default value to “0” and click **APPLY.** Now you will be able to select “Score” variable from the _Variable_ drop down menu. We are going to give 10 points for each coin the player collects. So, set the **Modification’s sign** to **\+ (add)** and set **Value** to 10. Click **OK** to save the action.  
  

[![](/images/48.variable.PNG)](https://1.bp.blogspot.com/-fDGg_eyr61o/Xq7_jkVMZqI/AAAAAAAALVU/Z47z_ir26sseZ45DMHI65xXNVP0hLKZ2ACLcBGAsYHQ/s1600/48.variable.PNG)

  
  

[![](/images/47.score.PNG)](https://1.bp.blogspot.com/-5G9IneaaOBE/Xq7_RxWgwQI/AAAAAAAALVM/gEuCqXpTjRsWEiGkTFXsN4bM14g_WwT4wCLcBGAsYHQ/s1600/47.score.PNG)

  

Let’s display the score in the scene. We need to use a **Text Object** to display the score. First, we need to add a new layer to hold the Text Object. Why? If we add the Text Object to the default layer, when the player runs, the Text Object will not remain fixed to the screen position. It will act as other background objects in the scene. To avoid that, we are going to place the Text Object in a different layer. So, open the **Layers** editor (as we did to change the color in the previous lesson) and click **ADD A LAYER**. Rename the new layer to “UI” and close the Layers editor.  
  

[![](/images/49.layer.PNG)](https://1.bp.blogspot.com/-D6i9XqQZ2sQ/Xq7_vMjiZzI/AAAAAAAALVY/38pxXKn4bSY2u1JzU_2kveFiEfshTznqACLcBGAsYHQ/s1600/49.layer.PNG)

  

Add a Text Object (from Objects panel). Name it as “ScoreDisplay”. Set font size to 36, enable Bold and change the text to “Score :” (you can change the color if you like) and click **APPLY.**

  

Drag and drop the “ScoreDisplay” text object to the canvas. Position it to Left top corner of the canvas. Now in the properties panel for the text object, select “UI” layer as the _Layer_from the drop down menu.  
  

[![](/images/51.layer.png)](https://1.bp.blogspot.com/-TJTGy2g0S0k/Xq8ADdF924I/AAAAAAAALVk/Etlv2bkfb9Iz7R1LVRz5R9kTs-ff6QoPwCLcBGAsYHQ/s1600/51.layer.png)

  

Now switch to Event editor. Add a new action to the coin deleting event. Search and select “**Modify the text”.**Select the object “ScoreDisplay” as the object. Set the _Modification’s sign_as **\= (set to).** Here we can’t assign the Score variable as value. Since this is a text object, it only displays text not numbers. Well, even numbers are displayed as text. Our **Score** variable is a number. We need to convert it in to text. If you are familiar with programming, you can understand what is going on here. Well I’m going to show this process in a short video for you to understand.  
  

<iframe allowfullscreen data-thumbnail-src="https://i.ytimg.com/vi/EPQtfIXnPEw/0.jpg" frameborder="0" height="360" src="https://www.youtube.com/embed/EPQtfIXnPEw?feature=player_embedded" width="100%"></iframe>

  

  

Well, if you did everything correct, your event should look something like this;

  

[![](/images/52.event.PNG)](https://1.bp.blogspot.com/--0n5dNJqWGE/Xq8AK5HM6WI/AAAAAAAALVo/MFcw-Txis9sWXrm3bRv017mxRMspBg9owCLcBGAsYHQ/s1600/52.event.PNG)

  

Hit the preview button and preview the game. And voila! The score shows for each coin the player collects. In the [next lesson](https://www.buddhilive.com/2020/05/adding-enemies-to-game-gdevelop.html) we are going to learn another important thing.

If you have any doubts in this lesson. Please feel free to ask it in the comment section below.
