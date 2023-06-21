---
title: "How to Customize Chatbot using Custom Intents"
description: "...."
pubDate: "2018-12-05"
categories: 
  - "chatbot"
  - "tensorflow"
---

[![](/images/tensorflow_chatbot_project.jpg)](https://3.bp.blogspot.com/-9dNVsi35UPE/XAf5a--fzbI/AAAAAAAAIFU/uQeLdxhn17szZ0hLF_yUjnr8kXfb_Jh3QCLcBGAs/s1600/tensorflow_chatbot_project.jpg)

> Use [Berkelium](https://berkelium.dev) NodeJS Chatbot library build using TensorflowJS.
> 
> Note: this tutorial is quite outdated. So I recommend to use Berkelium Library.

_(This article is related with [How to Create a Chatbot using TensorFlow](https://www.buddhilive.com/2018/12/buddhilive.html))_

_Now let's see how we can customize and improve our Chatbot. First go to the [Buddhilive Chatbot GitHub Repository](https://github.com/Buddhilive/Buddhilive-Chatbot). Then fork your own copy of the project to your GitHub account. Now go to that forked repository. Navigate in to **Datasets** folder and open **train\_intent.json** file. This file may look something like this;_

This is the dataset we are using to train our chatbot. You can clearly identify the JSON data structure we are using here;

- **tag:** "Tag" refers to the name of the particular intent.
- **patterns:** "Patterns" refers to some frequently used user queries and input patterns that are related to a specific intent. You can add several _patterns_ seperating with commas.
- **responses:** "Responses" refers to the responses that matches for a certain input. You can add several different _responses_ that can be given for the same query by separating them with commas.

Using the same data structure you can edit and add more intents to this file. When you train the chatbot with more intents, it will become more versatile.

You can clone your own copy of this repository on your local machine and edit **train\_intent.json** file and commit the changes to your repository.

When you are about to train the chatbot with your customized data, make sure to do the following;

[![](/images/tensorflow_chatbot_google_colabs.PNG)](https://4.bp.blogspot.com/-aH-FMBAhKtw/XAgBUFk3IcI/AAAAAAAAIFg/3AxXxISLbZwb8nwdgPc96y5bj-8t0kuuQCLcBGAs/s1600/tensorflow_chatbot_google_colabs.PNG)

1. Go to [Google Colabs](https://colab.research.google.com/)
2. Open the copy of **Buddhilive\_train.ipynb** file that you have saved to your Google Drive.
3. Go to the second Code Cell in the notebook where we import dataset from GitHub and change the URL with the URL to your own copy of Buddhilive Chatbot's repository.
4. Do the same to the copy of **Buddhilive\_Response.ipynb** file you have saved to your Google Drive

Now the chatbot will be trained with your new customized intents. Test the chatbot in **Buddhilive\_Response.ipynb**
