---
Link: https://blog.stevengong.co/how-does-a-neural-network-work-intuitively-in-code-f51f7b2c1e3f
ee:
  - EE
---
Hey everyone,

this is my attempt to explain how a Neural Network works. It is definitely not the first article in the world to do so, but this article is a more practical view of how Neural Networks are coded. It is less about the theory and more about understanding Neural Networks to use them in practice.

# What is a Neural Network?

A neural network is, simply put, a series of algorithms that is extremely good at recognizing underlying relationships (correlations) in a set of data through a process that mimics the way the human brain operates.

As humans, we have the exceptional ability to notice patterns in our everyday lives. Think of every time you solved a puzzle, or when you instantly recognized a song within a few seconds of it playing, or when you look anywhere and immediately recognize the thing that you are looking at. Or even when you speak. How were you able to achieve these extraordinary things without even having to think about it? This is thanks to our powerful brain, which gives us the ability to recognize patterns and notice correlations and has been the entire inspiration for the research behind **Deep learning**, with the hopes that we can create even more powerful machines by trying to replicate and even improve what humans are already able to do. Fascinating, isn’t it?

# Why do we use Neural Networks?

Neural networks have endless applications in today’s world. From solving many business problems such as sales forecasting, customer research, data validation, and risk management, to image and voice recognition in the world of medicine, to self-driving cars, the applications are truly endless.

Google’s latest self-driving car!

## So how does a Neural Network “work”?

When you think of a neural network, this image probably comes up to your mind:

Source: [https://towardsdatascience.com/applied-deep-learning-part-1-artificial-neural-networks-d7834f67a4f6](https://towardsdatascience.com/applied-deep-learning-part-1-artificial-neural-networks-d7834f67a4f6)

But chances are, you probably have no idea what this picture means.

You can think of an ANN as a model that solves a super complex math problem using a super complex math function. You give it a problem with a bunch of data describing it (the **input layer**), and it is able to find out the optimal solutions (the **output layer,** it is what you want to predict) by computing a complex function.

See the lines connecting the **nodes/neurons** represented as circles in the picture? These symbolize the **connections** that happen between neurons, and are what allows the model to become more accurate over time (by updating the **weights** of the connections).

# How it works intuitively

The creation of a basic Artificial Neural Network can be summarized in 5 steps. I will first explain it using a beginner vocabulary and re-phrase it using technical terms. They mean exactly the same thing, except the latter is a level of vocabulary widely adopted in the Deep Learning world, hence it is important to be familiar with it.

## Without the technical jargon

Imagine that you run the neural network program, and you want to teach the machine to be very good at recognizing patterns and predicting human behavior. Here’s what you would program the machine the do:

1. You give the machine some information/data about a specific specimen (ex: a customer’s banking habits and information). You tell the machine what you want it to predict exactly in regards to that specific specimen (ex: whether or not that specific customer will leave the bank in the next 6 months).
2. The computer makes a random prediction (ex: Yes, the customer will leave in the next 6 months).
3. You tell it the truth (ex: No, the customer will not leave in the next 6 months).
4. If it is wrong, it learns from its mistakes. It tries to correct itself.
5. You repeat steps 1 to 4 by giving information about new specimens (ex: You give the robot 10 000 more samples of customer information, with the truth of whether or not that customer would leave in the next 6 months). The machine keeps making mistakes, but it is gradually improving itself and becoming more accurate. Over time, the machine becomes so smart that it doesn’t need to know the truth to be able to predict the actual truth. (ex: You have a new customer now, and you have no idea whether the customer would leave in the next 6 months. You ask the robot, and it would tell you with almost 100% certainty!!)

> This is the reason Neural Networks have become so powerful in the last decade: it is thanks to its ability to continually improve and become more accurate as it learns from digesting more data. Eventually, we are able to create a model that can predict(generate) the most accurate result without needing to know it in advance.

Does it start to make sense? Now, let’s see how the same steps are reformulated using technical terms…

## With technical terms

1. Import the **training set** which serves as the **input layer**.
2. **Forward propagate** the data from the **input layer** through t**he hidden layer** to the **output layer**, where we get a predicted value **y**. Forward propagation is the process by which we multiply the **input node** by a random **weight**, and applying the **activation function**.
3. Measure the **error** between the predicted value and the real value.
4. **Backpropagate** the error and use **gradient descent** to modify the **weights** of the connections.
5. Repeats these steps until the error is **minimized** sufficiently, by finding the optimal weights.

Artificial Neural Network (Source: VIASAT)

> You might be asking yourself, how is this similar to what happens to human beings? Well, in the case of human beings, you can think of it this way: the input layer is our 5 senses, it is our raw perception of the world. Using this raw data, we are going to transform it to come to conclusions. For example, if we suddenly hear a loud bang, and we see a car flipped over after running into another one, we conclude that there was a car accident and we call the emergency services. This would be the output layer. What’s in between, how we came to that conclusion, is the hidden layer.

## Vocabulary

**The input layer:** What the machine always knows. Ex: The banking behavior of a customer.

**The hidden layer:** Where the magic happens.

**The output layer:** What the machine will predict Ex: Whether or not the customer will quit within the next 6 months.

**Node/Neuron:** A thing that holds a number. Represented by a circle in the image.

**Gradient descent:** The algorithm that allows us to get more and more accurate data as the model improves by updating the weights of the connections.

**Weights:** These are the things that get updated by the model to become more accurate after every iteration. They are represented by the connections formed between each neuron. Each connection has a different weight.

If you ever want to get more into Deep Learning, this vocabulary in bold will be an essential part of your vocabulary, alongside words such as **Activation Function**, **epochs**, **Node**, **Hyperparameters**, **overfitting**, **underfitting**, and **Optimizer**.

# **Conclusion**

After reading the article, you probably are left with tons of questions. How **exactly** does updating the weights work, and how does the machine exactly become more accurate? Why do you need a hidden layer? How do you backpropagate exactly? How does the gradient descent algorithm work? How do you pass the input?

These are all questions that are super reasonable to ask and that I would answer if I have the time and space in this article, but I really wanted to keep it concise and give you a basic introduction. There are tons of resources on the internet, hence a simple Google search will do the job.

The best way, however, is to start applying Neural Networks practically. Gradually, you will have a better grasp of Neural Networks, and soon, you will be able to write one by heart! Through the process, you will make mistakes, learn from them, and become more proficient, just like any learning process!

# What’s next?

This was just a short introduction to Artificial Neural Networks and the way they function intuitively. You are now a step closer to building your own ANN! If you feel like you are ready to code one, click here!