---
title: "Adding Animations Players – GDevelop"
description: "...."
pubDate: "2020-04-20"
categories: 
  - "archived"
---

[![](/images/14.+add-animation.PNG)](https://1.bp.blogspot.com/-pcOOX_4nRAU/Xp4DFto3MbI/AAAAAAAALIc/75HpCP3gF68u2QV-02aU1H8DthWfvXVeACLcBGAsYHQ/s1600/14.+add-animation.PNG)

  
  

In our [previous lesson](https://www.buddhilive.com/2020/04/lets-add-behaviors-to-game-objects.html) we add behaviors to objects. If remember, we found that our player character doesn’t animate when moving and jumping. In this lesson, we are going to fix that. We already have added one animation to our character. That is the “idle” animation. So let’s add other animations.

### Step 1

Now we are going to add “run” animation. Go to _Edit Object_ in “Bob” (you know how to if you followed the previous lesson). Click **ADD AN ANIMATION +**. This will add an empty animation to your character. Rename this animation to “run”. Click **ADD +** button. Now navigate to assets folder and go to _player > run_ and select all the images, then click ok to add images to animation. 

### Step 2

Click **ADD AN ANIMATION +** button again. Rename this animation to “jump”. Click **ADD+** button and add image _“1.png”_ from _player > jump_ folder. Click **ADD AN ANIMATION +** button again. Rename this animation to “fall”. This time select _“2.png”_ from _player > jump_ folder. If you follow the instructions correctly, your character properties should look like this;

  

[![](/images/15.+add+animation.PNG)](https://1.bp.blogspot.com/-CPKhIBesphY/Xp4EUQ32jAI/AAAAAAAALIw/peIeVsUVKf0giLqWwNuofDYpT-99rKZGwCLcBGAsYHQ/s1600/15.+add+animation.PNG)

  

  

If everything is done, click **APPLY** to save the changes you’ve made. If you hit the **Preview** button and see, still nothing changed. Well, this is because we need to program which animation to play when we control the player. This is where we need Events. So it’s time to create our first event!

### Step 3

Switch to “Level 1” scene’s event editor. You’ll see nothing at the moment. Since we haven’t created any event so far. This is where we add our game logic. You don’t need any coding knowledge to create events. It’s pretty simple visual editor anyone can learn within short period of time. But if you have a basic knowledge in programing concepts, that would be great. Anyways, it not compulsory to know coding.  
  

<table align="center" cellpadding="0" cellspacing="0" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-_t55a2iXed8/Xp4ElV17zSI/AAAAAAAALI4/Tl7DRMy4e_csHjd2nbmAL38tig4tTHt_wCLcBGAsYHQ/s1600/16.+add-new-event.PNG" style="margin-left: auto; margin-right: auto;"><img border="0" data-original-height="49" data-original-width="42" src="images/16.+add-new-event.PNG"></a></td></tr><tr><td style="text-align: center;">Figure 1 - Add anew empty event</td></tr></tbody></table>

  

<table align="center" cellpadding="0" cellspacing="0" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-B_ZD_2uxLeI/Xp4E4ogYYjI/AAAAAAAALJA/94rvlgDLTikrAGikNcDhQ6jaFpyfhuRGwCLcBGAsYHQ/s1600/17.empty-event.PNG"><img border="0" data-original-height="77" data-original-width="1354" src="images/17.empty-event.PNG" style="height: auto; width: 100%;"></a></td></tr><tr><td style="text-align: center;">Figure 2 - Empty Event</td></tr></tbody></table>

Click **Add a new empty event** button (Figure 1) from the top tool bar. This will ad an empty event (figure 2). Event has two sides. One is to define our condition and the other side to define the action. Click **Add condition**. This will open a popup which displays all available conditions in GDevelop.  
  

[![](/images/18.add-conditions.PNG)](https://1.bp.blogspot.com/-OyIeY7aiy_o/Xp4FP8_MBaI/AAAAAAAALJI/NTnbw9Z4Y14nPzZcQXwOWiCrPdlitr1BwCLcBGAsYHQ/s1600/18.add-conditions.PNG)

  

  

From the list of conditions in the left side, select **Is jumping**under _Platform BehaviorI_ or just simply type “is jumping” in search bar to find and select the condition. On the right side, all settings related to the condition we selected will appear. For “Is jumping” we need to configure which object’s movement we need to track. Select “Bob” from the dropdown. If you did correctly, your condition will look something just like this;  
  

[![](/images/24.+jumping.PNG)](https://1.bp.blogspot.com/-0xyN4ru6jNg/Xp4GjHsiglI/AAAAAAAALJg/8Uo2VPpLOY0uo_wvRv1aQc8DcIVuOy7HwCEwYBhgLKs0DAL1OcqyUtlQ6ylpqUj41JEZQfdo9MTDOkqTk7HW_J1VI5XmfPCHl8QhdPAO779Aa2hP1-tgIZs8KqNmU7wUZ5ebmBus2d7NUfgIyjSnioBuivVl149PZH_ji6nsV0HpI7zgNWISGKNI3j_O_LZ6GQzqjy0tLsIVgNtrA5X1X-EyPUBvw1nWo5_oSy5S7CzjHJCW3oVZB2QpSr2waSoqBzlvTPZUxED0-e2POJWO_h_BRO9U6XbUFHAY9rUER-RdyC65P3sdy1pbE77i3GlQRosYuhKapxHWbJEaF5gTyANb6KZoGdZZqfUZ4dUEtyobaPN6Pn_0fSEuJNkb0N0J31mLSbi8ExVIe13-2Wbf7Xv1XbBoTuEBCdihzp8ITRRG-xhlYSjZrDW6PgI3hrfbLX7awvdjAb9LMos3uH-K9K-nP7CBtZ2UnitWrg0YlXweLbypDFVUDKTMd9xTWakMTfWrUH0wnCAefj3G335vYWOCQpPL-1T3pXVh2kb8MA6hI_ELDMWhi9cwOdValI6VQ79Qkuql4MFW4_woG2VZSFLhLnnssXASIv063WUj9Q4Ielq0fjuz9tQk2taDJGGZ5QaGOnns4kszTZYHi2kEwhZL49AU/s1600/24.+jumping.PNG)

  

If everything is fine, click **OK** to add the condition to our event. Now click **Add action.** This will open a popup similar to condition popup. This popup contains all the available actions in GDevelop.

  

Now find **Sprite** category and open **Animations and images** sub category. Select **Change the animation (by name).** Similar to condition settings, you’ll be able to see relevant settings for the action you’ve selected. Choose “Bob” from the dropdown as the _Object._ Under _Animation name,_ enter the animation name we need to play. In this case it’s “jump”. Remember, you should define the animation name within quotes. We define strings within quotes. If you have a programing knowledge you must be familiar with the way we use string variables. If you configure the settings correctly, your action should look something just like this;

  

[![](/images/25.+jump-animation.PNG)](https://1.bp.blogspot.com/-_INq91gdUks/Xp4HDw-i_BI/AAAAAAAALJo/zTjgTMgdINQn4mc8ODbOd4wMNZekOrqmwCLcBGAsYHQ/s1600/25.+jump-animation.PNG)

  

If everything is ok, hit the **OK** button to save the action we created. Hooray! We just created our first Event! Well there are few more conditions to add before we wind up this lesson. Now follow the same steps to add the second animation.  
  

Our second event is as follows; Click **Add condition.**Find and select **Is falling** and select “Bob” as the object, then click **OK.**Now click **Add action.** Find and select **Change the animation (by name)**and select “Bob” as the object. Enter “fall” as the animation name and hit **OK.** Now we have successfully added our second event.  
  

<table align="center" cellpadding="0" cellspacing="0" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-cxYlcpn3jng/Xp4Ha6ZSrdI/AAAAAAAALJw/HieSRasmk-EI44DdRV6UR1FTVNV18ouTgCLcBGAsYHQ/s1600/23.sub-event-button.PNG" style="margin-left: auto; margin-right: auto;"><img border="0" data-original-height="41" data-original-width="39" src="images/23.sub-event-button.PNG"></a></td></tr><tr><td style="text-align: center;">Figure 3 - Add anew sub event button</td></tr></tbody></table>

Well, now we have already created three simple events. Our next event is little bit different. In previous events, we had only one condition. But we are not going to add sub-events. Click **Add a sub event** button (figure 3). Make sure you have selected the main event that you want to add the sub event. You can also right click on the event you want to add sub event and select “Add sub event”. We need two sub events.  
  

Click **Add condition** in main event**.** Find and select **Is on floor** and select “Bob” as the object, then click **OK.**Keep the actions empty for the main event.  
  

Go to first sub event and click **Add condition**. Find and select **Is moving** and select “Bob” as the object, then click **OK.**Now click **Add action.** Find and select **Change the animation (by name)**and select “Bob” as the object. Enter “run” as the animation name and hit **OK.**  

Go to second sub event and **Add condition**. Find and select **Is moving** and select “Bob” as the object. This time we are enabling **Invert condition** option in the settings. Click **OK** to save changes. Now click **Add action.** Find and select **Change the animation (by name)** and select “Bob” as the object. Enter “idle” as the animation name and hit **OK.**  

If you follow the instructions correctly, your events should look something similar to this;

  

[![](/images/22.all-conditions.PNG)](https://1.bp.blogspot.com/-lSzS-EAHREQ/Xp4HpxwO7uI/AAAAAAAALJ0/GkHbQ34XJAEKQUONQN_wrsVaKFxUFZTKQCLcBGAsYHQ/s1600/22.all-conditions.PNG)

  

If everything is ok, save your project. Now click **Preview**button to preview the changes we made. Now try to move and jump Bob. Well now Bob is animated for running, jumping and falling. But, still there’s a problem. Moving forward works fine. But when you try to move the player backward, it doesn’t turn around. How to fix this? That we’ll discuss in the [next lesson.](https://www.buddhilive.com/2020/04/flipping-objects-in-gdevelop.html)  
  

If you have any questions or doubts, please feel free to comment below.
