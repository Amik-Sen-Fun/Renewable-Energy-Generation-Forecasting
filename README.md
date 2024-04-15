# Renewable Energy Generation Forecasting

> Note: This is my first project in the process of learning Data Science. I'll be studying various data science topics and refering to various research papers on the go! 

# Approach

We will be using **XGBoost** for this and try to understand this famous algorithm, that helped win various Kaggel competitions in the past! 

Firstly, XGBoost is the name of a library! For me it was a shocker because I always thought of it as some Algorithm! However, it is not! The algorithm which is implemented with the help of XGBoost is **Gradient Boosted Trees**. The Extreme version of Gradient Boosted Tree is named as XGBoost.

Gradient Boosted Trees is a method where we leverage a bunch of shitty trees to get a super tree result. From the approach it is pretty clear that it is an Ensemble method, as we are using results of multiple trees

The following is the architecture of a Gradient Boosted Trees:

<img src="https://github.com/Amik-Sen-Fun/Renewable-Energy-Generation-Forecasting/blob/main/Notes/Gradient_Boosted_Tree_Architecture.jpeg">

> P.S. I could have used a good image, but I just wanted to use my notes as it's easier for to revise and understand! :P

Let's have some clarity on the terms used! 
- X -> input features
- Y -> Feature to be predicted
- F(X) -> It refers to the output of a decision tree
- m -> The number of decision trees that we will be using inside the Gradient Boosted Trees algoritm
- α -> Learning Rate
- h(X,r) -> residual predicting function
- L(Y,F(X)) -> Loss function

In this algorithm, 
- we define a basic tree (Tree 1)
- Calculate the residual (Real Value - Predicted Value)
- Use a model that helps us predict this residual
- Use this prediction of residuals to get the new updated value of F(X)

The above steps can be mathematically explained as:

<img src="https://github.com/Amik-Sen-Fun/Renewable-Energy-Generation-Forecasting/blob/main/Notes/Mathematical_Steps.jpeg">


