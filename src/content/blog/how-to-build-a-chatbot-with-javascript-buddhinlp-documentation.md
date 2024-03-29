---
title: "How to Build a Chatbot using JavaScript"
description: "BuddhiNLP is a Open Source NodeJS library for building chatbots."
pubDate: "2021-01-05"
categories: 
  - "machine-learning"
  - "tensorflow"
heroImage: "/images/buddhi-nlp-cover.jpg"
---

> Note: This package is deprecated. Please switch to **berkelium** instead. Documentation available at [https://berkelium.dev](https://berkelium.dev)
> 
> [View migration announcement](https://www.buddhilive.com/2022/05/launching-berkeliumlabs-opensource-machine-learning-projects.html)

BuddhiNLP is a Open Source NodeJS library for building chatbots. BuddhiNLP is developed using [TensorflowJS](https://www.tensorflow.org/js/), a popular machine learning library developed by Google Engineers.

## Install BuddhiNLP

Install BuddhiNLP using _npm._

```

npm i buddhi-nlp
```

### Import to the project

```
const buddhi = require('buddhi-nlp')

//or

import buddhi from 'buddhi-nlp'
```

## Train the Model

Training a chat model using BuddhiNLP is very easy and straight forward. We use JSON file format to input data for training the model. The JSON file structure is as follows;

```

{
    "intents": [{
            "tag": "greeting",
            "patterns": ["Hi", "How are you", "Is anyone there?", "Hello", "Good day"],
            "responses": ["Hello, How are you?", "Good to see you", "Hi there, how can I help?"]
        },
        {
            "tag": "goodbye",
            "patterns": ["Bye", "See you later", "Goodbye"],
            "responses": ["See you later!", "Have a nice day", "Bye!"]
        },
        {
            "tag": "thanks",
            "patterns": ["Thanks", "Thank you", "That's helpful"],
            "responses": ["Your welcome!", "Any time!", "My pleasure"]
        },
        {
            "tag": "fallback",
            "patterns": [""],
            "responses": ["Sorry, please say that again", "Please give me more info", "I still can't understand that."]
        }
    ]
}
```

This is the format of JSON file that we use as the training data for the chatbot.

**tag:** _(string)_ This is the intent name. Use lowercase alpha-numeric characters and underscore. Do not use any other symbols or capital letters.

**patterns:** (_Array<string>_) This is where we defined user utterances. Patterns of speech for the intent. This is a string array. You can define many patterns as you like. More the patterns are better the accuracy is.

**responses:** (Array<string>) Here we define the responses for the intent. This is also a string array. You can define variety of responses. Try to define variety of responses, so the chatbot won't keep repeating the same response.

Now to train the model use the following code:

```

buddhi.train('path/to/file.json', output_dir);
```

### Parameters

**datafile:** Path to training data file.

**output\_dir:** Path to out put folder where the model will be saved. Use _[\_\_dirname](https://nodejs.org/api/modules.html#modules_dirname)_ to save the model to the current directory of your project. Model files will be saved to this directory.

## Use Trained Model

Once you have trained your model you can implement it using following code;

### Initialize Model

```
const dataUrl = 'path/to/model_metadata.json';
const modelUrl = 'https://yourdomain.com/model/model.json';
buddhi.loadModel(modelUrl, dataUrl, callbackFunction);

function callbackFunction() {
console.log("model loaded!");
}
```

**modelUrl:** This is the URL where your trained model is located. You need to provided an **[Absolute URL](https://www.9thwonder.com/blog/the-difference-between-absolute-and-relative-urls-in-website-development)** here. **dataUrl:** This is the URL where _model\_metadata.json_ file is located. You need to provide a **[Relative URL](https://www.9thwonder.com/blog/the-difference-between-absolute-and-relative-urls-in-website-development)** here. **callbackFunction:** Provide a callback function to be executed when the model is loaded. This is where you can start your chatbot work.

### Classify Sentences

```
const sentence = 'What is your name?';
let answer = buddhi.classify(sentence);

console.log(answer);
```

Inputs **sentence:** (_String_) Basically this is the user utterance/input.

Outputs **answer:** (_Array<any>_) Returns an array of 3 elements

1. _answer\[0\]: Bot response as String_
2. _answer\[1\]: Name of Intent as String_
3. _answer\[2\]: Confidence or the accuracy as float_
