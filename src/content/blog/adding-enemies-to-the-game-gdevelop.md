---
title: "Adding Enemies to the Game – GDevelop"
description: "...."
pubDate: "2020-05-03"
categories: 
  - "archived"
---

  

[![](/images/00_GDevelop_Tutorial_for_beginners.PNG)](https://1.bp.blogspot.com/-ooaAnBJVIVI/XpyZp6wIMkI/AAAAAAAALFU/W0VAzxGoDhUpYFr_B7oKG-MB85uJSOmIwCPcBGAYYCw/s1600/00_GDevelop_Tutorial_for_beginners.PNG)

  

In our previous lesson we learned how to add collectable items and a score system. In this lesson we are going to add enemies to the game. There’s no fun without evil monster in the game, right?  
  

First, add a Sprite Object and rename it to “Monster”. Select _enemy.png_ from _assets > enemy_ folder as the sprite image. Drag and drop the monster to the canvas. Resize the monster sprite as you like.

### Moving the Enemy

Here we are going to move the enemy left and right. For that we need two trigger objects. Add another two sprite objects. For the first, name it “RightTrigger” and add _Right.png_from _assets > enemy_ folder and name the second object, name it “LeftTrigger” and add _Left.png_ as the sprite image. Now place those two objects as shown in the image below;

  

[![](/images/53.enemy.PNG)](https://1.bp.blogspot.com/-O87tR93D0Kk/Xq8Igne4XRI/AAAAAAAALV4/Rzms2M5PJ1kROcwAPE668YaMRL1R4ukjwCLcBGAsYHQ/s1600/53.enemy.PNG)

  

What we are going to do here is, when the enemy collide with “RightTrigger” it will move towards left and when it hits with “LeftTrigger” it will move towards right, thus enemy will move to left and right between the trigger objects. We need a Object Variable here. Right click the “Monster” object in the Objects panel and select **Edit object variables** from the menu. An empty popup window will appear. Add a variable (in the similar way we add scene variable in the previous lesson) named “direction” and set its default value to “left”. Click **APPLY.**  
  

[![](/images/54.variable.PNG)](https://1.bp.blogspot.com/-ni_VzazYw3A/Xq8JE_MvUvI/AAAAAAAALWA/W0x27lzvDh4SFrG34Zzs7L8cuUs9Ne55ACLcBGAsYHQ/s1600/54.variable.PNG)

Switch to Events Editor and add a new empty event. Well, I thought to show how this happens using a video. I think it will be more understandable if you can see how these events are build. I will explain what happens after the video;  
  

<iframe allowfullscreen data-thumbnail-src="https://i.ytimg.com/vi/5VZpJuuVWcg/0.jpg" frameborder="0" height="360" src="https://www.youtube.com/embed/5VZpJuuVWcg?feature=player_embedded" width="100%"></iframe>

  

  

Now what I did here is, from the first two events, if the monster hits the “RightTrigger” the _direction_ variable value changes to “right” and if monster hits “LeftTrigger” the _direction_variable value changes to “left”. And in the other two events, if the _direction_ variable is “left” it adds a force to the object in the direction of 180 degrees (i.e. left) or if the _direction_ variable is “right” it adds a force to the object in the direction of 0 degrees (i.e. right). You saw the preview worked fine. But there was a problem. We don’t need to see the triggers. So, we need to hide them. To do that, I add a new event which execute at the beginning of the game to hide the trigger objects.

### Kill the Enemy

For this, we need to create a similar event as we did for the coins. When the player collides with the enemy, the enemy should be deleted. But that should happen only if the player jumps on to the enemy. To trigger that, we need to add another condition to check whether the player is falling. When the player jumps on to the enemy, the player should bounce back too. For that, we need to simulate the Jump action of the player. And finally, we are adding points to the score for killing the enemy. The following video shows you how to build the event that adds the functionality I mentioned before.

  

<iframe allowfullscreen data-thumbnail-src="https://i.ytimg.com/vi/WnDfXYrE8Kc/0.jpg" frameborder="0" height="360" src="https://www.youtube.com/embed/WnDfXYrE8Kc?feature=player_embedded" width="100%"></iframe>

  

### Player gets killed by the Enemy

This is also somewhat like killing enemy. When enemy collides with the player, the player dies. But this happens only if the player is on the floor. When the player dies, game over. (We’ll discuss how to add a Game Over screen in the future). However, the proper way is to have a Life counter or a HP (Health Points) counter. So once the enemy collides with the player, the player gets hurt. You can do that too. But we’ll discuss about that in a future lesson. (if you can figure out how to do it. Just give it a shot). Ok, the event for killing the player by the enemy is as follows;

  

[![](/images/55.event.PNG)](https://1.bp.blogspot.com/-OEeCLHGWNWE/Xq8JVtGO4QI/AAAAAAAALWI/Alln-7KYFPwJ6rgpqpEgqMMdTM-4KqO5ACLcBGAsYHQ/s1600/55.event.PNG)

  

Ok, now we know how to add enemies or monsters to the game. If you have any doubts, you are always welcome to comment below. I’m happy to help.

  

For more tutorials, visit [http://wiki.compilgames.net/doku.php](http://wiki.compilgames.net/doku.php)
