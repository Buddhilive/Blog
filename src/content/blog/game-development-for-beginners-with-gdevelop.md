---
title: "Game Development for Beginners with GDevelop"
description: "...."
pubDate: "2020-04-19"
categories: 
  - "archived"
---

  

[![](/images/00_GDevelop_Tutorial_for_beginners.PNG)](https://1.bp.blogspot.com/-ooaAnBJVIVI/XpyZp6wIMkI/AAAAAAAALFQ/7gektVMe7q8wpv1ut6zLDFUHZPuda_JUQCLcBGAsYHQ/s1600/00_GDevelop_Tutorial_for_beginners.PNG)

  

GDevelop is free and open source 2D Game Development tool. It’s and easy to learn and easy to use game development software. Anyone can start building games with zero programming knowledge. GDevelop provides a easy and understandable expression builder to program a game. You can develop a whole 2D HTML5 games using GDevelop.

  

Starting from today, we are going to share how-to guides to learn game development with GDevelop. As the beginners tutorial, we are going to create 2D Platformer game. In this beginner tutorial, we hope to cover main concepts of GDevelop for you to understand how to develop 2D HTML5 games.

  

### Step 1

First of all, [download and install GDevelop](https://gdevelop-app.com/) in your computer. It’s completely free. After installing GDevelop, launch the application. You will see a welcome page as shown in the image below.

  

[![](/images/1.main.png)](https://1.bp.blogspot.com/-9MBnxS7j9Zw/Xpyat7JuCWI/AAAAAAAALFc/jEtcRPQGGjUdNt5F14qxALqtxCtbUG-GACLcBGAsYHQ/s1600/1.main.png)

  

  

We are using a free game assets pack [found here](https://bayat.itch.io/platform-game-assets). It’s also an awesome free assets pack for platformer game. There are lots of assets in the pack. However we refined the assets in it and select few of them which we use for this tutorial and create a minified version of the pack which you can [download from here](https://drive.google.com/file/d/12-2OgIiQvwc7aoQa81P-wnBXWrxmGVAq/view?usp=sharing). Extract the assets files. Now we are ready to begin game development.

  

### Step 2

Now click **_Create a New Project_** button. From the _Create a New Game_ popup window click **Empty Game**. (You will need to scroll down to find this option.)  
  

[![](/images/2.empty-game.PNG)](https://1.bp.blogspot.com/-m1iZ5lSK-s0/XpybAAOOmEI/AAAAAAAALFk/lDlrA3LLSioXRIMXeafooaHUa4fAdyYLwCLcBGAsYHQ/s1600/2.empty-game.PNG)

  

This will launch an empty game project and your screen will look something similar to the screenshot in figure 1. To begin, we need to create our first scene. Scenes are different screens in your game. Home screen, game screen, game over screen etc are all scenes. We add all our game graphics to those scenes. So to start, let’s create our first scene. In the project manager panel (the panel in the left side) click **\+** button next to _Click to add a scene (Under Scenes)._ This will add a “NewScene” to your project. To make things more clear and precise, let’s give this scene a proper name. Click 3 dots next to “NewScene” and select **Rename.** Set the name of the scene to “Level 1” and hit Enter. (You can rename scenes later too. But I recommend do it in the beginning. Try to give meaningful names. This will be useful when your game grows with many scenes). Now click on “Level 1” scene.  
  

<table align="center" cellpadding="0" cellspacing="0" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-55UXqJ9lp94/Xpybw4HXy9I/AAAAAAAALFw/Ph_InfEipcMWxK8c52myS7co0b5J_-a-wCLcBGAsYHQ/s1600/3.project-main-page.png"><img border="0" data-original-height="728" data-original-width="1366" src="images/3.project-main-page.png" style="height: auto; width: 100%;"></a></td></tr><tr><td style="text-align: center;">Figure 1</td></tr></tbody></table>

  

[![](/images/4.new-scene.png)](https://1.bp.blogspot.com/-4BbPNDq_Avw/XpycD-29cFI/AAAAAAAALF4/OzntQNsGCpcnEEOokCybN-VRVOCnMprIwCEwYBhgLKs0DAL1OcqxYoBCEJVS60JGICk7LSbu6keZAh7tGh-Pg-umed0dLsxPE9SHOm-c9c4Ql5sLNHRvm0HTl3-z4uHugJ_wePIlpRHaFbKVFu4Z5y8_C_dMQ56V565rI1GNnVfKfYUd61U30G3fQUSNao8BOlS7dhSP8vsTLW74gtBrPjklJVem_YVxKNjfNWA8O3vlib8uXR8YZ-5NbKkR1TXD3ONpS1IDJTJ70ZlZ3_J8BP8Sk-NHxkVsydrmOJ0K5ZA_Ctl_SnHl7mi80VFGK7H-IfQA60S8KwKd4o3Wt_wr5zSEdv7meSXn53F5YQfd5fm6QUZMSclEawFtatCXB022dmZBtG8zMEydwVC76lHiQRxSPvCOVccDb32xTFvRhAF6d_5gWepISF2PIEbTbQu3h-ViBXCF56bRzmzUlkqAHk-7lVK0Mtd5v0zm0I8GnUKyCBBjq77ZUKL-H8qSz7zGXIcNGyYD6MTsSmjBRlsJxrCIIB4CcHtS3FeXoHUy-zvnfu3oQqO2GelkqE4uYuzKwcTrY9fx_7QbHpnPfPn-YOxmp4e8pVZnUkaMkqtpc6B5XC_8_5qWSI9sSjQXPN8AHBO9gS23jZgehw4_Dbo0wjb3y9AU/s1600/4.new-scene.png)

  

You will be able to see a screen similar to the screenshot above. Here there are two tabs with the name “Level 1”. First one is the Scene Editor or game interface which users will see. Second one is, as it says, the Event Editor for the scene. This is where we include all our game logic or where we program the game. Each and every scene has its own Event Editor.

  

### Step 3

Now let’s import our first game asset to the scene. Click **\+** button next to _Add new object_ in the object panel. (This is the panel located in the right side). This will open _Add a new Object_ popup window. Select **Sprite.** (Sprites can be players, enemies, items etc. These objects can be animated). This will open another popup where you can insert a game object.  
  

[![](/images/5.add-object.PNG)](https://1.bp.blogspot.com/-N_vinaKIvBo/Xpyc2uhkcAI/AAAAAAAALGE/Ib31gi3q6Fki2qPB5hEglJTk48dHXf8OQCEwYBhgLKs0DAL1OcqyRCPn9GmfMRICL0bGgai5_H3WH-anKVJ8ay3WkikJK9I8QyGcs2q6M0ttw-F-2pk7rX9uCvrWA96SaaI6UHhLc3_8lfzHSnyMh1jq46daoCb2Uigj6eniFhhFdcutiGNLoTpGbG-1K6Gom0ecHh18FExgXY_L9hAmjdyhl9JYwqib5yRBI4uMncebC0T9_zCtsJoY-O4L_BAz4BcTWj9XX9UUQV0vVvBFzP5umbyJd6MIKqBesB0tK5y_XONEn1jiHUAXojWxoHIv9kkOCMHorrQ-yiwVbBBhFbX2DTbxy3NssXrxDLvcb8U8d5raZiOdwknmE6T_9uXMUB7cZxkb58WnaPQC9meYK3qL-ASWDyxIlHlxtOHAlc767UtSX7fHKV8OHRAFyFfK0klFwd7iDxxP_m8GEppJ-Y6F5TZriELnaKr9fFxjFfY0SPjXsC0d8gSZ3Vvz8sex-0geFNd0xhOZ5CzmPqi4cABj6V-042wUW8HecfAOMe_uRT3eEw8SOOCv3n8wTJJjCPObfkRKYHc9gqqpzoRl1KtxJCphObasPLWMUfHZa1jpldFYtKa6LQgw8Qfv7QzNKv6T1NEMuHQiYY4novckw8b7y9AU/s1600/5.add-object.PNG)

  
First give a name to that object. This name should be meaningful, because we are using this name when we are programing the game. In this case we’ll name it “Bob”. Well it’s our player. Now click **ADD AN ANIMATION +** button. You will see a popup something like this.  
  

[![](/images/6.add-sprite.PNG)](https://1.bp.blogspot.com/-3I0YktQvkqw/XpydY7OVuSI/AAAAAAAALGM/RT7zo8KPRb0BDP2v_BugExaskftw9xKAwCLcBGAsYHQ/s1600/6.add-sprite.PNG)

  

  

Now click on **ADD +** button. Sprites can be animated. So you can add one or more images to sprite. And a sprite can have several animations. In here we are going to add the “Idle” animation for the sprite. In the _Choose an_ image window, navigate to downloaded assets folder. Go to _Player > Idle_ and select all the images. Click _Open_ to add all the images. Click **Loop** to enable it and rename the animation to “idle” (Optional). Now you should see something just like this;  
  

[![](/images/7.add%2Bsprite.PNG)](https://1.bp.blogspot.com/-psmHCbLwg4U/Xpydvsk49lI/AAAAAAAALGU/Txtm62q6JRcGZ-DFYXJnAA3gHTPq8CQRgCLcBGAsYHQ/s1600/7.add%2Bsprite.PNG)

  

  

Now click **APPLY** to add the object in to the scene. You can see the object we created is added to Objects Panel on the right.

### Step 4

Let’s add the player to the scene. It’s very simple. Drag and drop the object “Bob” to the canvas (gray color area in the middle. This is the canvas.) Now you will be able to see your player object in the canvas. This is how we add objects to the scene. After adding the object to the scene, you can drag it and place it in a desired location.  
  

[![](/images/8.add-object-to%2Bthe%2Bscene.png)](https://1.bp.blogspot.com/-yBe4VW0jrwU/XpyeEYbyi6I/AAAAAAAALGc/e3QuU3J7dt0JC1MhMNBz9iYNc9fxRmWIQCLcBGAsYHQ/s1600/8.add-object-to%2Bthe%2Bscene.png)

  

  

### Step 5

It’s time to create a platform for our player to land on. For that let’s add some platform objects. Click **\+** button in the object panel as you did for player object. This time we are going to select **Tiled Sprite.** This will open a popup little bit similar to sprite object. Here we can only use one image. Tiled Sprites can not be animated. First we’ll name this object. Set object name to “GrassTile” (_Note: you can’t use space when naming a game object. Only alphanumeric characters and underscores are allowed)._Now click _Select an Image_, this will reveal a drop down. Click **\+ Choose a new image** to choose an image. Select “Grass.png” inside _platform_ folder the assets pack. Set default width and height to 120px. Finally click apply to add the object to the project.  
  

[![](/images/9.add-tiled-image.PNG)](https://1.bp.blogspot.com/-sT8AFGuvCrM/Xpye0F4eF_I/AAAAAAAALGk/4h-QfJQFn3kRCeqWmDW7aPqg2tRQdAI_wCLcBGAsYHQ/s1600/9.add-tiled-image.PNG)

  

### Step 6

Now let’s create a platform for our player to land on. Drag and drop “GrassTile” object to the canvas. You can see there are three squares and a little circle appeared around the object when it is selected. Those are the handles you can use to resize and rotate the objects. Right square is used to scale horizontally while bottom square is used to scale vertically. Square in the bottom right corner is used to scale both horizontally and vertically. Circle is use to rotate the object.

Here we are going to resize the object horizontally. So hold the right handle and drag to resize the object. You can see when you resize the object, it creates tiles. If you did everything correctly, you will have a scene something similar to this;  
  

[![](/images/9.1-game-development.png)](https://1.bp.blogspot.com/-_nhDIqBJ0uw/XpyfreRKYKI/AAAAAAAALG0/U9UGT_C0SqYn8utFfwVULnY0np9X5r2LwCLcBGAsYHQ/s1600/9.1-game-development.png)

  

  

Now we have created a very basic scene. So, let’s save our changes. You can use standard keyboard short cut to save the project (Ctrl+S) or got to _File > Save._

In the [next lesson](https://www.buddhilive.com/2020/04/lets-add-behaviors-to-game-objects.html) we are going to add behavior to these objects and give some life to those objects.
