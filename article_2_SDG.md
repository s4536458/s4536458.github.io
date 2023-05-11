# Stochastic Gradient Descent (SGD) Method

As discussed in [Article 1](article_1_DL_Explained.md), Deep Learning models require a **mechanism** to update the model parameters automatically. The **Stochastic gradient descent (SGD)** is the mathematical foundation of this mechanism. 

## Step 1: Initialize
- Gradient descent method involves starting at a random point on a function
- In DL, this involves **initializing model parameters (weights) to random values**

## Step 2: Prediction
- Using weights, an expected result can be predicted

## Step 3: Loss
- Using a function, evaluate the actual performance of the model
- Function will returns a:
    1. **Small number** - if the loss is minimal
    2. **Large number** - if the loss is significant

> Better result = less loss = lower number

