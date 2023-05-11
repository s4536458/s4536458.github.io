# Stochastic Gradient Descent (SGD) Method

As discussed in [Article 1](article_1_DL_Explained.md), Deep Learning models require a **mechanism** to update the model parameters automatically. The **Stochastic gradient descent (SGD)** is the mathematical foundation of this mechanism. 

## Step 1: Initialize
- Gradient descent method involves starting at a random point on a function
- Hence, in DL, this involves **initializing** model parameters **(weights)** to **random values**

## Step 2: Predict
- Using weights, an expected result can be predicted

## Step 3: Determine how much test loss by
- Need to measure the effectiveness of the weights
- Using a function, we can quantitatively describe the performance (level of loss)
- Function will return:
    1. **Small number** - if the loss is minimal
    2. **Large number** - if the loss is significant
- Gives DL a way of understanding **how well** the current model is performing

## Step 4: Gradient Step
- As **weight parameters** are adjusted, change in **gradient of loss** can be measured 
- Correlates weight values with respect to model performance
- Will indicate the **winning direction**, and amount to adjust weight parameters by
