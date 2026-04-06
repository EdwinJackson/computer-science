encoding is the process of transforming input data into a format that can be used by a machine learning algorithm. This transformation is necessary because machine learning algorithms typically only work with numeric data. [Encoding is used to convert categorical data into numerical data so that it can be used as input for machine learning models](https://reason.town/encoding-methods-machine-learning/)[1](https://reason.town/encoding-methods-machine-learning/)[2](https://machinelearningmastery.com/one-hot-encoding-for-categorical-data/)

It is important to understand that encoding always implies being able to undo the encoding operation in some sort of decoding operation. 

![[one-hot-encoding.png]]
## Understanding the Encoding Problem

In the neural network below each of the input features must be numeric. That means that in domains such as recommender systems, we must transform non-numeric variables (ex. items and users) into numbers and vectors. We could try to represent items by a product ID; however, neural networks treat numerical inputs as continuous variables. That means higher numbers are “greater than” lower numbers. It also sees numbers that are similar as being similar items. This makes perfect sense for a field like “age” but is nonsensical when the numbers represent a categorical variable. Prior to embeddings, one of the most common methods used was one-hot encoding.

