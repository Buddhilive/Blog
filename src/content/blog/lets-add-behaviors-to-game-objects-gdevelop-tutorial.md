---
title: "Let’s add behaviors to Game Objects - GDevelop Tutorial"
description: "...."
pubDate: "2020-04-19"
categories: 
  - "archived"
---

[![](/images/9.1-game-development.png)](https://1.bp.blogspot.com/-_nhDIqBJ0uw/XpyfreRKYKI/AAAAAAAALG0/U9UGT_C0SqYn8utFfwVULnY0np9X5r2LwCLcBGAsYHQ/s1600/9.1-game-development.png)

  

  

In our [previous lesson](https://www.buddhilive.com/2020/04/game-development-for-beginners-with.html) we learned how to add objects to a game scene. In this lesson we are going to add behaviors for those objects. Adding behaviors gives life to those objects. For instance, we need to add gravity, collision and player controls to make the game work. If you hit **Preview** button (image 1) will load the preview of the game as a popup. You’ll see the player is floating in the air and if you press arrow keys, player won’t respond. This isn’t how it should be.

<table align="center" cellpadding="0" cellspacing="0" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-xxiyGfQEWjs/XpyjjKxIMQI/AAAAAAAALHA/A6zbD0Yt6yIjFgEtWNOfNHcZ6y0cYwkWACLcBGAsYHQ/s1600/previe-button-gdevelop.PNG" style="margin-left: auto; margin-right: auto;"><img border="0" data-original-height="50" data-original-width="46" src="images/previe-button-gdevelop.PNG"></a></td></tr><tr><td style="text-align: center;">Image 1</td></tr></tbody></table>

Well this isn’t an easy task. It involves lots of lines of coding. But, fortunately, GDevelop have most of those features prebuilt as behaviors which saves our time.

### Step 1

In the object panel, click three dots like button (menu) next to “Bob”. From the drop down menu select **Edit Object.**

[![](/images/10.edit-object.png)](https://1.bp.blogspot.com/-i51K4JNGtyk/Xpyj8c4a72I/AAAAAAAALHI/sWPWiEnkFJAHDbI-r4wql-5762wG_DviACLcBGAsYHQ/s1600/10.edit-object.png)

  

In the popup, switch to **Behavior** tab and click **ADD A BEHAVIOR TO THE OBJECT +** button. From the behavior list select “Platformer character”. This will add some options to our player object’s behavior. You can change those values as you like. For now, we’ll keep those settings as it is. Click **APPLY** to add the behavior to the object.

  

[![](/images/11.behavior-list.PNG)](https://1.bp.blogspot.com/-eA3BVuwUQ5o/XpykCLnKGiI/AAAAAAAALHM/HDdc6xYZa9AZ99fVW41rhLDy_boEuMW_QCLcBGAsYHQ/s1600/11.behavior-list.PNG)

  

  

Now if you hit the **Preview** button, the player will fall off the screen. Actually it should land on the platform we created. Instead the player falls through the platform. Let’s fix this.

### Step 2

This time we need to add behavior “GrassTile” object. Go to edit object in “GrassTile” as we did in “Bob” object. Switch to behavior tab and click **ADD A BEHAVIOR TO THE OBJECT +** button. Here we are going to select “Platform” behavior. This will also add some settings to “GrassTile” behavior. At the moment we’ll keep those settings as it is and click **APPLY**to add the behavior to “GrassTile”.

  

Now hit **Preview** button to preview the changes. Bingo! Our player landed on the platform. Now use standard platformer game controls on your keyboard to move your player; Use left and right arrow keys to move the player back and forth. Use Shift or Space to jump.  
  

[![](/images/12.preview-project.png)](https://1.bp.blogspot.com/-PU4MooXjdoM/XpykXKR_PnI/AAAAAAAALHc/yMyiwQSs07weY0sQU51XZDH389JO3YnNgCLcBGAsYHQ/s1600/12.preview-project.png)

  

Congratulations! You just step in to game development. You may notice that when you move the player, it doesn’t change to walking animation. Well, we are going to learn it in the [next lesson.](https://www.buddhilive.com/2020/04/adding-animations-players-gdevelop.html)
