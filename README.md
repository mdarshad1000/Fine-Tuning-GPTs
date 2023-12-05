# Fine-Tuning-GPTs

Project Created By - Ali Quidwai and Nagharjun 

## Introduction
Not every organization will have the resources or capability to build a large language model from scratch due to the extensive dataset and computational requirements involved in the process

We believe that Model as a Service will become the standard in the industry, and that the most effective way to improve already trained large language models (LLMs) with over 100 billion parameters will be through fine-tuning

In this context, we propose an optimized method for fine-tuning Large LLM with a high accuracy rate on a limited amount of training data, which is known as few-shot learning


This is a project using transfer learning to fine tune GPT3 Language Model. With low amount of data, we are efficiently fine tuning the model based on a specific task. We also explore a cost effective way for training. 

## Workflow
We implement transfer learning strategy for fine tuning a GPT-3 model to work on script generation for a language model.

To optimize the performance of the model, we have experimented with different values for epochs, batch size, and learning rate during the fine-tuning process. By altering these parameters, we were able to determine which combination yields the best results.

We were able to successfully train the model with only a small amount of training and validation data.

We propose a strategy to lower the cost of GPT-3 while maintaining its high quality.

## Architecture

![hpml drawio (1)](https://user-images.githubusercontent.com/64778259/208584100-9d38a668-04b2-4793-b2e5-d3425a854533.png)

## Code Walkthrough

1) The `code.ipynb` file can run locally through Jupyter Notebook or Google Colab.
2) Requirements: 

   `pip install openai`
   
   `pip install wandb`
   
3) A wandb account is required to run this code. Creating a wandb account is free and the API Key of the wandb account is required to publish the graphs and visualizations into it.
4) While running the `Preparing the data to be fed into the GPT-3 model for fine tuning. The CSV file is converted to a JSON file format suitable to fine tune OpenAI's GPT model.` cell, pass `Y` to all requests

   <img width="1408" alt="image" src="https://user-images.githubusercontent.com/64778259/208596331-b96d823d-eebc-4a95-b453-2894bccf20d8.png">
   
5) While running the `Training the model` cell, pass empty strings to everything.

   <img width="1134" alt="image" src="https://user-images.githubusercontent.com/64778259/208596662-733ba91c-288d-42df-af56-530b1f79708c.png">

## Results

![bar-graph (7)](https://user-images.githubusercontent.com/64778259/208597297-55f95c27-d830-470b-b30c-9ea3534baf4f.png)
![bar-graph (6)](https://user-images.githubusercontent.com/64778259/208597299-9eabaf43-ee55-43cd-9829-da801c303d57.png)

![bar-graph (5)](https://user-images.githubusercontent.com/64778259/208597301-2054e1c9-3a55-46cb-8cc4-355c32a8161a.png)
![bar-graph (4)](https://user-images.githubusercontent.com/64778259/208597302-407d675e-5c4b-4c83-b4fa-e0a7ef410fec.png)


![tl (5)](https://user-images.githubusercontent.com/64778259/208597394-206cffb9-b847-4637-9e08-6f529278bad4.png)
![vl (5)](https://user-images.githubusercontent.com/64778259/208597396-3923a6be-811a-4c1e-be56-32c508df4175.png)

![va (4)](https://user-images.githubusercontent.com/64778259/208597400-973ed62e-1115-4ba2-a3cd-7f4942409dce.png)
![ta (3)](https://user-images.githubusercontent.com/64778259/208597405-1991a118-3d03-497b-8a11-7111d8c52a2e.png)


