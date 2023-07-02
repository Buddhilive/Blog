---
title: "Flipping Objects in GDevelop"
description: "...."
pubDate: "2020-04-22"
categories: 
  - "archived"
---

[![](/images/9.1-game-development.png)](https://1.bp.blogspot.com/-_nhDIqBJ0uw/XpyfreRKYKI/AAAAAAAALG4/zVJsZTXNJCUbEI_JNc6lytv_qgPzL0cbQCPcBGAYYCw/s1600/9.1-game-development.png)

  
  

In our [previous lesson](https://www.buddhilive.com/2020/04/adding-animations-players-gdevelop.html), we learned how to change the animation of our character “Bob”. We came across a small issue. When we move the player backwards, it doesn’t turn back. In this lesson, we are going to fix that. Well, you may think that we should add a separate animation for that. Nope. We don’t need. We can flip the object horizontally. So the same animation can be used. To do this, we need to update our events.

### Step 1

Go to event editor of scene “Level 1”. Select “Bob is Moving” sub task (figure 1) and add two sub tasks under it. Now do to add condition in the first sub event. Find and select **Key pressed** condition. Select **Left** (i.e. Left arrow key) as the “Key” from the dropdown. And click **OK** to add the condition.

  

<table align="center" cellpadding="0" cellspacing="0" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-6K5JqHdnPQE/Xp_mMKgrJWI/AAAAAAAALKo/Tm7bGi5LB34CkEveIzS4lrA5xkKG0WG-QCLcBGAsYHQ/s1600/26.select-subtask.PNG" style="margin-left: auto; margin-right: auto;"><img border="0" data-original-height="91" data-original-width="865" src="images/26.select-subtask.PNG" style="height: auto; width: 100%;"></a></td></tr><tr><td style="text-align: center;">Figure 1</td></tr></tbody></table>

  

Go to add action for this condition and Find and select **Flip the object horizontally**. Select “Bob” as the “Object” in the settings. Click **Yes** for “Activate flipping” and click **OK.** Then add another condition below it. This time, select **Change the animation (by name)** and select “Bob” as the object. Enter “run” as the animation name and hit **OK.**Remove the action in “Bob is moving” sub event.  
  

[![](/images/28.+add+condition.PNG)](https://1.bp.blogspot.com/--84i_hMyODY/Xp_nAE2oR-I/AAAAAAAALK0/ol9E6lXydVsVdLkz_pOm5BUfbEoK4uayQCLcBGAsYHQ/s1600/28.+add+condition.PNG)

  
  

  

[![](/images/28.+add+condition.PNG)](https://1.bp.blogspot.com/--84i_hMyODY/Xp_nAE2oR-I/AAAAAAAALK4/cCcHG2WUeswWnRW9oE2EmyMrhMFYRBUUgCEwYBhgL/s1600/28.+add+condition.PNG)

  

What we do here is, we give instructions to our game that, when we press left key arrow, our character should flip horizontal and then it should play “run” animation. We set “Activate flipping” to “Yes” to tell the game to activate flipping horizontal effect.  
  

Next go to add action for the second sub event. Find and select **Flip the object horizontally**. Select “Bob” as the “Object” in the settings. Click **No** for “Activate flipping” and click **OK.** Then add another condition below it. This time, select **Change the animation (by name)**and select “Bob” as the object. Enter “run” as the animation name and hit **OK.** Finally, your events should look like this;

  

[![](/images/30.events.PNG)](https://1.bp.blogspot.com/--PkXHTzWkOw/Xp_n4Ax2sqI/AAAAAAAALLE/AUV2g1kEsMARD14fObAlSLCQBBHCGonugCLcBGAsYHQ/s1600/30.events.PNG)

  

Here we instruct the game to deactivate flipping effect if it is activated (if not it will remain the as it is) and play “run” animation when we press right arrow key is pressed. We set “Activate flipping” to “No” to tell the game to deactivate flipping horizontal effect if it is enabled or else no flipping effect will apply on the object.  
  

Ok, now we are ready to preview our game. Hit the **Preview** button and move the player back and forth. Now you can see all our animations for player movements work perfectly. Basically, we have created a platformer game. In the [next lesson](https://www.buddhilive.com/2020/04/moving-camera-with-player-gdevelop.html) we are going learn how to move camera with the player.  
  

Feel free to ask any question regarding this lesson in the comment section below.
