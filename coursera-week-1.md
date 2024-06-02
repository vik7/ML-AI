## Introduction to Machine Learning:

Machine Learning (ML) is the science of getting computers to act without being explicitly programmed. It is used in various applications like email filtering, speech recognition, and computer vision.

## Linear Regression
### Understanding linear regression with an example

Linear regression is a powerful tool in machine learning to predict dependent variables (output) based on the value of independent variables (input).

### Example

Let's say you wanna predict the price(output) of the house based on its size (input).

| Size (sq ft)    | Price (k$) |
| -------- | ------- |
| 800  | 200    |
| 1000 | 250     |
| 1200    | 300    |
| 1400    | 350    |
| 1600    | 400    |


### Steps in Linear Regression

* Plot the data
  * Plot house size on the x-axis and price on the y-axis
* Model representation
  * The linear equation can model the relationship between size and price. Price = ⍬0 + ⍬1 x size.
  * Here ⍬0 is the y-intercept (when the price is 0) and ⍬1 is the slope (the rate at which the price increases with size).
* Cost function
  * Cost function measures how well our line fits the data. It's calculated based on the average squared difference between predicted prices and the actual prices.
    J(⍬0, ⍬1) = 1/2m ∑i = 1 to m (Predicted price - Actual price)^2
* Gradient descent
  *  It's an algorithm used to minimize the cost function which measures how well a model prediction matches the actual data.
  *  The goal of Gradient Desendent is to adjust the model parameters to find the lowest point of the cost function which represents the best possible model.
  *  It adjusts ⍬0 and ⍬1 to reduce the error in the prediction. ⍬j := ⍬j - ⍺ ∂/∂⍬ J(⍬0, ⍬1)
  *  Here ⍺ is the learning rate, controlling the step size during each iteration.
 
* Simple example to understand the Gradient Descendant

  #### Imagine a Mountain
  * **Picture a Mountain:** Imagine you're at the top of a mountain and you want to find the lowest point (the valley). The mountain represents the cost function, and your position on the mountain represents the current values of the model's parameters.

  * **Finding the Slope:** At any point on the mountain, you can find the direction of the steepest descent. This is like standing on the mountain and looking around to see which direction slopes downward the most. This direction is given by the gradient of the cost function.

  * **Taking a Step:** You take a small step in the direction of the steepest descent. This step is controlled by a parameter called the learning rate, which determines how big each step should be. If the learning rate is too high, you might overshoot the valley. If it's too low, you'll take forever to get there.

  * **Repeat:** You keep taking steps, always moving downhill, until you can't go any lower. This means you've found the minimum point of the cost function, which corresponds to the best values for your model's parameters.















