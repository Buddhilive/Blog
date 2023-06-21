---
title: "How to Create a Chatbot using TensorFlow"
description: "...."
pubDate: "2018-12-02"
categories: 
  - "chatbot"
  - "tensorflow"
---

[![create a chatbot](/images/cover-photo.jpg)](https://2.bp.blogspot.com/-w7pKzAxhzB8/XAQA5M1ucDI/AAAAAAAAIFA/ocC1cavnTUk2vhlJshX-TFkOiRsSBI8HACLcBGAs/s1600/cover-photo.jpg)

> Try [Berkelium](https://berkelium.dev), a NodeJS Chatbot library build using TensorflowJS.
> 
> Note: this tutorial is quite outdated. So I recommend to use Berkelium Library.

Chatbots have been very famous these days. With the evolution of Machine Learning and Deep Learning Technologies, Chatbots have gain a significant popularity in the industry. Many companies are trying to build Chatbots for their businesses.

There are lots of Chatbot frameworks in the internet. Some are free and some are paid. Different frameworks has different capabilities. And there are some opensource frameworks as well. Those opensource frameworks allows developers to create Chatbots from the scrach.

Among many Machine Learning and Deep Learning frameworks, TensorFlow has become very popular and powerful. Building a Chatbot using TensorFlow is easy. "Buddhilive Chatbot" is a OpenSource Chatbot Project build using TensorFlow.

As you know, to train a model in TensorFlow, you need lot of computation power and there are set of libraries and dependencies you have to install to run TensorFlow in your local computer. But thanks to Google, we can use Google Colabs to train our TensorFlow models. Not only that, Google offers free GPUs to use up-to 12 hours a day. This allows us to train a model without a hazel. (_Note: Colabs is designed for training models with small datasets. Do not use it to train large amount of data.)_

Google Colabs is same as a Jupyter notebook. So if you are familiar with Jupyter notebooks, Google Colabs would be easy to adapt.

Let see how you can create your own custom Chatbot. Follow these steps;

1. Go to [Google Colabs](https://colab.research.google.com/).
2. Click on **File > Open notebook**
3. Go to GitHub Tab and Past this link: [https://github.com/Buddhilive/Buddhilive/blob/master/buddhilive\_train.ipynb](https://github.com/Buddhilive/Buddhilive/blob/master/buddhilive_train.ipynb)
4. Press Enter
5. Select **"buddhilive\_train.ipynb".** A Jupyter notebook will be opened.
6. Go to **File > Save a copy in Drive** to save it to your Google Drive

A new notebook will be opened on Colabs form Google Drive. All changes you make here will be saved in this notebook. Now go to **Runtime > Change runtime type** and choose **GPU** under "Hardware Accelerator".

Then go to **Runtime > Run all** (or Ctrl+F9). Now the training starts. (_Note: Read the notes in the notebook to get more information_)

When the training is finished;

1. click on **File > Open notebook** again.
2. Go to GitHub Tab and Past this link: [https://github.com/Buddhilive/Buddhilive/blob/master/Buddhilive\_Response.ipynb](https://github.com/Buddhilive/Buddhilive/blob/master/Buddhilive_Response.ipynb)
3. Press Enter
4. Select **"buddhilive\_train.ipynb".** A Jupyter notebook will be opened.
5. Go to **File > Save a copy in Drive** to save it to your Google Drive

A new notebook will be opened on Colabs form Google Drive as earlier. Here we are going to test the trained model we have created. You can see some sample queries at the end of the notebook to test the trained model.

As earlier, go to **Runtime > Run all** (or Ctrl+F9) to test the model.

(Fork the project on GitHub: [https://github.com/Buddhilive/Buddhilive](https://github.com/Buddhilive/Buddhilive))

### Next Step

- [How to Customize Cahtbot using Custom Intents](https://www.buddhilive.com/2018/12/how-to-customize-chatbot-using-custom.html)

[![](/images/google_colab.PNG)](https://3.bp.blogspot.com/-SaX9q_BzaEE/XAgBrNRn0iI/AAAAAAAAIFo/3-3Cb14PeFoperWc6Ifz-tXdKne0o5WVwCLcBGAs/s1600/google_colab.PNG)

This project was launched based on [this GitHub project.](https://github.com/ferrygun/FlowerBot)
