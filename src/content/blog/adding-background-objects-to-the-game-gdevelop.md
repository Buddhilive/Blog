---
title: "Adding Background Objects to the Game – GDevelop"
description: "...."
pubDate: "2020-05-03"
categories: 
  - "archived"
---

[![](/images/00_GDevelop_Tutorial_for_beginners.PNG)](https://1.bp.blogspot.com/-ooaAnBJVIVI/XpyZp6wIMkI/AAAAAAAALFU/W0VAzxGoDhUpYFr_B7oKG-MB85uJSOmIwCPcBGAYYCw/s1600/00_GDevelop_Tutorial_for_beginners.PNG)

  
In our previous lesson we learned how to add a jump through platform. In this lesson we are going to learn how to add background objects to our game and, we are going to extend the platform for our player to run.  

### Step 1

Well adding background Objects are simple. All you have to do is add some sprite objects. We are going to add four background objects. Add Sprite Objects of Tree, Bush, Flower and Cloud. All these images can be found in our assets folder. (_assets folder > Background_).  
  

[![](/images/36.background.PNG)](https://1.bp.blogspot.com/-2zv0sPRk698/Xq7vqlqBdOI/AAAAAAAALTs/mM24g5g35YAFquFoiUZq3v-xZaZn14ZGQCEwYBhgL/s1600/36.background.PNG)

  

Once you have added these objects, you can drag and place these objects in the canvas as you wish. When you are placing these objects, you may notice that the player goes behind these objects.

  

[![](/images/37.background.PNG)](https://1.bp.blogspot.com/-vlWqKU4Scfc/Xq7v3nKPx1I/AAAAAAAALTw/6eyxwnvGty06NI7z4HQW9IVXHTXQq0hvQCLcBGAsYHQ/s1600/37.background.PNG)

  

This can be fixed by adjusting the **Z-Order** of the object. To change the **Z-Order** of the object, you have to select the object, then you can see some settings in the **Properties**panel in the left-hand side. This **Properties** panel shows properties of a selected object like width, height, position etc. Now change the Z Order of those background objects to something like “-2”. Yes, you can insert negative values too. This will arrange the background objects behind our player.  
  

[![](/images/38.background.PNG)](https://1.bp.blogspot.com/-jhc7VJqaA-w/Xq7weOpAMgI/AAAAAAAALUA/9pNa8V_2Dlocm0GaeyMsgE0SusV73RjpgCLcBGAsYHQ/s1600/38.background.PNG)

  

To understand this let’s take a simple example. Think we have two object **A** and **B. A** has Z order set to 3 and B has Z order set to 4. So, **B** will appear on top of **A.** If you need to bring **A** on top of **B**, then either you have to increase the Z Order of **A** to 5 or above, or else you need to decrease Z order of **B** to something below 3. 
  

[![](/images/39.background.PNG)](https://1.bp.blogspot.com/-Qovkp-Lv_ZA/Xq7wk52sCgI/AAAAAAAALUE/uV-w_dDfxAEccc0K85yugzrrVhfka9WagCLcBGAsYHQ/s1600/39.background.PNG)

  

### Step 2

<table align="center" cellpadding="0" cellspacing="0" style="margin-left: auto; margin-right: auto; text-align: center;"><tbody><tr><td style="text-align: center;"><a href="https://1.bp.blogspot.com/-NIYxOYdx1J4/Xq7w_gM6bGI/AAAAAAAALUY/fInTAxZeLVwj-i1O1txjYFYj_mF7uURBgCLcBGAsYHQ/s1600/40.layers.PNG" style="margin-left: auto; margin-right: auto;"><img border="0" data-original-height="50" data-original-width="43" src="images/40.layers.PNG"></a></td></tr><tr><td style="text-align: center;">Figure 1 - Open the layers editor</td></tr></tbody></table>

Ok, now we have some background objects placed, let’s change the background color. For that, click **Open the layers editor** button (Figure 1) on the top tool bar. This will open the **Layers Editor** popup window. There, click the gray color button next to **Background color**. This will open a color picker. Select a color that is similar to sky blue. Now close the **Layers** editor. You can see the background color has changed now.  

  

[![](/images/41.background-color.png)](https://1.bp.blogspot.com/-Hil025j9pWY/Xq7w5BLCv7I/AAAAAAAALUQ/EM6OoAgioEIWcy4p-Ps6pTfIHyPdnPtewCLcBGAsYHQ/s1600/41.background-color.png)

  

Now we are going to extend the platform, so our player will have some space to run. This is I’m not going to explain much. The things you have learned so far is enough to do this. I’m going to show how I did this using a video. You don’t need to do exactly what I did. Just let your inner creativity to take over this situation. And with this video, I’m going to close this lesson. After watching the video and completing your platform design, move on to the [next lesson.](https://www.buddhilive.com/2020/05/adding-coins-and-score-system-gdevelop.html)  
  

And feel free to ask your question down below in the comment section.  
  

_Note: To clone/copy an object press and hold Ctrl while dragging the object. To Zoom the canvas, use the mouse wheel._  
  

<iframe allowfullscreen data-thumbnail-src="https://i.ytimg.com/vi/Y6RSwyYGAWI/0.jpg" frameborder="0" height="360" src="https://www.youtube.com/embed/Y6RSwyYGAWI?feature=player_embedded" width="100%"></iframe>
