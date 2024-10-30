---
Link: https://developers.google.com/machine-learning/glossary#gradient_descent
ee:
  - EE
---
A that checks whether a classifier produces the same result for one individual as it does for another individual who is identical to the first, except with respect to one or more . Evaluating a classifier for counterfactual fairness is one method for surfacing potential sources of bias in a model. A that checks whether, for a preferred (one that confers an advantage or benefit to a person) and a given , a classifier predicts that preferred label equally well for all values of that attribute. In other words, equality of opportunity measures whether the people who should qualify for an opportunity are equally likely to do so regardless of their group membership. A that checks if, for any particular label and attribute, a classifier predicts that label equally well for all values of that attribute.

Applying a constraint to an algorithm to ensure one or more definitions of fairness are satisfied. Examples of fairness constraints include:

## gradient boosted (decision) trees (GBT)

\#df

A type of [**decision forest**](https://developers.google.com/machine-learning/glossary#decision-forest) in which:

- [**Training**](https://developers.google.com/machine-learning/glossary#training) relies on [**gradient boosting**](https://developers.google.com/machine-learning/glossary#gradient-boosting).
- The weak model is a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree).

## gradient clipping

\#seq

A commonly used mechanism to mitigate the [**exploding gradient problem**](https://developers.google.com/machine-learning/glossary#exploding_gradient_problem) by artificially limiting (clipping) the maximum value of gradients when using [**gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent) to [**train**](https://developers.google.com/machine-learning/glossary#training) a model.

## gradient descent

\#fundamentals

A mathematical technique to minimize [**loss**](https://developers.google.com/machine-learning/glossary#loss). Gradient descent iteratively adjusts [**weights**](https://developers.google.com/machine-learning/glossary#weight) and [**biases**](https://developers.google.com/machine-learning/glossary#bias), gradually finding the best combination to minimize loss.

Gradient descent is older—much, much older—than machine learning.

## graph

\#TensorFlow

In TensorFlow, a computation specification. Nodes in the graph represent operations. Edges are directed and represent passing the result of an operation (a [**Tensor**](https://developers.google.com/machine-learning/glossary#tensor)) as an operand to another operation. Use [**TensorBoard**](https://developers.google.com/machine-learning/glossary#TensorBoard) to visualize a graph.

## graph execution

\#TensorFlow

A TensorFlow programming environment in which the program first constructs a [**graph**](https://developers.google.com/machine-learning/glossary#graph) and then executes all or part of that graph. Graph execution is the default execution mode in TensorFlow 1.x.

Contrast with [**eager execution**](https://developers.google.com/machine-learning/glossary#eager_execution).

## greedy policy

\#rl

In reinforcement learning, a [**policy**](https://developers.google.com/machine-learning/glossary#policy) that always chooses the action with the highest expected [**return**](https://developers.google.com/machine-learning/glossary#return).

## ground truth

\#fundamentals

Reality.

The thing that actually happened.

For example, consider a [**binary classification**](https://developers.google.com/machine-learning/glossary#binary_classification) model that predicts whether a student in their first year of university will graduate within six years. Ground truth for this model is whether or not that student actually graduated within six years.

### Click the icon for additional notes.

## group attribution bias

\#fairness

Assuming that what is true for an individual is also true for everyone in that group. The effects of group attribution bias can be exacerbated if a [**convenience sampling**](https://developers.google.com/machine-learning/glossary#convenience_sampling) is used for data collection. In a non-representative sample, attributions may be made that do not reflect reality.

See also [**out-group homogeneity bias**](https://developers.google.com/machine-learning/glossary#out-group_homogeneity_bias) and [**in-group bias**](https://developers.google.com/machine-learning/glossary#in-group_bias).

## H

## hallucination

\#language

The production of plausible-seeming but factually incorrect output by a [**generative model**](https://developers.google.com/machine-learning/glossary#generative_model) that purports to be making an assertion about the real world. For example, if a dialog agent claims that Barack Obama died in 1865, the agent is _hallucinating_.

## hashing

In machine learning, a mechanism for bucketing [**categorical data**](https://developers.google.com/machine-learning/glossary#categorical_data), particularly when the number of categories is large, but the number of categories actually appearing in the dataset is comparatively small.

For example, Earth is home to about 73,000 tree species. You could represent each of the 73,000 tree species in 73,000 separate categorical buckets. Alternatively, if only 200 of those tree species actually appear in a dataset, you could use hashing to divide tree species into perhaps 500 buckets.

A single bucket could contain multiple tree species. For example, hashing could place _baobab_ and _red maple_—two genetically dissimilar species—into the same bucket. Regardless, hashing is still a good way to map large categorical sets into the desired number of buckets. Hashing turns a categorical feature having a large number of possible values into a much smaller number of values by grouping values in a deterministic way.

## heuristic

A simple and quickly implemented solution to a problem. For example, "With a heuristic, we achieved 86% accuracy. When we switched to a deep neural network, accuracy went up to 98%."

## hidden layer

\#fundamentals

A layer in a [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network) between the [**input layer**](https://developers.google.com/machine-learning/glossary#input_layer) (the features) and the [**output layer**](https://developers.google.com/machine-learning/glossary#output_layer) (the prediction). Each hidden layer consists of one or more [**neurons**](https://developers.google.com/machine-learning/glossary#neuron). For example, the following neural network contains two hidden layers, the first with three neurons and the second with two neurons:

![[HiddenLayerBigPicture.png]]

A [**deep neural network**](https://developers.google.com/machine-learning/glossary#deep_neural_network) contains more than one hidden layer. For example, the preceding illustration is a deep neural network because the model contains two hidden layers.

## hierarchical clustering

\#clustering

A category of [**clustering**](https://developers.google.com/machine-learning/glossary#clustering) algorithms that create a tree of clusters. Hierarchical clustering is well-suited to hierarchical data, such as botanical taxonomies. There are two types of hierarchical clustering algorithms:

- **Agglomerative clustering** first assigns every example to its own cluster, and iteratively merges the closest clusters to create a hierarchical tree.
- **Divisive clustering** first groups all examples into one cluster and then iteratively divides the cluster into a hierarchical tree.

Contrast with [**centroid-based clustering**](https://developers.google.com/machine-learning/glossary#centroid_based_clustering).

## hinge loss

A family of [**loss**](https://developers.google.com/machine-learning/glossary#loss) functions for [**classification**](https://developers.google.com/machine-learning/glossary#classification_model) designed to find the [**decision boundary**](https://developers.google.com/machine-learning/glossary#decision_boundary) as distant as possible from each training example, thus maximizing the margin between examples and the boundary. [**KSVMs**](https://developers.google.com/machine-learning/glossary#KSVMs) use hinge loss (or a related function, such as squared hinge loss). For binary classification, the hinge loss function is defined as follows:

loss=max(0,1−(y∗y′))

where _y_ is the true label, either -1 or +1, and _y'_ is the raw output of the classifier model:

y′=b+w1x1+w2x2+…wnxn

Consequently, a plot of hinge loss vs. (y * y') looks as follows:

![[hinge-loss.svg]]

## holdout data

[**Examples**](https://developers.google.com/machine-learning/glossary#example) intentionally not used ("held out") during training. The [**validation dataset**](https://developers.google.com/machine-learning/glossary#validation_set) and [**test dataset**](https://developers.google.com/machine-learning/glossary#test_set) are examples of holdout data. Holdout data helps evaluate your model's ability to generalize to data other than the data it was trained on. The loss on the holdout set provides a better estimate of the loss on an unseen dataset than does the loss on the training set.

## hyperparameter

\#fundamentals

The variables that you or a hyperparameter tuning service adjust during successive runs of training a model. For example, [**learning rate**](https://developers.google.com/machine-learning/glossary#learning_rate) is a hyperparameter. You could set the learning rate to 0.01 before one training session. If you determine that 0.01 is too high, you could perhaps set the learning rate to 0.003 for the next training session.

In contrast, [**parameters**](https://developers.google.com/machine-learning/glossary#parameter) are the various [**weights**](https://developers.google.com/machine-learning/glossary#weight) and [**bias**](https://developers.google.com/machine-learning/glossary#bias) that the model _learns_ during training.

## hyperplane

A boundary that separates a space into two subspaces. For example, a line is a hyperplane in two dimensions and a plane is a hyperplane in three dimensions. More typically in machine learning, a hyperplane is the boundary separating a high-dimensional space. [**Kernel Support Vector Machines**](https://developers.google.com/machine-learning/glossary#KSVMs) use hyperplanes to separate positive classes from negative classes, often in a very high-dimensional space.

## I

## i.i.d.

Abbreviation for [**independently and identically distributed**](https://developers.google.com/machine-learning/glossary#iid).

## image recognition

\#image

A process that classifies object(s), pattern(s), or concept(s) in an image. Image recognition is also known as **image classification**.

For more information, see [ML Practicum: Image Classification](https://developers.google.com/machine-learning/practica/image-classification).

## imbalanced dataset

Synonym for [**class-imbalanced dataset**](https://developers.google.com/machine-learning/glossary#class_imbalanced_data_set).

## implicit bias

\#fairness

Automatically making an association or assumption based on one’s mental models and memories. Implicit bias can affect the following:

- How data is collected and classified.
- How machine learning systems are designed and developed.

For example, when building a classifier to identify wedding photos, an engineer may use the presence of a white dress in a photo as a feature. However, white dresses have been customary only during certain eras and in certain cultures.

See also [**confirmation bias**](https://developers.google.com/machine-learning/glossary#confirmation_bias).

## imputation

Short form of [**value imputation**](https://developers.google.com/machine-learning/glossary#value-imputation).

## incompatibility of fairness metrics

\#fairness

The idea that some notions of fairness are mutually incompatible and cannot be satisfied simultaneously. As a result, there is no single universal [**metric**](https://developers.google.com/machine-learning/glossary#fairness_metric) for quantifying fairness that can be applied to all ML problems.

While this may seem discouraging, incompatibility of fairness metrics doesn’t imply that fairness efforts are fruitless. Instead, it suggests that fairness must be defined contextually for a given ML problem, with the goal of preventing harms specific to its use cases.

See ["On the (im)possibility of fairness"](https://arxiv.org/pdf/1609.07236.pdf) for a more detailed discussion of this topic.

## independently and identically distributed (i.i.d)

\#fundamentals

Data drawn from a distribution that doesn't change, and where each value drawn doesn't depend on values that have been drawn previously. An i.i.d. is the [ideal gas](https://wikipedia.org/wiki/Ideal_gas) of machine learning—a useful mathematical construct but almost never exactly found in the real world. For example, the distribution of visitors to a web page may be i.i.d. over a brief window of time; that is, the distribution doesn't change during that brief window and one person's visit is generally independent of another's visit. However, if you expand that window of time, seasonal differences in the web page's visitors may appear.

See also [**nonstationarity**](https://developers.google.com/machine-learning/glossary#nonstationarity).

## individual fairness

\#fairness

A fairness metric that checks whether similar individuals are classified similarly. For example, Brobdingnagian Academy might want to satisfy individual fairness by ensuring that two students with identical grades and standardized test scores are equally likely to gain admission.

Note that individual fairness relies entirely on how you define "similarity" (in this case, grades and test scores), and you can run the risk of introducing new fairness problems if your similarity metric misses important information (such as the rigor of a student’s curriculum).

See ["Fairness Through Awareness"](https://arxiv.org/pdf/1104.3913.pdf) for a more detailed discussion of individual fairness.

## inference

\#fundamentals

In machine learning, the process of making predictions by applying a trained model to [**unlabeled examples**](https://developers.google.com/machine-learning/glossary#unlabeled_example).

Inference has a somewhat different meaning in statistics. See the [Wikipedia article on statistical inference](https://wikipedia.org/wiki/Statistical_inference) for details.

## inference path

\#df

In a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree), during [**inference**](https://developers.google.com/machine-learning/glossary#inference), the route a particular [**example**](https://developers.google.com/machine-learning/glossary#example) takes from the [**root**](https://developers.google.com/machine-learning/glossary#root) to other [**conditions**](https://developers.google.com/machine-learning/glossary#condition), terminating with a [**leaf**](https://developers.google.com/machine-learning/glossary#leaf). For instance, in the following decision tree, the thicker arrows show the inference path for an example with the following feature values:

- x = 7
- y = 12
- z = -3

The inference path in the following illustration travels through three conditions before reaching the leaf (`Zeta`).

**The three thick arrows show the inference path.**

## information gain

\#df

In [**decision forests**](https://developers.google.com/machine-learning/glossary#decision-forest), the difference between a node's [**entropy**](https://developers.google.com/machine-learning/glossary#entropy) and the weighted (by number of examples) sum of the entropy of its children nodes. A node's entropy is the entropy of the examples in that node.

For example, consider the following entropy values:

- entropy of parent node = 0.6
- entropy of one child node with 16 relevant examples = 0.2
- entropy of another child node with 24 relevant examples = 0.1

So 40% of the examples are in one child node and 60% are in the other child node. Therefore:

- weighted entropy sum of child nodes = (0.4 * 0.2) + (0.6 * 0.1) = 0.14

So, the information gain is:

- information gain = entropy of parent node - weighted entropy sum of child nodes
- information gain = 0.6 - 0.14 = 0.46

Most [**splitters**](https://developers.google.com/machine-learning/glossary#splitter) seek to create [**conditions**](https://developers.google.com/machine-learning/glossary#condition) that maximize information gain.

## in-group bias

\#fairness

Showing partiality to one's own group or own characteristics. If testers or raters consist of the machine learning developer's friends, family, or colleagues, then in-group bias may invalidate product testing or the dataset.

In-group bias is a form of [**group attribution bias**](https://developers.google.com/machine-learning/glossary#group_attribution_bias). See also [**out-group homogeneity bias**](https://developers.google.com/machine-learning/glossary#out-group_homogeneity_bias).

## input generator

A mechanism by which data is loaded into a [**neural network**](https://developers.google.com/machine-learning/glossary#neural-network).

An input generator can be thought of as a component responsible for processing raw data into tensors which are iterated over to generate batches for training, evaluation, and inference.

## input layer

\#fundamentals

The [**layer**](https://developers.google.com/machine-learning/glossary#layer) of a [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network) that holds the [**feature vector**](https://developers.google.com/machine-learning/glossary#feature_vector). That is, the input layer provides [**examples**](https://developers.google.com/machine-learning/glossary#example) for [**training**](https://developers.google.com/machine-learning/glossary#training) or [**inference**](https://developers.google.com/machine-learning/glossary#inference). For example, the input layer in the following neural network consists of two features:

## in-set condition

\#df

In a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree), a [**condition**](https://developers.google.com/machine-learning/glossary#condition) that tests for the presence of one item in a set of items. For example, the following is an in-set condition:

```Plain
  house-style in [tudor, colonial, cape]
```

During inference, if the value of the house-style [**feature**](https://developers.google.com/machine-learning/glossary#feature) is `tudor` or `colonial` or `cape`, then this condition evaluates to Yes. If the value of the house-style feature is something else (for example, `ranch`), then this condition evaluates to No.

In-set conditions usually lead to more efficient decision trees than conditions that test [**one-hot encoded**](https://developers.google.com/machine-learning/glossary#one-hot_encoding) features.

## instance

Synonym for [**example**](https://developers.google.com/machine-learning/glossary#example).

## interpretability

\#fundamentals

The ability to explain or to present an ML model's reasoning in understandable terms to a human.

Most linear regression models, for example, are highly interpretable. (You merely need to look at the trained weights for each feature.) Decision forests are also highly interpretable. Some models, however, require sophisticated visualization to become interpretable.

## inter-rater agreement

A measurement of how often human raters agree when doing a task. If raters disagree, the task instructions may need to be improved. Also sometimes called **inter-annotator agreement** or **inter-rater reliability**. See also [Cohen's kappa](https://wikipedia.org/wiki/Cohen%27s_kappa), which is one of the most popular inter-rater agreement measurements.

## intersection over union (IoU)

\#image

The intersection of two sets divided by their union. In machine-learning image-detection tasks, IoU is used to measure the accuracy of the model’s predicted [**bounding box**](https://developers.google.com/machine-learning/glossary#bounding_box) with respect to the [**ground-truth**](https://developers.google.com/machine-learning/glossary#ground_truth) bounding box. In this case, the IoU for the two boxes is the ratio between the overlapping area and the total area, and its value ranges from 0 (no overlap of predicted bounding box and ground-truth bounding box) to 1 (predicted bounding box and ground-truth bounding box have the exact same coordinates).

For example, in the image below:

- The predicted bounding box (the coordinates delimiting where the model predicts the night table in the painting is located) is outlined in purple.
- The ground-truth bounding box (the coordinates delimiting where the night table in the painting is actually located) is outlined in green.

## IoU

Abbreviation for [**intersection over union**](https://developers.google.com/machine-learning/glossary#intersection_over_union).

## item matrix

\#recsystems

In [**recommendation systems**](https://developers.google.com/machine-learning/glossary#recommendation_system), a matrix of [**embedding vectors**](https://developers.google.com/machine-learning/glossary#embedding_vector) generated by [**matrix factorization**](https://developers.google.com/machine-learning/glossary#matrix_factorization) that holds latent signals about each [**item**](https://developers.google.com/machine-learning/glossary#items). Each row of the item matrix holds the value of a single latent feature for all items. For example, consider a movie recommendation system. Each column in the item matrix represents a single movie. The latent signals might represent genres, or might be harder-to-interpret signals that involve complex interactions among genre, stars, movie age, or other factors.

The item matrix has the same number of columns as the target matrix that is being factorized. For example, given a movie recommendation system that evaluates 10,000 movie titles, the item matrix will have 10,000 columns.

## items

\#recsystems

In a [**recommendation system**](https://developers.google.com/machine-learning/glossary#recommendation_system), the entities that a system recommends. For example, videos are the items that a video store recommends, while books are the items that a bookstore recommends.

## iteration

\#fundamentals

A single update of a [**model's**](https://developers.google.com/machine-learning/glossary#model) parameters—the model's [**weights**](https://developers.google.com/machine-learning/glossary#weight) and [**biases**](https://developers.google.com/machine-learning/glossary#bias)—during [**training**](https://developers.google.com/machine-learning/glossary#training). The [**batch size**](https://developers.google.com/machine-learning/glossary#batch_size) determines how many examples the model processes in a single iteration. For instance, if the batch size is 20, then the model processes 20 examples before adjusting the parameters.

When training a [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network), a single iteration involves the following two passes:

1. A forward pass to evaluate loss on a single batch.
2. A backward pass ([**backpropagation**](https://developers.google.com/machine-learning/glossary#backpropagation)) to adjust the model's parameters based on the loss and the learning rate.

## J

## JAX

An array computing library, bringing together [**XLA (Accelerated Linear Algebra)**](https://developers.google.com/machine-learning/glossary#XLA) and automatic differentiation for high-performance numerical computing. JAX provides a simple and powerful API for writing accelerated numerical code with composable transformations. JAX provides features such as:

- `grad` (automatic differentiation)
- `jit` (just-in-time compilation)
- `vmap` (automatic vectorization or batching)
- `pmap` (parallelization)

JAX is a language for expressing and composing transformations of numerical code, analogous—but much larger in scope—to Python’s [**NumPy**](https://developers.google.com/machine-learning/glossary#numpy) library. (In fact, the .numpy library under JAX is a functionally equivalent, but entirely rewritten version of the Python NumPy library.)

JAX is particularly well-suited for speeding up many machine learning tasks by transforming the models and data into a form suitable for parallelism across GPU and [**TPU**](https://developers.google.com/machine-learning/glossary#TPU) [**accelerator chips**](https://developers.google.com/machine-learning/glossary#accelerator-chip).

[**Flax**](https://developers.google.com/machine-learning/glossary#flax), [**Optax**](https://developers.google.com/machine-learning/glossary#optax), [**Pax**](https://developers.google.com/machine-learning/glossary#pax), and many other libraries are built on the JAX infrastructure.

## K

## Keras

A popular Python machine learning API. [Keras](https://keras.io/) runs on several deep learning frameworks, including TensorFlow, where it is made available as [tf.keras](https://www.tensorflow.org/api_docs/python/tf/keras).

## keypoints

\#image

The coordinates of particular features in an image. For example, for an [**image recognition**](https://developers.google.com/machine-learning/glossary#image_recognition) model that distinguishes flower species, keypoints might be the center of each petal, the stem, the stamen, and so on.

## Kernel Support Vector Machines (KSVMs)

A classification algorithm that seeks to maximize the margin between [**positive**](https://developers.google.com/machine-learning/glossary#positive_class) and [**negative classes**](https://developers.google.com/machine-learning/glossary#negative_class) by mapping input data vectors to a higher dimensional space. For example, consider a classification problem in which the input dataset has a hundred features. To maximize the margin between positive and negative classes, a KSVM could internally map those features into a million-dimension space. KSVMs uses a loss function called [**hinge loss**](https://developers.google.com/machine-learning/glossary#hinge-loss).

## k-fold cross validation

An algorithm for predicting a model's ability to [**generalize**](https://developers.google.com/machine-learning/glossary#generalization) to new data. The _k_ in k-fold refers to the number of equal groups you divide a dataset's examples into; that is, you train and test your model k times. For each round of training and testing, a different group is the test set, and all remaining groups become the training set. After k rounds of training and testing, you calculate the mean and standard deviation of the desired test metric(s).

For example, suppose your dataset consists of 120 examples. Further suppose, you decide to set k to 4. Therefore, after shuffling the examples, you divide the dataset into four equal groups of 30 examples and conduct four training/testing rounds:

For example, [**Mean Squared Error (MSE)**](https://developers.google.com/machine-learning/glossary#MSE) might be the most meaningful metric for a linear regression model. Therefore, you would find the mean and standard deviation of the MSE across all four rounds.

## k-means

\#clustering

A popular [**clustering**](https://developers.google.com/machine-learning/glossary#clustering) algorithm that groups examples in unsupervised learning. The k-means algorithm basically does the following:

- Iteratively determines the best k center points (known as [**centroids**](https://developers.google.com/machine-learning/glossary#centroid)).
- Assigns each example to the closest centroid. Those examples nearest the same centroid belong to the same group.

The k-means algorithm picks centroid locations to minimize the cumulative _square_ of the distances from each example to its closest centroid.

For example, consider the following plot of dog height to dog width:

If k=3, the k-means algorithm will determine three centroids. Each example is assigned to its closest centroid, yielding three groups:

Imagine that a manufacturer wants to determine the ideal sizes for small, medium, and large sweaters for dogs. The three centroids identify the mean height and mean width of each dog in that cluster. So, the manufacturer should probably base sweater sizes on those three centroids. Note that the centroid of a cluster is typically _not_ an example in the cluster.

The preceding illustrations shows k-means for examples with only two features (height and width). Note that k-means can group examples across many features.

## k-median

\#clustering

A clustering algorithm closely related to [**k-means**](https://developers.google.com/machine-learning/glossary#k-means). The practical difference between the two is as follows:

- In k-means, centroids are determined by minimizing the sum of the _squares_ of the distance between a centroid candidate and each of its examples.
- In k-median, centroids are determined by minimizing the sum of the distance between a centroid candidate and each of its examples.

Note that the definitions of distance are also different:

- k-means relies on the [Euclidean distance](https://wikipedia.org/wiki/Euclidean_distance) from the centroid to an example. (In two dimensions, the Euclidean distance means using the Pythagorean theorem to calculate the hypotenuse.) For example, the k-means distance between (2,2) and (5,-2) would be:

Euclidean distance=(2−5)2+(2−−2)2=5

- k-median relies on the [Manhattan distance](https://wikipedia.org/wiki/Taxicab_geometry) from the centroid to an example. This distance is the sum of the absolute deltas in each dimension. For example, the k-median distance between (2,2) and (5,-2) would be:

Manhattan distance=|2−5|+|2−−2|=7

## L

## L0 regularization

\#fundamentals

A type of [**regularization**](https://developers.google.com/machine-learning/glossary#regularization) that penalizes the _total number_ of nonzero [**weights**](https://developers.google.com/machine-learning/glossary#weight) in a model. For example, a model having 11 nonzero weights would be penalized more than a similar model having 10 nonzero weights.

L0 regularization is sometimes called _L0-norm regularization_.

### Click the icon for additional notes.

## L1 loss

\#fundamentals

A [**loss function**](https://developers.google.com/machine-learning/glossary#loss-function) that calculates the absolute value of the difference between actual [**label**](https://developers.google.com/machine-learning/glossary#label) values and the values that a [**model**](https://developers.google.com/machine-learning/glossary#model) predicts. For example, here's the calculation of L1 loss for a [**batch**](https://developers.google.com/machine-learning/glossary#batch) of five [**examples**](https://developers.google.com/machine-learning/glossary#example):

|   |   |   |
|---|---|---|
|Actual value of example|Model's predicted value|Absolute value of delta|
|7|6|1|
|5|4|1|
|8|11|3|
|4|6|2|
|9|8|1|
|||8 = L1 loss|

L1 loss is less sensitive to [**outliers**](https://developers.google.com/machine-learning/glossary#outliers) than [**L**](https://developers.google.com/machine-learning/glossary#squared_loss)[**2**](https://developers.google.com/machine-learning/glossary#squared_loss) [**loss**](https://developers.google.com/machine-learning/glossary#squared_loss).

The [**Mean Absolute Error**](https://developers.google.com/machine-learning/glossary#MAE) is the average L1 loss per example.

### Click the icon to see the formal math.

## L1 regularization

\#fundamentals

A type of [**regularization**](https://developers.google.com/machine-learning/glossary#regularization) that penalizes [**weights**](https://developers.google.com/machine-learning/glossary#weight) in proportion to the sum of the absolute value of the weights. L1 regularization helps drive the weights of irrelevant or barely relevant features to _exactly 0_. A [**feature**](https://developers.google.com/machine-learning/glossary#feature) with a weight of 0 is effectively removed from the model.

Contrast with [**L**](https://developers.google.com/machine-learning/glossary#L2_regularization)[**2**](https://developers.google.com/machine-learning/glossary#L2_regularization) [**regularization**](https://developers.google.com/machine-learning/glossary#L2_regularization).

## L2 loss

\#fundamentals

A [**loss function**](https://developers.google.com/machine-learning/glossary#loss-function) that calculates the square of the difference between actual [**label**](https://developers.google.com/machine-learning/glossary#label) values and the values that a [**model**](https://developers.google.com/machine-learning/glossary#model) predicts. For example, here's the calculation of L2 loss for a [**batch**](https://developers.google.com/machine-learning/glossary#batch) of five [**examples**](https://developers.google.com/machine-learning/glossary#example):

|   |   |   |
|---|---|---|
|Actual value of example|Model's predicted value|Square of delta|
|7|6|1|
|5|4|1|
|8|11|9|
|4|6|4|
|9|8|1|
|||16 = L2 loss|

Due to squaring, L2 loss amplifies the influence of [**outliers**](https://developers.google.com/machine-learning/glossary#outliers). That is, L2 loss reacts more strongly to bad predictions than [**L**](https://developers.google.com/machine-learning/glossary#L1_loss)[**1**](https://developers.google.com/machine-learning/glossary#L1_loss) [**loss**](https://developers.google.com/machine-learning/glossary#L1_loss). For example, the L1 loss for the preceding batch would be 8 rather than 16. Notice that a single outlier accounts for 9 of the 16.

[**Regression models**](https://developers.google.com/machine-learning/glossary#regression_model) typically use L2 loss as the loss function.

The [**Mean Squared Error**](https://developers.google.com/machine-learning/glossary#MSE) is the average L2 loss per example. **Squared loss** is another name for L2 loss.

### Click the icon to see the formal math.

## L2 regularization

\#fundamentals

A type of [**regularization**](https://developers.google.com/machine-learning/glossary#regularization) that penalizes [**weights**](https://developers.google.com/machine-learning/glossary#weight) in proportion to the sum of the _squares_ of the weights. L2 regularization helps drive [**outlier**](https://developers.google.com/machine-learning/glossary#outliers) weights (those with high positive or low negative values) closer to 0 but _not quite to 0_. Features with values very close to 0 remain in the model but don't influence the model's prediction very much.

L2 regularization always improves generalization in [**linear models**](https://developers.google.com/machine-learning/glossary#linear_model).

Contrast with [**L**](https://developers.google.com/machine-learning/glossary#L1_regularization)[**1**](https://developers.google.com/machine-learning/glossary#L1_regularization) [**regularization**](https://developers.google.com/machine-learning/glossary#L1_regularization).

## label

\#fundamentals

In [**supervised machine learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning), the "answer" or "result" portion of an [**example**](https://developers.google.com/machine-learning/glossary#example).

Each [**labeled example**](https://developers.google.com/machine-learning/glossary#labeled_example) consists of one or more [**features**](https://developers.google.com/machine-learning/glossary#feature) and a label. For instance, in a spam detection dataset, the label would probably be either "spam" or "not spam." In a rainfall dataset, the label might be the amount of rain that fell during a certain period.

## labeled example

\#fundamentals

An example that contains one or more [**features**](https://developers.google.com/machine-learning/glossary#feature) and a [**label**](https://developers.google.com/machine-learning/glossary#label). For example, the following table shows three labeled examples from a house valuation model, each with three features and one label:

|   |   |   |   |
|---|---|---|---|
|Number of bedrooms|Number of bathrooms|House age|House price (label)|
|3|2|15|$345,000|
|2|1|72|$179,000|
|4|2|34|$392,000|

In [**supervised machine learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning), models train on labeled examples and make predictions on [**unlabeled examples**](https://developers.google.com/machine-learning/glossary#unlabeled_example).

Contrast labeled example with unlabeled examples.

## label leakage

A model design flaw in which a [**feature**](https://developers.google.com/machine-learning/glossary#feature) is a proxy for the [**label**](https://developers.google.com/machine-learning/glossary#label). For example, consider a [**binary classification**](https://developers.google.com/machine-learning/glossary#binary-classification) model that predicts whether or not a prospective customer will purchase a particular product. Suppose that one of the features for the model is a Boolean named `SpokeToCustomerAgent`. Further suppose that a customer agent is only assigned _after_ the prospective customer has actually purchased the product. During training, the model will quickly learn the association between `SpokeToCustomerAgent` and the label.

## LaMDA (Language Model for Dialogue Applications)

\#language

A [**Transformer**](https://developers.google.com/machine-learning/glossary#Transformer)-based [**large language model**](https://developers.google.com/machine-learning/glossary#large-language-model) developed by Google trained on a large dialogue dataset that can generate realistic conversational responses.

[LaMDA: our breakthrough conversation technology](https://blog.google/technology/ai/lamda/) provides an overview.

## lambda

\#fundamentals

Synonym for [**regularization rate**](https://developers.google.com/machine-learning/glossary#regularization_rate).

Lambda is an overloaded term. Here we're focusing on the term's definition within [**regularization**](https://developers.google.com/machine-learning/glossary#regularization).

## landmarks

\#image

Synonym for [**keypoints**](https://developers.google.com/machine-learning/glossary#keypoints).

## language model

\#language

A [**model**](https://developers.google.com/machine-learning/glossary#model) that estimates the probability of a [**token**](https://developers.google.com/machine-learning/glossary#token) or sequence of tokens occurring in a longer sequence of tokens.

### Click the icon for additional notes.

## large language model

\#language

An informal term with no strict definition that usually means a [**language model**](https://developers.google.com/machine-learning/glossary#language-model) that has a high number of [**parameters**](https://developers.google.com/machine-learning/glossary#parameter). Some large language models contain over 100 billion parameters.

### Click the icon for additional notes.

## layer

\#fundamentals

A set of [**neurons**](https://developers.google.com/machine-learning/glossary#neuron) in a [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network). Three common types of layers are as follows:

- The [**input layer**](https://developers.google.com/machine-learning/glossary#input_layer), which provides values for all the [**features**](https://developers.google.com/machine-learning/glossary#feature).
- One or more [**hidden layers**](https://developers.google.com/machine-learning/glossary#hidden_layer), which find nonlinear relationships between the features and the label.
- The [**output layer**](https://developers.google.com/machine-learning/glossary#output_layer), which provides the prediction.

For example, the following illustration shows a neural network with one input layer, two hidden layers, and one output layer:

In [**TensorFlow**](https://developers.google.com/machine-learning/glossary#TensorFlow), **layers** are also Python functions that take [**Tensors**](https://developers.google.com/machine-learning/glossary#tensor) and configuration options as input and produce other tensors as output.

## Layers API (tf.layers)

\#TensorFlow

A TensorFlow API for constructing a [**deep**](https://developers.google.com/machine-learning/glossary#deep_model) neural network as a composition of layers. The Layers API enables you to build different types of [**layers**](https://developers.google.com/machine-learning/glossary#layer), such as:

- `tf.layers.Dense` for a [**fully-connected layer**](https://developers.google.com/machine-learning/glossary#fully_connected_layer).
- `tf.layers.Conv2D` for a convolutional layer.

The Layers API follows the [**Keras**](https://developers.google.com/machine-learning/glossary#Keras) layers API conventions. That is, aside from a different prefix, all functions in the Layers API have the same names and signatures as their counterparts in the Keras layers API.

## leaf

\#df

Any endpoint in a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree). Unlike a [**condition**](https://developers.google.com/machine-learning/glossary#condition), a leaf does not perform a test. Rather, a leaf is a possible prediction. A leaf is also the terminal [**node**](https://developers.google.com/machine-learning/glossary#node) of an [**inference path**](https://developers.google.com/machine-learning/glossary#inference-path).

For example, the following decision tree contains three leaves:

## learning rate

\#fundamentals

A floating-point number that tells the [**gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent) algorithm how strongly to adjust weights and biases on each [**iteration**](https://developers.google.com/machine-learning/glossary#iteration). For example, a learning rate of 0.3 would adjust weights and biases three times more powerfully than a learning rate of 0.1.

Learning rate is a key [**hyperparameter**](https://developers.google.com/machine-learning/glossary#hyperparameter). If you set the learning rate too low, training will take too long. If you set the learning rate too high, gradient descent often has trouble reaching [**convergence**](https://developers.google.com/machine-learning/glossary#convergence).

### Click the icon for a more mathematical explanation.

## least squares regression

A linear regression model trained by minimizing [**L**](https://developers.google.com/machine-learning/glossary#L2_loss)[**2**](https://developers.google.com/machine-learning/glossary#L2_loss) [**Loss**](https://developers.google.com/machine-learning/glossary#L2_loss).

## linear model

\#fundamentals

A [**model**](https://developers.google.com/machine-learning/glossary#model) that assigns one [**weight**](https://developers.google.com/machine-learning/glossary#weight) per [**feature**](https://developers.google.com/machine-learning/glossary#feature) to make [**predictions**](https://developers.google.com/machine-learning/glossary#prediction). (Linear models also incorporate a [**bias**](https://developers.google.com/machine-learning/glossary#bias).) In contrast, the relationship of features to predictions in [**deep models**](https://developers.google.com/machine-learning/glossary#deep_model) is generally **nonlinear**.

Linear models are usually easier to train and more [**interpretable**](https://developers.google.com/machine-learning/glossary#interpretability) than deep models. However, deep models can learn complex relationships _between_ features.

[**Linear regression**](https://developers.google.com/machine-learning/glossary#linear_regression) and [**logistic regression**](https://developers.google.com/machine-learning/glossary#logistic_regression) are two types of linear models.

### Click the icon to see the math.

## linear

\#fundamentals

A relationship between two or more variables that can be represented solely through addition and multiplication.

The plot of a linear relationship is a line.

Contrast with [**nonlinear**](https://developers.google.com/machine-learning/glossary#nonlinear).

## linear regression

\#fundamentals

A type of machine learning model in which both of the following are true:

- The model is a [**linear model**](https://developers.google.com/machine-learning/glossary#linear_model).
- The prediction is a floating-point value. (This is the [**regression**](https://developers.google.com/machine-learning/glossary#regression_model) part of _linear regression_.)

Contrast linear regression with [**logistic regression**](https://developers.google.com/machine-learning/glossary#logistic_regression). Also, contrast regression with [**classification**](https://developers.google.com/machine-learning/glossary#classification_model).

## logistic regression

\#fundamentals

A type of [**regression model**](https://developers.google.com/machine-learning/glossary#regression_model) that predicts a probability. Logistic regression models have the following characteristics:

- The label is [**categorical**](https://developers.google.com/machine-learning/glossary#categorical_data). The term logistic regression usually refers to **binary logistic regression**, that is, to a model that calculates probabilities for labels with two possible values. A less common variant, **multinomial logistic regression**, calculates probabilities for labels with more than two possible values.
- The loss function during training is [**Log Loss**](https://developers.google.com/machine-learning/glossary#Log_Loss). (Multiple Log Loss units can be placed in parallel for labels with more than two possible values.)
- The model has a linear architecture, not a deep neural network. However, the remainder of this definition also applies to [**deep models**](https://developers.google.com/machine-learning/glossary#deep_model) that predict probabilities for categorical labels.

For example, consider a logistic regression model that calculates the probability of an input email being either spam or not spam. During inference, suppose the model predicts 0.72. Therefore, the model is estimating:

- A 72% chance of the email being spam.
- A 28% chance of the email not being spam.

A logistic regression model uses the following two-step architecture:

1. The model generates a raw prediction (y') by applying a linear function of input features.
2. The model uses that raw prediction as input to a [**sigmoid function**](https://developers.google.com/machine-learning/glossary#sigmoid-function), which converts the raw prediction to a value between 0 and 1, exclusive.

Like any regression model, a logistic regression model predicts a number. However, this number typically becomes part of a binary classification model as follows:

- If the predicted number is _greater_ than the [**classification threshold**](https://developers.google.com/machine-learning/glossary#classification_threshold), the binary classification model predicts the positive class.
- If the predicted number is _less_ than the classification threshold, the binary classification model predicts the negative class.

## logits

The vector of raw (non-normalized) predictions that a classification model generates, which is ordinarily then passed to a normalization function. If the model is solving a [**multi-class classification**](https://developers.google.com/machine-learning/glossary#multi-class) problem, logits typically become an input to the [**softmax**](https://developers.google.com/machine-learning/glossary#softmax) function. The softmax function then generates a vector of (normalized) probabilities with one value for each possible class.

[tf.nn.sigmoid_cross_entropy_with_logits](https://www.tensorflow.org/api_docs/python/tf/nn/sigmoid_cross_entropy_with_logits).

## Log Loss

\#fundamentals

The [**loss function**](https://developers.google.com/machine-learning/glossary#loss-function) used in binary [**logistic regression**](https://developers.google.com/machine-learning/glossary#logistic_regression).

### Click the icon to see the math.

## log-odds

\#fundamentals

The logarithm of the odds of some event.

### Click the icon to see the math.

## Long Short-Term Memory (LSTM)

\#seq

A type of cell in a [**recurrent neural network**](https://developers.google.com/machine-learning/glossary#recurrent_neural_network) used to process sequences of data in applications such as handwriting recognition, machine translation, and image captioning. LSTMs address the [**vanishing gradient problem**](https://developers.google.com/machine-learning/glossary#vanishing_gradient_problem) that occurs when training RNNs due to long data sequences by maintaining history in an internal memory state based on new input and context from previous cells in the RNN.

## loss

\#fundamentals

During the [**training**](https://developers.google.com/machine-learning/glossary#training) of a [**supervised model**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning), a measure of how far a model's [**prediction**](https://developers.google.com/machine-learning/glossary#prediction) is from its [**label**](https://developers.google.com/machine-learning/glossary#label).

A [**loss function**](https://developers.google.com/machine-learning/glossary#loss-function) calculates the loss.

## loss aggregator

A type of [**machine learning**](https://developers.google.com/machine-learning/glossary#machine_learning) algorithm that improves the [**performance**](https://developers.google.com/machine-learning/glossary#performance) of a [**model**](https://developers.google.com/machine-learning/glossary#model) by combining the [**predictions**](https://developers.google.com/machine-learning/glossary#prediction) of multiple models and using those predictions to make a single prediction. As a result, a loss aggregator can reduce the variance of the predictions and improve the [**accuracy**](https://developers.google.com/machine-learning/glossary#accuracy) of the predictions.

## loss curve

\#fundamentals

A plot of [**loss**](https://developers.google.com/machine-learning/glossary#loss) as a function of the number of training [**iterations**](https://developers.google.com/machine-learning/glossary#iteration). The following plot shows a typical loss curve:

Loss curves can help you determine when your model is [**converging**](https://developers.google.com/machine-learning/glossary#convergence) or [**overfitting**](https://developers.google.com/machine-learning/glossary#overfitting).

Loss curves can plot all of the following types of loss:

- [**training loss**](https://developers.google.com/machine-learning/glossary#training-loss)
- [**validation loss**](https://developers.google.com/machine-learning/glossary#validation-loss)
- [**test loss**](https://developers.google.com/machine-learning/glossary#test-loss)

See also [**generalization curve**](https://developers.google.com/machine-learning/glossary#generalization_curve).

## loss function

\#fundamentals

During [**training**](https://developers.google.com/machine-learning/glossary#training) or testing, a mathematical function that calculates the loss on a [**batch**](https://developers.google.com/machine-learning/glossary#batch) of examples. A loss function returns a lower loss for models that makes good predictions than for models that make bad predictions.

The goal of training is typically to minimize the loss that a loss function returns.

Many different kinds of loss functions exist. Pick the appropriate loss function for the kind of model you are building. For example:

- [**L**](https://developers.google.com/machine-learning/glossary#L2_loss)[**2**](https://developers.google.com/machine-learning/glossary#L2_loss) [**loss**](https://developers.google.com/machine-learning/glossary#L2_loss) (or [**Mean Squared Error**](https://developers.google.com/machine-learning/glossary#MSE)) is the loss function for [**linear regression**](https://developers.google.com/machine-learning/glossary#linear_regression).
- [**Log Loss**](https://developers.google.com/machine-learning/glossary#Log_Loss) is the loss function for [**logistic regression**](https://developers.google.com/machine-learning/glossary#logistic_regression).

## loss surface

A graph of weight(s) vs. loss. [**Gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent) aims to find the weight(s) for which the loss surface is at a local minimum.

## LSTM

\#seq

Abbreviation for [**Long Short-Term Memory**](https://developers.google.com/machine-learning/glossary#Long_Short-Term_Memory).

## M

## machine learning

\#fundamentals

A program or system that [**trains**](https://developers.google.com/machine-learning/glossary#training) a [**model**](https://developers.google.com/machine-learning/glossary#model) from input data. The trained model can make useful predictions from new (never-before-seen) data drawn from the same distribution as the one used to train the model.

Machine learning also refers to the field of study concerned with these programs or systems.

## majority class

\#fundamentals

The more common label in a [**class-imbalanced dataset**](https://developers.google.com/machine-learning/glossary#class_imbalanced_data_set). For example, given a dataset containing 99% negative labels and 1% positive labels, the negative labels are the majority class.

Contrast with [**minority class**](https://developers.google.com/machine-learning/glossary#minority_class).

## Markov decision process (MDP)

\#rl

A graph representing the decision-making model where decisions (or [**actions**](https://developers.google.com/machine-learning/glossary#action)) are taken to navigate a sequence of [**states**](https://developers.google.com/machine-learning/glossary#state) under the assumption that the [**Markov property**](https://developers.google.com/machine-learning/glossary#Markov_property) holds. In [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning), these transitions between states return a numerical [**reward**](https://developers.google.com/machine-learning/glossary#reward).

## Markov property

\#rl

A property of certain [**environments**](https://developers.google.com/machine-learning/glossary#environment), where state transitions are entirely determined by information implicit in the current [**state**](https://developers.google.com/machine-learning/glossary#state) and the agent’s [**action**](https://developers.google.com/machine-learning/glossary#action).

## masked language model

\#language

A [**language model**](https://developers.google.com/machine-learning/glossary#language-model) that predicts the probability of candidate tokens to fill in blanks in a sequence. For instance, a masked language model can calculate probabilities for candidate word(s) to replace the underline in the following sentence:

> The ____ in the hat came back.

The literature typically uses the string "MASK" instead of an underline. For example:

> The "MASK" in the hat came back.

Most modern masked language models are [**bidirectional**](https://developers.google.com/machine-learning/glossary#bidirectional).

## matplotlib

An open-source Python 2D plotting library. [matplotlib](https://matplotlib.org/) helps you visualize different aspects of machine learning.

## matrix factorization

\#recsystems

In math, a mechanism for finding the matrices whose dot product approximates a target matrix.

In [**recommendation systems**](https://developers.google.com/machine-learning/glossary#recommendation_system), the target matrix often holds users' ratings on [**items**](https://developers.google.com/machine-learning/glossary#items). For example, the target matrix for a movie recommendation system might look something like the following, where the positive integers are user ratings and 0 means that the user didn't rate the movie:

|   |   |   |   |   |   |
|---|---|---|---|---|---|
||Casablanca|The Philadelphia Story|Black Panther|Wonder Woman|Pulp Fiction|
|User 1|5.0|3.0|0.0|2.0|0.0|
|User 2|4.0|0.0|0.0|1.0|5.0|
|User 3|3.0|1.0|4.0|5.0|0.0|

The movie recommendation system aims to predict user ratings for unrated movies. For example, will User 1 like _Black Panther_?

One approach for recommendation systems is to use matrix factorization to generate the following two matrices:

- A [**user matrix**](https://developers.google.com/machine-learning/glossary#user_matrix), shaped as the number of users X the number of embedding dimensions.
- An [**item matrix**](https://developers.google.com/machine-learning/glossary#item_matrix), shaped as the number of embedding dimensions X the number of items.

For example, using matrix factorization on our three users and five items could yield the following user matrix and item matrix:

```Plain
User Matrix                 Item Matrix1.1   2.3           0.9   0.2   1.4    2.0   1.20.6   2.0           1.7   1.2   1.2   -0.1   2.12.5   0.5
```

The dot product of the user matrix and item matrix yields a recommendation matrix that contains not only the original user ratings but also predictions for the movies that each user hasn't seen. For example, consider User 1's rating of _Casablanca_, which was 5.0. The dot product corresponding to that cell in the recommendation matrix should hopefully be around 5.0, and it is:

```Plain
(1.1 * 0.9) + (2.3 * 1.7) = 4.9
```

More importantly, will User 1 like _Black Panther_? Taking the dot product corresponding to the first row and the third column yields a predicted rating of 4.3:

```Plain
(1.1 * 1.4) + (2.3 * 1.2) = 4.3
```

Matrix factorization typically yields a user matrix and item matrix that, together, are significantly more compact than the target matrix.

## Mean Absolute Error (MAE)

The average loss per example when [**L**](https://developers.google.com/machine-learning/glossary#L1_loss)[**1**](https://developers.google.com/machine-learning/glossary#L1_loss) [**loss**](https://developers.google.com/machine-learning/glossary#L1_loss) is used. Calculate Mean Absolute Error as follows:

1. Calculate the L loss for a batch.
    
    1
    
2. Divide the L loss by the number of examples in the batch.
    
    1
    

### Click the icon to see the formal math.

For example, consider the calculation of L1 loss on the following batch of five examples:

|   |   |   |
|---|---|---|
|Actual value of example|Model's predicted value|Loss (difference between actual and predicted)|
|7|6|1|
|5|4|1|
|8|11|3|
|4|6|2|
|9|8|1|
|||8 = L1 loss|

So, L1 loss is 8 and the number of examples is 5. Therefore, the Mean Absolute Error is:

```Plain
Mean Absolute Error = L1 loss / Number of Examples
Mean Absolute Error = 8/5 = 1.6
```

Contrast Mean Absolute Error with [**Mean Squared Error**](https://developers.google.com/machine-learning/glossary#MSE) and [**Root Mean Squared Error**](https://developers.google.com/machine-learning/glossary#RMSE).

## Mean Squared Error (MSE)

The average loss per example when [**L**](https://developers.google.com/machine-learning/glossary#L2_loss)[**2**](https://developers.google.com/machine-learning/glossary#L2_loss) [**loss**](https://developers.google.com/machine-learning/glossary#L2_loss) is used. Calculate Mean Squared Error as follows:

1. Calculate the L loss for a batch.
    
    2
    
2. Divide the L loss by the number of examples in the batch.
    
    2
    

### Click the icon to see the formal math.

For example, consider the loss on the following batch of five examples:

|   |   |   |   |
|---|---|---|---|
|Actual value|Model's prediction|Loss|Squared loss|
|7|6|1|1|
|5|4|1|1|
|8|11|3|9|
|4|6|2|4|
|9|8|1|1|
||||16 = L2 loss|

Therefore, the Mean Squared Error is:

```Plain
Mean Squared Error = L2 loss / Number of Examples
Mean Squared Error = 16/5 = 3.2
```

Mean Squared Error is a popular training [**optimizer**](https://developers.google.com/machine-learning/glossary#optimizer), particularly for [**linear regression**](https://developers.google.com/machine-learning/glossary#linear_regression).

Contrast Mean Squared Error with [**Mean Absolute Error**](https://developers.google.com/machine-learning/glossary#MAE) and [**Root Mean Squared Error**](https://developers.google.com/machine-learning/glossary#RMSE).

[**TensorFlow Playground**](https://developers.google.com/machine-learning/glossary#TensorFlow_Playground) uses Mean Squared Error to calculate loss values.

### Click the icon to see more details about outliers.

## metric

\#TensorFlow

A statistic that you care about.

An [**objective**](https://developers.google.com/machine-learning/glossary#objective) is a metric that a machine learning system tries to optimize.

## meta-learning

\#language

A subset of machine learning that discovers or improves a learning algorithm. A meta-learning system can also aim to train a model to quickly learn a new task from a small amount of data or from experience gained in previous tasks. Meta-learning algorithms generally try to achieve the following:

- Improve/learn hand-engineered features (such as an initializer or an optimizer).
- Be more data-efficient and compute-efficient.
- Improve generalization.

Meta-learning is related to [**few-shot learning**](https://developers.google.com/machine-learning/glossary#few-shot_learning).

## Metrics API (tf.metrics)

A TensorFlow API for evaluating models. For example, `tf.metrics.accuracy` determines how often a model's predictions match labels.

## mini-batch

\#fundamentals

A small, randomly selected subset of a [**batch**](https://developers.google.com/machine-learning/glossary#batch) processed in one [**iteration**](https://developers.google.com/machine-learning/glossary#iteration). The [**batch size**](https://developers.google.com/machine-learning/glossary#batch_size) of a mini-batch is usually between 10 and 1,000 examples.

For example, suppose the entire training set (the full batch) consists of 1,000 examples. Further suppose that you set the [**batch size**](https://developers.google.com/machine-learning/glossary#batch_size) of each mini-batch to 20. Therefore, each iteration determines the loss on a random 20 of the 1,000 examples and then adjusts the [**weights**](https://developers.google.com/machine-learning/glossary#weight) and [**biases**](https://developers.google.com/machine-learning/glossary#bias) accordingly.

It is much more efficient to calculate the loss on a mini-batch than the loss on all the examples in the full batch.

## mini-batch stochastic gradient descent

A [**gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent) algorithm that uses [**mini-batches**](https://developers.google.com/machine-learning/glossary#mini-batch). In other words, mini-batch stochastic gradient descent estimates the gradient based on a small subset of the training data. Regular [**stochastic gradient descent**](https://developers.google.com/machine-learning/glossary#SGD) uses a mini-batch of size 1.

## minimax loss

A loss function for [**generative adversarial networks**](https://developers.google.com/machine-learning/glossary#generative_adversarial_network), based on the [**cross-entropy**](https://developers.google.com/machine-learning/glossary#cross-entropy) between the distribution of generated data and real data.

Minimax loss is used in the [first paper](https://arxiv.org/pdf/1406.2661.pdf) to describe generative adversarial networks.

## minority class

\#fundamentals

The less common label in a [**class-imbalanced dataset**](https://developers.google.com/machine-learning/glossary#class_imbalanced_data_set). For example, given a dataset containing 99% negative labels and 1% positive labels, the positive labels are the minority class.

Contrast with [**majority class**](https://developers.google.com/machine-learning/glossary#majority_class).

### Click the icon for additional notes.

## ML

Abbreviation for [**machine learning**](https://developers.google.com/machine-learning/glossary#machine_learning).

## MNIST

\#image

A public-domain dataset compiled by LeCun, Cortes, and Burges containing 60,000 images, each image showing how a human manually wrote a particular digit from 0–9. Each image is stored as a 28x28 array of integers, where each integer is a grayscale value between 0 and 255, inclusive.

MNIST is a canonical dataset for machine learning, often used to test new machine learning approaches. For details, see [The MNIST Database of Handwritten Digits](http://yann.lecun.com/exdb/mnist/).

## modality

\#language

A high-level data category. For example, numbers, text, images, video, and audio are five different modalities.

## model

\#fundamentals

In general, any mathematical construct that processes input data and returns output. Phrased differently, a model is the set of parameters and structure needed for a system to make predictions. In [**supervised machine learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning), a model takes an [**example**](https://developers.google.com/machine-learning/glossary#example) as input and infers a [**prediction**](https://developers.google.com/machine-learning/glossary#prediction) as output. Within supervised machine learning, models differ somewhat. For example:

- A linear regression model consists of a set of [**weights**](https://developers.google.com/machine-learning/glossary#weight) and a [**bias**](https://developers.google.com/machine-learning/glossary#bias).
- A [**neural network**](https://developers.google.com/machine-learning/glossary#neural-network) model consists of:
    - A set of [**hidden layers**](https://developers.google.com/machine-learning/glossary#hidden_layer), each containing one or more [**neurons**](https://developers.google.com/machine-learning/glossary#neuron).
    - The weights and bias associated with each neuron.
- A [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree) model consists of:
    - The shape of the tree; that is, the pattern in which the conditions and leaves are connected.
    - The conditions and leaves.

You can save, restore, or make copies of a model.

[**Unsupervised machine learning**](https://developers.google.com/machine-learning/glossary#unsupervised_machine_learning) also generates models, typically a function that can map an input example to the most appropriate [**cluster**](https://developers.google.com/machine-learning/glossary#clustering).

### Click the icon to compare algebraic and programming functions to ML models.

## model capacity

The complexity of problems that a model can learn. The more complex the problems that a model can learn, the higher the model’s capacity. A model’s capacity typically increases with the number of model parameters. For a formal definition of classifier capacity, see [VC dimension](https://wikipedia.org/wiki/VC_dimension).

## model parallelism

\#language

A way of scaling training or inference that puts different parts of one model on different devices. Model parallelism enables models that are too big to fit on a single device.

See also [**data parallelism**](https://developers.google.com/machine-learning/glossary#data-parallelism).

## model training

The process of determining the best [**model**](https://developers.google.com/machine-learning/glossary#model).

## Momentum

A sophisticated gradient descent algorithm in which a learning step depends not only on the derivative in the current step, but also on the derivatives of the step(s) that immediately preceded it. Momentum involves computing an exponentially weighted moving average of the gradients over time, analogous to momentum in physics. Momentum sometimes prevents learning from getting stuck in local minima.

## multi-class classification

\#fundamentals

In supervised learning, a [**classification**](https://developers.google.com/machine-learning/glossary#classification_model) problem in which the dataset contains _more than two_ [**classes**](https://developers.google.com/machine-learning/glossary#class) of labels. For example, the labels in the Iris dataset must be one of the following three classes:

- Iris setosa
- Iris virginica
- Iris versicolor

A model trained on the Iris dataset that predicts Iris type on new examples is performing multi-class classification.

In contrast, classification problems that distinguish between exactly two classes are [**binary classification models**](https://developers.google.com/machine-learning/glossary#binary_classification). For example, an email model that predicts either _spam_ or _not spam_ is a binary classification model.

In clustering problems, multi-class classification refers to more than two clusters.

## multi-class logistic regression

Using [**logistic regression**](https://developers.google.com/machine-learning/glossary#logistic_regression) in [**multi-class classification**](https://developers.google.com/machine-learning/glossary#multi-class) problems.

## multi-head self-attention

\#language

An extension of [**self-attention**](https://developers.google.com/machine-learning/glossary#self-attention) that applies the self-attention mechanism multiple times for each position in the input sequence.

[**Transformers**](https://developers.google.com/machine-learning/glossary#Transformer) introduced multi-head self-attention.

## multimodal model

\#language

A model whose inputs and/or outputs include more than one [**modality**](https://developers.google.com/machine-learning/glossary#modality). For example, consider a model that takes both an image and a text caption (two modalities) as [**features**](https://developers.google.com/machine-learning/glossary#feature), and outputs a score indicating how appropriate the text caption is for the image. So, this model's inputs are multimodal and the output is unimodal.

## multinomial classification

Synonym for [**multi-class classification**](https://developers.google.com/machine-learning/glossary#multi-class).

## multinomial regression

Synonym for [**multi-class logistic regression**](https://developers.google.com/machine-learning/glossary#multi-class_logistic_regression).

## multitask

A machine learning technique in which a single [**model**](https://developers.google.com/machine-learning/glossary#model) is trained to perform multiple [**tasks**](https://developers.google.com/machine-learning/glossary#task).

Multitask models are created by training on data that is appropriate for each of the different tasks. This allows the model to learn to share information across the tasks, which helps the model learn more effectively.

A model trained for multiple tasks often has improved generalization abilities and can be more robust at handling different types of data.

## N

## NaN trap

When one number in your model becomes a [NaN](https://wikipedia.org/wiki/NaN) during training, which causes many or all other numbers in your model to eventually become a NaN.

NaN is an abbreviation for **N**ot **a** **N**umber.

## natural language understanding

\#language

Determining a user's intentions based on what the user typed or said. For example, a search engine uses natural language understanding to determine what the user is searching for based on what the user typed or said.

## negative class

\#fundamentals

In [**binary classification**](https://developers.google.com/machine-learning/glossary#binary_classification), one class is termed _positive_ and the other is termed _negative_. The positive class is the thing or event that the model is testing for and the negative class is the other possibility. For example:

- The negative class in a medical test might be "not tumor."
- The negative class in an email classifier might be "not spam."

Contrast with [**positive class**](https://developers.google.com/machine-learning/glossary#positive_class).

## negative sampling

Synonym for [**candidate sampling**](https://developers.google.com/machine-learning/glossary#candidate_sampling).

## Neural Architecture Search (NAS)

A technique for automatically designing the architecture of a [**neural network**](https://developers.google.com/machine-learning/glossary#neural-network). NAS algorithms can reduce the amount of time and resources required to train a neural network.

NAS typically uses:

- A search space, which is a set of possible architectures.
- A fitness function, which is a measure of how well a particular architecture performs on a given task.

NAS algorithms often start with a small set of possible architectures and gradually expand the search space as the algorithm learns more about what architectures are effective. The fitness function is typically based on the performance of the architecture on a training set, and the algorithm is typically trained using a [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning) technique.

NAS algorithms have proven effective in finding high-performing architectures for a variety of tasks, including image [**classification**](https://developers.google.com/machine-learning/glossary#classification_model), text classification, and machine translation.

## neural network

\#fundamentals

A [**model**](https://developers.google.com/machine-learning/glossary#model) containing at least one [**hidden layer**](https://developers.google.com/machine-learning/glossary#hidden_layer). A [**deep neural network**](https://developers.google.com/machine-learning/glossary#deep_neural_network) is a type of neural network containing more than one hidden layer. For example, the following diagram shows a deep neural network containing two hidden layers.

Each neuron in a neural network connects to all of the nodes in the next layer. For example, in the preceding diagram, notice that each of the three neurons in the first hidden layer separately connect to both of the two neurons in the second hidden layer.

Neural networks implemented on computers are sometimes called **artificial neural networks** to differentiate them from neural networks found in brains and other nervous systems.

Some neural networks can mimic extremely complex nonlinear relationships between different features and the label.

See also [**convolutional neural network**](https://developers.google.com/machine-learning/glossary#convolutional_neural_network) and [**recurrent neural network**](https://developers.google.com/machine-learning/glossary#recurrent_neural_network).

## neuron

\#fundamentals

In machine learning, a distinct unit within a [**hidden layer**](https://developers.google.com/machine-learning/glossary#hidden_layer) of a [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network). Each neuron performs the following two-step action:

1. Calculates the [**weighted sum**](https://developers.google.com/machine-learning/glossary#weighted_sum) of input values multiplied by their corresponding weights.
2. Passes the weighted sum as input to an [**activation function**](https://developers.google.com/machine-learning/glossary#activation_function).

A neuron in the first hidden layer accepts inputs from the feature values in the [**input layer**](https://developers.google.com/machine-learning/glossary#input_layer). A neuron in any hidden layer beyond the first accepts inputs from the neurons in the preceding hidden layer. For example, a neuron in the second hidden layer accepts inputs from the neurons in the first hidden layer.

The following illustration highlights two neurons and their inputs.

A neuron in a neural network mimics the behavior of neurons in brains and other parts of nervous systems.

## N-gram

\#seq

\#language

An ordered sequence of N words. For example, _truly madly_ is a 2-gram. Because order is relevant, _madly truly_ is a different 2-gram than _truly madly_.

|   |   |   |
|---|---|---|
|N|Name(s) for this kind of N-gram|Examples|
|2|bigram or 2-gram|_to go, go to, eat lunch, eat dinner_|
|3|trigram or 3-gram|_ate too much, three blind mice, the bell tolls_|
|4|4-gram|_walk in the park, dust in the wind, the boy ate lentils_|

Many [**natural language understanding**](https://developers.google.com/machine-learning/glossary#natural_language_understanding) models rely on N-grams to predict the next word that the user will type or say. For example, suppose a user typed _three blind_. An NLU model based on trigrams would likely predict that the user will next type _mice_.

Contrast N-grams with [**bag of words**](https://developers.google.com/machine-learning/glossary#bag_of_words), which are unordered sets of words.

## NLU

\#language

Abbreviation for [**natural language understanding**](https://developers.google.com/machine-learning/glossary#natural_language_understanding).

## node (neural network)

\#fundamentals

A [**neuron**](https://developers.google.com/machine-learning/glossary#neuron) in a [**hidden layer**](https://developers.google.com/machine-learning/glossary#hidden_layer).

## node (TensorFlow graph)

\#TensorFlow

An operation in a TensorFlow [**graph**](https://developers.google.com/machine-learning/glossary#graph).

## node (decision tree)

\#df

In a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree), any [**condition**](https://developers.google.com/machine-learning/glossary#condition) or [**leaf**](https://developers.google.com/machine-learning/glossary#leaf).

## noise

Broadly speaking, anything that obscures the signal in a dataset. Noise can be introduced into data in a variety of ways. For example:

- Human raters make mistakes in labeling.
- Humans and instruments mis-record or omit feature values.

## non-binary condition

\#df

A [**condition**](https://developers.google.com/machine-learning/glossary#condition) containing more than two possible outcomes. For example, the following non-binary condition contains three possible outcomes:

## nonlinear

\#fundamentals

A relationship between two or more variables that can't be represented solely through addition and multiplication. A _linear_ relationship can be represented as a line; a _nonlinear_ relationship can't be represented as a line. For example, consider two models that each relate a single feature to a single label. The model on the left is linear and the model on the right is nonlinear:

## non-response bias

\#fairness

See [**selection bias**](https://developers.google.com/machine-learning/glossary#selection_bias).

## nonstationarity

\#fundamentals

A feature whose values change across one or more dimensions, usually time. For example, consider the following examples of nonstationarity:

- The number of swimsuits sold at a particular store varies with the season.
- The quantity of a particular fruit harvested in a particular region is zero for much of the year but large for a brief period.
- Due to climate change, annual mean temperatures are shifting.

Contrast with [**stationarity**](https://developers.google.com/machine-learning/glossary#stationarity).

## normalization

\#fundamentals

Broadly speaking, the process of converting a variable's actual range of values into a standard range of values, such as:

- 1 to +1
- 0 to 1
- the normal distribution

For example, suppose the actual range of values of a certain feature is 800 to 2,400. As part of [**feature engineering**](https://developers.google.com/machine-learning/glossary#feature_engineering), you could normalize the actual values down to a standard range, such as -1 to +1.

Normalization is a common task in [**feature engineering**](https://developers.google.com/machine-learning/glossary#feature_engineering). Models usually train faster (and produce better predictions) when every numerical feature in the [**feature vector**](https://developers.google.com/machine-learning/glossary#feature_vector) has roughly the same range.

## novelty detection

The process of determining whether a new (novel) example comes from the same distribution as the [**training set**](https://developers.google.com/machine-learning/glossary#training_set). In other words, after training on the training set, novelty detection determines whether a _new_ example (during inference or during additional training) is an [**outlier**](https://developers.google.com/machine-learning/glossary#outliers).

Contrast with [**outlier detection**](https://developers.google.com/machine-learning/glossary#outlier-detection).

## numerical data

\#fundamentals

[**Features**](https://developers.google.com/machine-learning/glossary#feature) represented as integers or real-valued numbers. For example, a house valuation model would probably represent the size of a house (in square feet or square meters) as numerical data. Representing a feature as numerical data indicates that the feature's values have a _mathematical_ relationship to the label. That is, the number of square meters in a house probably has some mathematical relationship to the value of the house.

Not all integer data should be represented as numerical data. For example, postal codes in some parts of the world are integers; however, integer postal codes should not be represented as numerical data in models. That's because a postal code of `20000` is not twice (or half) as potent as a postal code of 10000. Furthermore, although different postal codes _do_ correlate to different real estate values, we can't assume that real estate values at postal code 20000 are twice as valuable as real estate values at postal code 10000. Postal codes should be represented as [**categorical data**](https://developers.google.com/machine-learning/glossary#categorical_data) instead.

Numerical features are sometimes called [**continuous features**](https://developers.google.com/machine-learning/glossary#continuous_feature).

## NumPy

An [open-source math library](http://www.numpy.org/) that provides efficient array operations in Python. [**pandas**](https://developers.google.com/machine-learning/glossary#pandas) is built on NumPy.

## O

## objective

A metric that your algorithm is trying to optimize.

## objective function

The mathematical formula or [**metric**](https://developers.google.com/machine-learning/glossary#metric) that a model aims to optimize. For example, the objective function for [**linear regression**](https://developers.google.com/machine-learning/glossary#linear_regression) is usually [**Mean Squared Loss**](https://developers.google.com/machine-learning/glossary#MSE). Therefore, when training a linear regression model, training aims to minimize Mean Squared Loss.

In some cases, the goal is to _maximize_ the objective function. For example, if the objective function is accuracy, the goal is to maximize accuracy.

See also [**loss**](https://developers.google.com/machine-learning/glossary#loss).

## oblique condition

\#df

In a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree), a [**condition**](https://developers.google.com/machine-learning/glossary#condition) that involves more than one [**feature**](https://developers.google.com/machine-learning/glossary#feature). For example, if height and width are both features, then the following is an oblique condition:

```Plain
  height > width
```

Contrast with [**axis-aligned condition**](https://developers.google.com/machine-learning/glossary#axis-aligned-condition).

## offline

\#fundamentals

Synonym for [**static**](https://developers.google.com/machine-learning/glossary#static).

## offline inference

\#fundamentals

The process of a model generating a batch of [**predictions**](https://developers.google.com/machine-learning/glossary#prediction) and then caching (saving) those predictions. Apps can then access the desired prediction from the cache rather than rerunning the model.

For example, consider a model that generates local weather forecasts (predictions) once every four hours. After each model run, the system caches all the local weather forecasts. Weather apps retrieve the forecasts from the cache.

Offline inference is also called **static inference**.

Contrast with [**online inference**](https://developers.google.com/machine-learning/glossary#online_inference).

## one-hot encoding

\#fundamentals

Representing categorical data as a vector in which:

- One element is set to 1.
- All other elements are set to 0.

One-hot encoding is commonly used to represent strings or identifiers that have a finite set of possible values. For example, suppose a certain categorical feature named `Scandinavia` has five possible values:

- "Denmark"
- "Sweden"
- "Norway"
- "Finland"
- "Iceland"

One-hot encoding could represent each of the five values as follows:

|   |   |   |   |   |   |
|---|---|---|---|---|---|
|country|Vector|||||
|"Denmark"|1|0|0|0|0|
|"Sweden"|0|1|0|0|0|
|"Norway"|0|0|1|0|0|
|"Finland"|0|0|0|1|0|
|"Iceland"|0|0|0|0|1|

Thanks to one-hot encoding, a model can learn different connections based on each of the five countries.

Representing a feature as [**numerical data**](https://developers.google.com/machine-learning/glossary#numerical_data) is an alternative to one-hot encoding. Unfortunately, representing the Scandinavian countries numerically is not a good choice. For example, consider the following numeric representation:

- "Denmark" is 0
- "Sweden" is 1
- "Norway" is 2
- "Finland" is 3
- "Iceland" is 4

With numeric encoding, a model would interpret the raw numbers mathematically and would try to train on those numbers. However, Iceland isn't actually twice as much (or half as much) of something as Norway, so the model would come to some strange conclusions.

## one-shot learning

A machine learning approach, often used for object classification, designed to learn effective classifiers from a single training example.

See also [**few-shot learning**](https://developers.google.com/machine-learning/glossary#few-shot_learning) and [**zero-shot learning**](https://developers.google.com/machine-learning/glossary#zero-shot-learning).

## one-vs.-all

\#fundamentals

Given a classification problem with N classes, a solution consisting of N separate [**binary classifiers**](https://developers.google.com/machine-learning/glossary#binary_classification)—one binary classifier for each possible outcome. For example, given a model that classifies examples as animal, vegetable, or mineral, a one-vs.-all solution would provide the following three separate binary classifiers:

- animal vs. not animal
- vegetable vs. not vegetable
- mineral vs. not mineral

## online

\#fundamentals

Synonym for [**dynamic**](https://developers.google.com/machine-learning/glossary#dynamic).

## online inference

\#fundamentals

Generating [**predictions**](https://developers.google.com/machine-learning/glossary#prediction) on demand. For example, suppose an app passes input to a model and issues a request for a prediction. A system using online inference responds to the request by running the model (and returning the prediction to the app).

Contrast with [**offline inference**](https://developers.google.com/machine-learning/glossary#offline_inference).

## operation (op)

\#TensorFlow

In TensorFlow, any procedure that creates, manipulates, or destroys a [**Tensor**](https://developers.google.com/machine-learning/glossary#tensor). For example, a matrix multiply is an operation that takes two Tensors as input and generates one Tensor as output.

## Optax

A gradient processing and optimization library for [**JAX**](https://developers.google.com/machine-learning/glossary#JAX). Optax facilitates research by providing building blocks that can be recombined in custom ways to optimize parametric models such as deep neural networks. Other goals include:

- Providing readable, well-tested, efficient implementations of core components.
- Improving productivity by making it possible to combine low level ingredients into custom optimizers (or other gradient processing components).
- Accelerating adoption of new ideas by making it easy for anyone to contribute.

## out-of-bag evaluation (OOB evaluation)

\#df

A mechanism for evaluating the quality of a [**decision forest**](https://developers.google.com/machine-learning/glossary#decision-forest) by testing each [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree) against the [**examples**](https://developers.google.com/machine-learning/glossary#example) _not_ used during [**training**](https://developers.google.com/machine-learning/glossary#training) of that decision tree. For example, in the following diagram, notice that the system trains each decision tree on about two-thirds of the examples and then evaluates against the remaining one-third of the examples.

Out-of-bag evaluation is a computationally efficient and conservative approximation of the [**cross-validation**](https://developers.google.com/machine-learning/glossary#cross-validation) mechanism. In cross-validation, one model is trained for each cross-validation round (for example, 10 models are trained in a 10-fold cross-validation). With OOB evaluation, a single model is trained. Because [**bagging**](https://developers.google.com/machine-learning/glossary#bagging) withholds some data from each tree during training, OOB evaluation can use that data to approximate cross-validation.

## optimizer

A specific implementation of the [**gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent) algorithm. Popular optimizers include:

- [**AdaGrad**](https://developers.google.com/machine-learning/glossary#AdaGrad), which stands for ADAptive GRADient descent.
- Adam, which stands for ADAptive with Momentum.

## out-group homogeneity bias

\#fairness

The tendency to see out-group members as more alike than in-group members when comparing attitudes, values, personality traits, and other characteristics. **In-group** refers to people you interact with regularly; **out-group** refers to people you do not interact with regularly. If you create a dataset by asking people to provide attributes about out-groups, those attributes may be less nuanced and more stereotyped than attributes that participants list for people in their in-group.

For example, Lilliputians might describe the houses of other Lilliputians in great detail, citing small differences in architectural styles, windows, doors, and sizes. However, the same Lilliputians might simply declare that Brobdingnagians all live in identical houses.

Out-group homogeneity bias is a form of [**group attribution bias**](https://developers.google.com/machine-learning/glossary#group_attribution_bias).

See also [**in-group bias**](https://developers.google.com/machine-learning/glossary#in-group_bias).

## outlier detection

The process of identifying [**outliers**](https://developers.google.com/machine-learning/glossary#outliers) in a [**training set**](https://developers.google.com/machine-learning/glossary#training_set).

Contrast with [**novelty detection**](https://developers.google.com/machine-learning/glossary#novelty-detection).

## outliers

Values distant from most other values. In machine learning, any of the following are outliers:

- Input data whose values are more than roughly 3 standard deviations from the mean.
- [**Weights**](https://developers.google.com/machine-learning/glossary#weight) with high absolute values.
- Predicted values relatively far away from the actual values.

For example, suppose that `widget-price` is a feature of a certain model. Assume that the mean `widget-price` is 7 Euros with a standard deviation of 1 Euro. Examples containing a `widget-price` of 12 Euros or 2 Euros would therefore be considered outliers because each of those prices is five standard deviations from the mean.

Outliers are often caused by typos or other input mistakes. In other cases, outliers aren't mistakes; after all, values five standard deviations away from the mean are rare but hardly impossible.

Outliers often cause problems in model training. [**Clipping**](https://developers.google.com/machine-learning/glossary#clipping) is one way of managing outliers.

## output layer

\#fundamentals

The "final" layer of a neural network. The output layer contains the prediction.

The following illustration shows a small deep neural network with an input layer, two hidden layers, and an output layer:

## overfitting

\#fundamentals

Creating a [**model**](https://developers.google.com/machine-learning/glossary#model) that matches the [**training data**](https://developers.google.com/machine-learning/glossary#training_set) so closely that the model fails to make correct predictions on new data.

[**Regularization**](https://developers.google.com/machine-learning/glossary#regularization) can reduce overfitting. Training on a large and diverse training set can also reduce overfitting.

### Click the icon for additional notes.

## oversampling

Reusing the [**examples**](https://developers.google.com/machine-learning/glossary#example) of a [**minority class**](https://developers.google.com/machine-learning/glossary#minority_class) in a [**class-imbalanced dataset**](https://developers.google.com/machine-learning/glossary#class_imbalanced_data_set) in order to create a more balanced [**training set**](https://developers.google.com/machine-learning/glossary#training_set).

For example, consider a [**binary classification**](https://developers.google.com/machine-learning/glossary#binary_classification) problem in which the ratio of the [**majority class**](https://developers.google.com/machine-learning/glossary#majority_class) to the minority class is 5,000:1. If the dataset contains a million examples, then the dataset contains only about 200 examples of the minority class, which might be too few examples for effective training. To overcome this deficiency, you might oversample (reuse) those 200 examples multiple times, possibly yielding sufficient examples for useful training.

You need to be careful about over [**overfitting**](https://developers.google.com/machine-learning/glossary#overfitting) when oversampling.

Contrast with [**undersampling**](https://developers.google.com/machine-learning/glossary#undersampling).

## P

## packed data

An approach for storing data more efficiently.

Packed data stores data either by using a compressed format or in some other way that allows it to be accessed more efficiently. Packed data minimizes the amount of memory and computation required to access it, leading to faster training and more efficient model inference.

Packed data is often used with other techniques, such as [**data augmentation**](https://developers.google.com/machine-learning/glossary#data_augmentation) and [**regularization**](https://developers.google.com/machine-learning/glossary#regularization), further improving the performance of [**models**](https://developers.google.com/machine-learning/glossary#model).

## pandas

\#fundamentals

A column-oriented data analysis API built on top of [**numpy**](https://developers.google.com/machine-learning/glossary#numpy). Many machine learning frameworks, including TensorFlow, support pandas data structures as inputs. See the [pandas documentation](http://pandas.pydata.org/) for details.

## parameter

\#fundamentals

The [**weights**](https://developers.google.com/machine-learning/glossary#weight) and [**biases**](https://developers.google.com/machine-learning/glossary#bias) that a model learns during [**training**](https://developers.google.com/machine-learning/glossary#training). For example, in a [**linear regression**](https://developers.google.com/machine-learning/glossary#linear_regression) model, the parameters consist of the bias (_b_) and all the weights (_w__1_, _w__2_, and so on) in the following formula:

y′=b+w1x1+w2x2+…wnxn

In contrast, [**hyperparameter**](https://developers.google.com/machine-learning/glossary#hyperparameter) are the values that _you_ (or a hyperparameter turning service) supply to the model. For example, [**learning rate**](https://developers.google.com/machine-learning/glossary#learning_rate) is a hyperparameter.

## Parameter Server (PS)

\#TensorFlow

A job that keeps track of a model's [**parameters**](https://developers.google.com/machine-learning/glossary#parameter) in a distributed setting.

## parameter update

The operation of adjusting a model's [**parameters**](https://developers.google.com/machine-learning/glossary#parameter) during training, typically within a single iteration of [**gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent).

## partial derivative

A derivative in which all but one of the variables is considered a constant. For example, the partial derivative of _f(x, y)_ with respect to _x_ is the derivative of _f_ considered as a function of _x_ alone (that is, keeping _y_ constant). The partial derivative of _f_ with respect to _x_ focuses only on how _x_ is changing and ignores all other variables in the equation.

## participation bias

\#fairness

Synonym for non-response bias. See [**selection bias**](https://developers.google.com/machine-learning/glossary#selection_bias).

## partitioning strategy

The algorithm by which variables are divided across [**parameter servers**](https://developers.google.com/machine-learning/glossary#Parameter_Server).

## Pax

A programming framework designed for training large-scale [**neural network**](https://developers.google.com/machine-learning/glossary#neural-network) [**models**](https://developers.google.com/machine-learning/glossary#model) so large that they span multiple [**TPU**](https://developers.google.com/machine-learning/glossary#TPU) [**accelerator chip**](https://developers.google.com/machine-learning/glossary#accelerator-chip) [**slices**](https://developers.google.com/machine-learning/glossary#TPU_slice) or [**pods**](https://developers.google.com/machine-learning/glossary#TPU_Pod).

Pax is built on [**Flax**](https://developers.google.com/machine-learning/glossary#flax), which is built on [**JAX**](https://developers.google.com/machine-learning/glossary#JAX).

## perceptron

A system (either hardware or software) that takes in one or more input values, runs a function on the weighted sum of the inputs, and computes a single output value. In machine learning, the function is typically nonlinear, such as [**ReLU**](https://developers.google.com/machine-learning/glossary#ReLU), [**sigmoid**](https://developers.google.com/machine-learning/glossary#sigmoid-function), or [tanh](https://wikipedia.org/wiki/Hyperbolic_functions). For example, the following perceptron relies on the sigmoid function to process three input values:

f(x1,x2,x3)=sigmoid(w1x1+w2x2+w3x3)

In the following illustration, the perceptron takes three inputs, each of which is itself modified by a weight before entering the perceptron:

Perceptrons are the [**neurons**](https://developers.google.com/machine-learning/glossary#neuron) in [**neural networks**](https://developers.google.com/machine-learning/glossary#neural-network).

## performance

Overloaded term with the following meanings:

- The traditional meaning within software engineering. Namely: How fast (or efficiently) does this piece of software run?
- The meaning within machine learning. Here, performance answers the following question: How correct is this [**model**](https://developers.google.com/machine-learning/glossary#model)? That is, how good are the model's predictions?

## permutation variable importances

\#df

A type of [**variable importance**](https://developers.google.com/machine-learning/glossary#variable-importances) that evaluates the increase in the prediction error of a model _after_ permuting the feature’s values. Permutation variable importance is a model agnostic metric.

## perplexity

One measure of how well a [**model**](https://developers.google.com/machine-learning/glossary#model) is accomplishing its task. For example, suppose your task is to read the first few letters of a word a user is typing on a smartphone keyboard, and to offer a list of possible completion words. Perplexity, P, for this task is approximately the number of guesses you need to offer in order for your list to contain the actual word the user is trying to type.

Perplexity is related to [**cross-entropy**](https://developers.google.com/machine-learning/glossary#cross-entropy) as follows:

P=2−cross entropy

## pipeline

The infrastructure surrounding a machine learning algorithm. A pipeline includes gathering the data, putting the data into training data files, training one or more models, and exporting the models to production.

## pipelining

\#language

A form of [**model parallelism**](https://developers.google.com/machine-learning/glossary#model-parallelism) in which a model's processing is divided into consecutive stages and each stage is executed on a different device. While a stage is processing one batch, the preceding stage can work on the next batch.

See also [**staged training**](https://developers.google.com/machine-learning/glossary#staged-training).

## pjit

A [**JAX**](https://developers.google.com/machine-learning/glossary#JAX) function that splits code to run across multiple [**accelerator chips**](https://developers.google.com/machine-learning/glossary#accelerator-chip). The user passes a function to pjit, which returns a function that has the equivalent semantics but is compiled into an [**XLA**](https://developers.google.com/machine-learning/glossary#XLA) computation that runs across multiple devices (such as GPUs or [**TPU**](https://developers.google.com/machine-learning/glossary#TPU) cores).

pjit enables users to shard computations without rewriting them by using the [**SPMD**](https://developers.google.com/machine-learning/glossary#single-program) partitioner.

As of March 2023, `pjit` has been merged with `jit`. Refer to [Distributed arrays and automatic parallelization](https://jax.readthedocs.io/en/latest/notebooks/Distributed_arrays_and_automatic_parallelization.html) for more details.

## pmap

A [**JAX**](https://developers.google.com/machine-learning/glossary#JAX) function that executes copies of an input function on multiple underlying hardware devices (CPUs, GPUs, or [**TPUs**](https://developers.google.com/machine-learning/glossary#TPU)), with different input values. pmap relies on [**SPMD**](https://developers.google.com/machine-learning/glossary#single-program).

## policy

\#rl

In reinforcement learning, an [**agent's**](https://developers.google.com/machine-learning/glossary#agent) probabilistic mapping from [**states**](https://developers.google.com/machine-learning/glossary#state) to [**actions**](https://developers.google.com/machine-learning/glossary#action).

## pooling

\#image

Reducing a matrix (or matrices) created by an earlier [**convolutional layer**](https://developers.google.com/machine-learning/glossary#convolutional_layer) to a smaller matrix. Pooling usually involves taking either the maximum or average value across the pooled area. For example, suppose we have the following 3x3 matrix:

A pooling operation, just like a convolutional operation, divides that matrix into slices and then slides that convolutional operation by [**strides**](https://developers.google.com/machine-learning/glossary#stride). For example, suppose the pooling operation divides the convolutional matrix into 2x2 slices with a 1x1 stride. As the following diagram illustrates, four pooling operations take place. Imagine that each pooling operation picks the maximum value of the four in that slice:

Pooling helps enforce [**translational invariance**](https://developers.google.com/machine-learning/glossary#translational_invariance) in the input matrix.

Pooling for vision applications is known more formally as **spatial pooling**. Time-series applications usually refer to pooling as **temporal pooling**. Less formally, pooling is often called **subsampling** or **downsampling**.

## positional encoding

\#language

A technique to add information about the _position_ of a token in a sequence to the token's embedding. [**Transformer models**](https://developers.google.com/machine-learning/glossary#transformer) use positional encoding to better understand the relationship between different parts of the sequence.

A common implementation of positional encoding uses a sinusoidal function. (Specifically, the frequency and amplitude of the sinusoidal function are determined by the position of the token in the sequence.) This technique enables a Transformer model to learn to attend to different parts of the sequence based on their position.

## positive class

\#fundamentals

The class you are testing for.

For example, the positive class in a cancer model might be "tumor." The positive class in an email classifier might be "spam."

Contrast with [**negative class**](https://developers.google.com/machine-learning/glossary#negative_class).

### Click the icon for additional notes.

## post-processing

\#fairness

\#fundamentals

Adjusting the output of a model _after_ the model has been run. Post-processing can be used to enforce fairness constraints without modifying models themselves.

For example, one might apply post-processing to a binary classifier by setting a classification threshold such that [**equality of opportunity**](https://developers.google.com/machine-learning/glossary#equality_of_opportunity) is maintained for some attribute by checking that the [**true positive rate**](https://developers.google.com/machine-learning/glossary#TP_rate) is the same for all values of that attribute.

## PR AUC (area under the PR curve)

Area under the interpolated [**precision-recall curve**](https://developers.google.com/machine-learning/glossary#precision-recall_curve), obtained by plotting (recall, precision) points for different values of the [**classification threshold**](https://developers.google.com/machine-learning/glossary#classification_threshold). Depending on how it's calculated, PR AUC may be equivalent to the [**average precision**](https://developers.google.com/machine-learning/glossary#average_precision) of the model.

## Praxis

A core, high-performance ML library of [**Pax**](https://developers.google.com/machine-learning/glossary#pax). Praxis is often called the "Layer library".

Praxis contains not just the definitions for the Layer class, but most of its supporting components as well, including:

- data inputs
- configuration libraries (HParam and [**Fiddle**](https://developers.google.com/machine-learning/glossary#fiddle))
- [**optimizers**](https://developers.google.com/machine-learning/glossary#optimizer)

Praxis provides the definitions for the Model class.

## precision

A metric for [**classification models**](https://developers.google.com/machine-learning/glossary#classification_model) that answers the following question:

> When the model predicted the [**positive class**](https://developers.google.com/machine-learning/glossary#positive_class), what percentage of the predictions were correct?

Here is the formula:

Precision=true positivestrue positives+false positives

where:

- true positive means the model _correctly_ predicted the positive class.
- false positive means the model _mistakenly_ predicted the positive class.

For example, suppose a model made 200 positive predictions. Of these 200 positive predictions:

- 150 were true positives.
- 50 were false positives.

In this case:

Precision=150150+50=0.75

Contrast with [**accuracy**](https://developers.google.com/machine-learning/glossary#accuracy) and [**recall**](https://developers.google.com/machine-learning/glossary#recall).

## precision-recall curve

A curve of [**precision**](https://developers.google.com/machine-learning/glossary#precision) vs. [**recall**](https://developers.google.com/machine-learning/glossary#recall) at different [**classification thresholds**](https://developers.google.com/machine-learning/glossary#classification_threshold).

## prediction

\#fundamentals

A model's output. For example:

- The prediction of a binary classification model is either the positive class or the negative class.
- The prediction of a multi-class classification model is one class.
- The prediction of a linear regression model is a number.

## prediction bias

A value indicating how far apart the average of [**predictions**](https://developers.google.com/machine-learning/glossary#prediction) is from the average of [**labels**](https://developers.google.com/machine-learning/glossary#label) in the dataset.

Not to be confused with the [**bias term**](https://developers.google.com/machine-learning/glossary#bias) in machine learning models or with [**bias in ethics and fairness**](https://developers.google.com/machine-learning/glossary#bias_ethics).

## predictive parity

\#fairness

A [**fairness metric**](https://developers.google.com/machine-learning/glossary#fairness_metric) that checks whether, for a given classifier, the [**precision**](https://developers.google.com/machine-learning/glossary#precision) rates are equivalent for subgroups under consideration.

For example, a model that predicts college acceptance would satisfy predictive parity for nationality if its precision rate is the same for Lilliputians and Brobdingnagians.

Predictive parity is sometime also called _predictive rate parity_.

See ["Fairness Definitions Explained"](http://fairware.cs.umass.edu/papers/Verma.pdf) (section 3.2.1) for a more detailed discussion of predictive parity.

## predictive rate parity

\#fairness

Another name for [**predictive parity**](https://developers.google.com/machine-learning/glossary#predictive_parity).

## preprocessing

\#fairness

Processing data before it's used to train a model. Preprocessing could be as simple as removing words from an English text corpus that don't occur in the English dictionary, or could be as complex as re-expressing data points in a way that eliminates as many attributes that are correlated with [**sensitive attributes**](https://developers.google.com/machine-learning/glossary#sensitive_attribute) as possible. Preprocessing can help satisfy [**fairness constraints**](https://developers.google.com/machine-learning/glossary#fairness_constraint).

## pre-trained model

Models or model components (such as [**embedding vector**](https://developers.google.com/machine-learning/glossary#embedding_vector)) that have been already been trained. Sometimes, you'll feed pre-trained embedding vectors into a [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network). Other times, your model will train the embedding vectors itself rather than rely on the pre-trained embeddings.

## prior belief

What you believe about the data before you begin training on it. For example, [**L**](https://developers.google.com/machine-learning/glossary#L2_regularization)[**2**](https://developers.google.com/machine-learning/glossary#L2_regularization) [**regularization**](https://developers.google.com/machine-learning/glossary#L2_regularization) relies on a prior belief that [**weights**](https://developers.google.com/machine-learning/glossary#weight) should be small and normally distributed around zero.

## probabilistic regression model

A [**regression model**](https://developers.google.com/machine-learning/glossary#regression_model) that uses not only the [**weights**](https://developers.google.com/machine-learning/glossary#weight) for each [**feature**](https://developers.google.com/machine-learning/glossary#feature), but also the uncertainty of those weights. A probabilistic regression model generates a prediction and the uncertainty of that prediction. For example, a probabilistic regression model might yield a prediction of 325 with a standard deviation of 12. For more information about probabilistic regression models, see this [Colab on tensorflow.org](https://www.tensorflow.org/probability/examples/Probabilistic_Layers_Regression).

## proxy (sensitive attributes)

\#fairness

An attribute used as a stand-in for a [**sensitive attribute**](https://developers.google.com/machine-learning/glossary#sensitive_attribute). For example, an individual's postal code might be used as a proxy for their income, race, or ethnicity.

## proxy labels

\#fundamentals

Data used to approximate labels not directly available in a dataset.

For example, suppose you must train a model to predict employee stress level. Your dataset contains a lot of predictive features but doesn't contain a label named _stress level._ Undaunted, you pick "workplace accidents" as a proxy label for stress level. After all, employees under high stress get into more accidents than calm employees. Or do they? Maybe workplace accidents actually rise and fall for multiple reasons.

As a second example, suppose you want _is it raining?_ to be a Boolean label for your dataset, but your dataset doesn't contain rain data. If photographs are available, you might establish pictures of people carrying umbrellas as a proxy label for _is it raining?_ Is that a good proxy label? Possibly, but people in some cultures may be more likely to carry umbrellas to protect against sun than the rain.

Proxy labels are often imperfect. When possible, choose actual labels over proxy labels. That said, when an actual label is absent, pick the proxy label very carefully, choosing the least horrible proxy label candidate.

## pure function

A function whose outputs are based only on its inputs, and that has no side effects. Specifically, a pure function does not use or change any global state, such as the contents of a file or the value of a variable outside the function.

Pure functions can be used to create thread-safe code, which is beneficial when sharding [**model**](https://developers.google.com/machine-learning/glossary#model) code across multiple [**accelerator chips**](https://developers.google.com/machine-learning/glossary#accelerator-chip).

[**JAX's**](https://developers.google.com/machine-learning/glossary#JAX) function transformation methods require that the input functions are pure functions.

## Q

## Q-function

\#rl

In [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning), the function that predicts the expected [**return**](https://developers.google.com/machine-learning/glossary#return) from taking an [**action**](https://developers.google.com/machine-learning/glossary#action) in a [**state**](https://developers.google.com/machine-learning/glossary#state) and then following a given [**policy**](https://developers.google.com/machine-learning/glossary#policy).

Q-function is also known as **state-action value function**.

## Q-learning

\#rl

In [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning), an algorithm that allows an [**agent**](https://developers.google.com/machine-learning/glossary#agent) to learn the optimal [**Q-function**](https://developers.google.com/machine-learning/glossary#q-function) of a [**Markov decision process**](https://developers.google.com/machine-learning/glossary#markov_decision_process) by applying the [**Bellman equation**](https://developers.google.com/machine-learning/glossary#bellman_equation). The Markov decision process models an [**environment**](https://developers.google.com/machine-learning/glossary#environment).

## quantile

Each bucket in [**quantile bucketing**](https://developers.google.com/machine-learning/glossary#quantile_bucketing).

## quantile bucketing

Distributing a feature's values into [**buckets**](https://developers.google.com/machine-learning/glossary#bucketing) so that each bucket contains the same (or almost the same) number of examples. For example, the following figure divides 44 points into 4 buckets, each of which contains 11 points. In order for each bucket in the figure to contain the same number of points, some buckets span a different width of x-values.

## quantization

Overloaded term that could be used in either of two ways:

- Implementing [**quantile bucketing**](https://developers.google.com/machine-learning/glossary#quantile_bucketing) on a particular [**feature**](https://developers.google.com/machine-learning/glossary#feature).
- Transforming data into zeroes and ones for quicker storing, training, and inferring. As Boolean data is more robust to noise and errors than other formats, quantization can improve model correctness. Quantization techniques include rounding, truncating, and [**binning**](https://developers.google.com/machine-learning/glossary#binning).

## queue

\#TensorFlow

A TensorFlow [**Operation**](https://developers.google.com/machine-learning/glossary#Operation) that implements a queue data structure. Typically used in I/O.

## R

## random forest

\#df

An [**ensemble**](https://developers.google.com/machine-learning/glossary#ensemble) of [**decision trees**](https://developers.google.com/machine-learning/glossary#decision-tree) in which each decision tree is trained with a specific random noise, such as [**bagging**](https://developers.google.com/machine-learning/glossary#bagging).

Random forests are a type of [**decision forest**](https://developers.google.com/machine-learning/glossary#decision-forest).

## random policy

\#rl

In [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning), a [**policy**](https://developers.google.com/machine-learning/glossary#policy) that chooses an [**action**](https://developers.google.com/machine-learning/glossary#action) at random.

## ranking

A type of [**supervised learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning) whose objective is to order a list of items.

## rank (ordinality)

The ordinal position of a class in a machine learning problem that categorizes classes from highest to lowest. For example, a behavior ranking system could rank a dog's rewards from highest (a steak) to lowest (wilted kale).

## rank (Tensor)

\#TensorFlow

The number of dimensions in a [**Tensor**](https://developers.google.com/machine-learning/glossary#tensor). For instance, a scalar has rank 0, a vector has rank 1, and a matrix has rank 2.

Not to be confused with [**rank (ordinality)**](https://developers.google.com/machine-learning/glossary#rank_ordinality).

## rater

\#fundamentals

A human who provides [**labels**](https://developers.google.com/machine-learning/glossary#label) for [**examples**](https://developers.google.com/machine-learning/glossary#example). "Annotator" is another name for rater.

## recall

A metric for [**classification models**](https://developers.google.com/machine-learning/glossary#classification_model) that answers the following question:

> When [**ground truth**](https://developers.google.com/machine-learning/glossary#ground_truth) was the [**positive class**](https://developers.google.com/machine-learning/glossary#positive_class), what percentage of predictions did the model correctly identify as the positive class?

Here is the formula:

Recall=true positivestrue positives+false negatives

where:

- true positive means the model _correctly_ predicted the positive class.
- false negative means that the model _mistakenly_ predicted the [**negative class**](https://developers.google.com/machine-learning/glossary#negative_class).

For instance, suppose your model made 200 predictions on examples for which ground truth was the positive class. Of these 200 predictions:

- 180 were true positives.
- 20 were false negatives.

In this case:

Recall=180180+20=0.9

### Click the icon for notes about class-imbalanced datasets.

## recommendation system

\#recsystems

A system that selects for each user a relatively small set of desirable [**items**](https://developers.google.com/machine-learning/glossary#items) from a large corpus. For example, a video recommendation system might recommend two videos from a corpus of 100,000 videos, selecting _Casablanca_ and _The Philadelphia Story_ for one user, and _Wonder Woman_ and _Black Panther_ for another. A video recommendation system might base its recommendations on factors such as:

- Movies that similar users have rated or watched.
- Genre, directors, actors, target demographic...

## Rectified Linear Unit (ReLU)

\#fundamentals

An [**activation function**](https://developers.google.com/machine-learning/glossary#activation_function) with the following behavior:

- If input is negative or zero, then the output is 0.
- If input is positive, then the output is equal to the input.

For example:

- If the input is -3, then the output is 0.
- If the input is +3, then the output is 3.0.

Here is a plot of ReLU:

ReLU is a very popular activation function. Despite its simple behavior, ReLU still enables a neural network to learn [**nonlinear**](https://developers.google.com/machine-learning/glossary#nonlinear) relationships between [**features**](https://developers.google.com/machine-learning/glossary#feature) and the [**label**](https://developers.google.com/machine-learning/glossary#label).

## recurrent neural network

\#seq

A [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network) that is intentionally run multiple times, where parts of each run feed into the next run. Specifically, hidden layers from the previous run provide part of the input to the same hidden layer in the next run. Recurrent neural networks are particularly useful for evaluating sequences, so that the hidden layers can learn from previous runs of the neural network on earlier parts of the sequence.

For example, the following figure shows a recurrent neural network that runs four times. Notice that the values learned in the hidden layers from the first run become part of the input to the same hidden layers in the second run. Similarly, the values learned in the hidden layer on the second run become part of the input to the same hidden layer in the third run. In this way, the recurrent neural network gradually trains and predicts the meaning of the entire sequence rather than just the meaning of individual words.

## regression model

\#fundamentals

Informally, a model that generates a numerical prediction. (In contrast, a [**classification model**](https://developers.google.com/machine-learning/glossary#classification_model) generates a class prediction.) For example, the following are all regression models:

- A model that predicts a certain house's value, such as 423,000 Euros.
- A model that predicts a certain tree's life expectancy, such as 23.2 years.
- A model that predicts the amount of rain that will fall in a certain city over the next six hours, such as 0.18 inches.

Two common types of regression models are:

- [**Linear regression**](https://developers.google.com/machine-learning/glossary#linear_regression), which finds the line that best fits label values to features.
- [**Logistic regression**](https://developers.google.com/machine-learning/glossary#logistic_regression), which generates a probability between 0.0 and 1.0 that a system typically then maps to a class prediction.

Not every model that outputs numerical predictions is a regression model. In some cases, a numeric prediction is really just a classification model that happens to have numeric class names. For example, a model that predicts a numeric postal code is a classification model, not a regression model.

## regularization

\#fundamentals

Any mechanism that reduces [**overfitting**](https://developers.google.com/machine-learning/glossary#overfitting). Popular types of regularization include:

- [**L**](https://developers.google.com/machine-learning/glossary#L1_regularization)[**1**](https://developers.google.com/machine-learning/glossary#L1_regularization) [**regularization**](https://developers.google.com/machine-learning/glossary#L1_regularization)
- [**L**](https://developers.google.com/machine-learning/glossary#L2_regularization)[**2**](https://developers.google.com/machine-learning/glossary#L2_regularization) [**regularization**](https://developers.google.com/machine-learning/glossary#L2_regularization)
- [**dropout regularization**](https://developers.google.com/machine-learning/glossary#dropout_regularization)
- [**early stopping**](https://developers.google.com/machine-learning/glossary#early_stopping) (this is not a formal regularization method, but can effectively limit overfitting)

Regularization can also be defined as the penalty on a model's complexity.

### Click the icon for additional notes.

## regularization rate

\#fundamentals

A number that specifies the relative importance of [**regularization**](https://developers.google.com/machine-learning/glossary#regularization) during training. Raising the regularization rate reduces [**overfitting**](https://developers.google.com/machine-learning/glossary#overfitting) but may reduce the model's predictive power. Conversely, reducing or omitting the regularization rate increases overfitting.

### Click the icon to see the math.

## reinforcement learning (RL)

\#rl

A family of algorithms that learn an optimal [**policy**](https://developers.google.com/machine-learning/glossary#policy), whose goal is to maximize [**return**](https://developers.google.com/machine-learning/glossary#return) when interacting with an [**environment**](https://developers.google.com/machine-learning/glossary#environment). For example, the ultimate reward of most games is victory. Reinforcement learning systems can become expert at playing complex games by evaluating sequences of previous game moves that ultimately led to wins and sequences that ultimately led to losses.

## ReLU

\#fundamentals

Abbreviation for [**Rectified Linear Unit**](https://developers.google.com/machine-learning/glossary#ReLU).

## replay buffer

\#rl

In [**DQN**](https://developers.google.com/machine-learning/glossary#deep_q-network)-like algorithms, the memory used by the agent to store state transitions for use in [**experience replay**](https://developers.google.com/machine-learning/glossary#experience_replay).

## reporting bias

\#fairness

The fact that the frequency with which people write about actions, outcomes, or properties is not a reflection of their real-world frequencies or the degree to which a property is characteristic of a class of individuals. Reporting bias can influence the composition of data that machine learning systems learn from.

For example, in books, the word _laughed_ is more prevalent than _breathed_. A machine learning model that estimates the relative frequency of laughing and breathing from a book corpus would probably determine that laughing is more common than breathing.

## representation

The process of mapping data to useful [**features**](https://developers.google.com/machine-learning/glossary#feature).

## re-ranking

\#recsystems

The final stage of a [**recommendation system**](https://developers.google.com/machine-learning/glossary#recommendation_system), during which scored items may be re-graded according to some other (typically, non-ML) algorithm. Re-ranking evaluates the list of items generated by the [**scoring**](https://developers.google.com/machine-learning/glossary#scoring) phase, taking actions such as:

- Eliminating items that the user has already purchased.
- Boosting the score of fresher items.

## retrieval-augmented generation

\#fundamentals

A software architecture commonly used in [large language model](https://developers.google.com/machine-learning/glossary#large-language-model) (LLM) applications. Common motivations to use retrieval-augmented generation include:

- Increasing the factual accuracy of the model's generated responses
- Giving the model access to knowledge it was not trained on
- Changing what knowledge the model uses
- Enabling the model to cite sources

For example, suppose that a chemistry app uses the [PaLM API](https://developers.generativeai.google/products/palm) to generate summaries related to user queries. When the app's backend receives a query, the backend first searches for ("retrieves") data that's relevant to the user's query, appends ("augments") the relevant chemistry data to the user's query, and instructs the LLM to create a summary based on the appended data.

## return

\#rl

In reinforcement learning, given a certain policy and a certain state, the return is the sum of all [**rewards**](https://developers.google.com/machine-learning/glossary#reward) that the [**agent**](https://developers.google.com/machine-learning/glossary#agent) expects to receive when following the [**policy**](https://developers.google.com/machine-learning/glossary#policy) from the [**state**](https://developers.google.com/machine-learning/glossary#state) to the end of the [**episode**](https://developers.google.com/machine-learning/glossary#episode). The agent accounts for the delayed nature of expected rewards by discounting rewards according to the state transitions required to obtain the reward.

Therefore, if the discount factor is , and

r0,…,rN denote the rewards until the end of the episode, then the return calculation is as follows:

Return=r0+γr1+γ2r2+…+γN−1rN−1

## reward

\#rl

In reinforcement learning, the numerical result of taking an [**action**](https://developers.google.com/machine-learning/glossary#action) in a [**state**](https://developers.google.com/machine-learning/glossary#state), as defined by the [**environment**](https://developers.google.com/machine-learning/glossary#environment).

## ridge regularization

Synonym for [**L**](https://developers.google.com/machine-learning/glossary#L2_regularization)[**2**](https://developers.google.com/machine-learning/glossary#L2_regularization) [**regularization**](https://developers.google.com/machine-learning/glossary#L2_regularization). The term **ridge regularization** is more frequently used in pure statistics contexts, whereas **L****2** **regularization** is used more often in machine learning.

## RNN

\#seq

Abbreviation for [**recurrent neural networks**](https://developers.google.com/machine-learning/glossary#recurrent_neural_network).

## ROC (receiver operating characteristic) Curve

\#fundamentals

A graph of [**true positive rate**](https://developers.google.com/machine-learning/glossary#TP_rate) vs. [**false positive rate**](https://developers.google.com/machine-learning/glossary#FP_rate) for different [**classification thresholds**](https://developers.google.com/machine-learning/glossary#classification_threshold) in binary classification.

The shape of an ROC curve suggests a binary classification model's ability to separate positive classes from negative classes. Suppose, for example, that a binary classification model perfectly separates all the negative classes from all the positive classes:

The ROC curve for the preceding model looks as follows:

In contrast, the following illustration graphs the raw logistic regression values for a terrible model that can't separate negative classes from positive classes at all:

The ROC curve for this model looks as follows:

Meanwhile, back in the real world, most binary classification models separate positive and negative classes to some degree, but usually not perfectly. So, a typical ROC curve falls somewhere between the two extremes:

The point on an ROC curve closest to (0.0,1.0) theoretically identifies the ideal classification threshold. However, several other real-world issues influence the selection of the ideal classification threshold. For example, perhaps false negatives cause far more pain than false positives.

A numerical metric called [**AUC**](https://developers.google.com/machine-learning/glossary#AUC) summarizes the ROC curve into a single floating-point value.

## root

\#df

The starting [**node**](https://developers.google.com/machine-learning/glossary#node-decision-tree) (the first [**condition**](https://developers.google.com/machine-learning/glossary#condition)) in a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree). By convention, diagrams put the root at the top of the decision tree. For example:

## root directory

\#TensorFlow

The directory you specify for hosting subdirectories of the TensorFlow checkpoint and events files of multiple models.

## Root Mean Squared Error (RMSE)

\#fundamentals

The square root of the [**Mean Squared Error**](https://developers.google.com/machine-learning/glossary#MSE).

## rotational invariance

\#image

In an image classification problem, an algorithm's ability to successfully classify images even when the orientation of the image changes. For example, the algorithm can still identify a tennis racket whether it is pointing up, sideways, or down. Note that rotational invariance is not always desirable; for example, an upside-down 9 should not be classified as a 9.

See also [**translational invariance**](https://developers.google.com/machine-learning/glossary#translational_invariance) and [**size invariance**](https://developers.google.com/machine-learning/glossary#size_invariance).

## R-squared

A [**regression**](https://developers.google.com/machine-learning/glossary#regression_model) metric indicating how much variation in a [**label**](https://developers.google.com/machine-learning/glossary#label) is due to an individual feature or to a feature set. R-squared is a value between 0 and 1, which you can interpret as follows:

- An R-squared of 0 means that none of a label's variation is due to the feature set.
- An R-squared of 1 means that all of a label's variation is due to the feature set.
- An R-squared between 0 and 1 indicates the extent to which the label's variation can be predicted from a particular feature or the feature set. For example, an R-squared of 0.10 means that 10 percent of the variance in the label is due to the feature set, an R-squared of 0.20 means that 20 percent is due to the feature set, and so on.

R-squared is the square of the [Pearson correlation coefficient](https://wikipedia.org/wiki/Correlation_coefficient) between the values that a model predicted and [**ground truth**](https://developers.google.com/machine-learning/glossary#ground_truth).

## S

## sampling bias

\#fairness

See [**selection bias**](https://developers.google.com/machine-learning/glossary#selection_bias).

## sampling with replacement

\#df

A method of picking items from a set of candidate items in which the same item can be picked multiple times. The phrase "with replacement" means that after each selection, the selected item is returned to the pool of candidate items. The inverse method, **sampling without replacement**, means that a candidate item can only be picked once.

For example, consider the following fruit set:

```Plain
fruit = {kiwi, apple, pear, fig, cherry, lime, mango}
```

Suppose that the system randomly picks `fig` as the first item. If using sampling with replacement, then the system picks the second item from the following set:

```Plain
fruit = {kiwi, apple, pear, fig, cherry, lime, mango}
```

Yes, that's the same set as before, so the system could potentially pick `fig` again.

If using sampling without replacement, once picked, a sample can't be picked again. For example, if the system randomly picks `fig` as the first sample, then `fig` can't be picked again. Therefore, the system picks the second sample from the following (reduced) set:

```Plain
fruit = {kiwi, apple, pear, cherry, lime, mango}
```

### Click the icon for additional notes.

## SavedModel

\#TensorFlow

The recommended format for saving and recovering TensorFlow models. SavedModel is a language-neutral, recoverable serialization format, which enables higher-level systems and tools to produce, consume, and transform TensorFlow models.

See the [Saving and Restoring chapter](https://www.tensorflow.org/guide/saved_model) in the TensorFlow Programmer's Guide for complete details.

## Saver

\#TensorFlow

A [TensorFlow object](https://www.tensorflow.org/api_docs/python/tf/compat/v1/train/Saver) responsible for saving model checkpoints.

## scalar

A single number or a single string that can be represented as a [**tensor**](https://developers.google.com/machine-learning/glossary#tensor) of [**rank**](https://developers.google.com/machine-learning/glossary#rank) 0. For example, the following lines of code each create one scalar in TensorFlow:

```Plain
breed = tf.Variable("poodle", tf.string)
temperature = tf.Variable(27, tf.int16)
precision = tf.Variable(0.982375101275, tf.float64)
```

## scaling

Any mathematical transform or technique that shifts the range of a label and/or feature value. Some forms of scaling are very useful for transformations like [**normalization**](https://developers.google.com/machine-learning/glossary#normalization).

Common forms of scaling useful in Machine Learning include:

- linear scaling, which typically uses a combination of subtraction and division to replace the original value with a number between -1 and +1 or between 0 and 1.
- logarithmic scaling, which replaces the original value with its logarithm.
- [**Z-score normalization**](https://developers.google.com/machine-learning/glossary#Z-score-normalization), which replaces the original value with a floating-point value representing the number of standard deviations from that feature's mean.

## scikit-learn

A popular open-source machine learning platform. See [scikit-learn.org](http://scikit-learn.org/).

## scoring

\#recsystems

The part of a [**recommendation system**](https://developers.google.com/machine-learning/glossary#recommendation_system) that provides a value or ranking for each item produced by the [**candidate generation**](https://developers.google.com/machine-learning/glossary#candidate_generation) phase.

## selection bias

\#fairness

Errors in conclusions drawn from sampled data due to a selection process that generates systematic differences between samples observed in the data and those not observed. The following forms of selection bias exist:

- **coverage bias**: The population represented in the dataset does not match the population that the machine learning model is making predictions about.
- **sampling bias**: Data is not collected randomly from the target group.
- **non-response bias** (also called **participation bias**): Users from certain groups opt-out of surveys at different rates than users from other groups.

For example, suppose you are creating a machine learning model that predicts people's enjoyment of a movie. To collect training data, you hand out a survey to everyone in the front row of a theater showing the movie. Offhand, this may sound like a reasonable way to gather a dataset; however, this form of data collection may introduce the following forms of selection bias:

- coverage bias: By sampling from a population who chose to see the movie, your model's predictions may not generalize to people who did not already express that level of interest in the movie.
- sampling bias: Rather than randomly sampling from the intended population (all the people at the movie), you sampled only the people in the front row. It is possible that the people sitting in the front row were more interested in the movie than those in other rows.
- non-response bias: In general, people with strong opinions tend to respond to optional surveys more frequently than people with mild opinions. Since the movie survey is optional, the responses are more likely to form a [bimodal distribution](https://wikipedia.org/wiki/Multimodal_distribution) than a normal (bell-shaped) distribution.

## self-attention (also called self-attention layer)

\#language

A neural network layer that transforms a sequence of embeddings (for instance, [**token**](https://developers.google.com/machine-learning/glossary#token) embeddings) into another sequence of embeddings. Each embedding in the output sequence is constructed by integrating information from the elements of the input sequence through an [**attention**](https://developers.google.com/machine-learning/glossary#attention) mechanism.

The **self** part of **self-attention** refers to the sequence attending to itself rather than to some other context. Self-attention is one of the main building blocks for [**Transformers**](https://developers.google.com/machine-learning/glossary#Transformer) and uses dictionary lookup terminology, such as “query”, “key”, and “value”.

A self-attention layer starts with a sequence of input representations, one for each word. The input representation for a word can be a simple embedding. For each word in an input sequence, the network scores the relevance of the word to every element in the whole sequence of words. The relevance scores determine how much the word's final representation incorporates the representations of other words.

For example, consider the following sentence:

> The animal didn't cross the street because it was too tired.

The following illustration (from [Transformer: A Novel Neural Network Architecture for Language Understanding](https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html)) shows a self-attention layer's attention pattern for the pronoun **it**, with the darkness of each line indicating how much each word contributes to the representation:

The self-attention layer highlights words that are relevant to "it". In this case, the attention layer has learned to highlight words that **it** might refer to, assigning the highest weight to **animal**.

For a sequence of _n_ [**tokens**](https://developers.google.com/machine-learning/glossary#token), self-attention transforms a sequence of embeddings _n_ separate times, once at each position in the sequence.

Refer also to [**attention**](https://developers.google.com/machine-learning/glossary#attention) and [**multi-head self-attention**](https://developers.google.com/machine-learning/glossary#multi-head-self-attention).

## self-supervised learning

A family of techniques for converting an [**unsupervised machine learning**](https://developers.google.com/machine-learning/glossary#unsupervised_machine_learning) problem into a [**supervised machine learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning) problem by creating surrogate [**labels**](https://developers.google.com/machine-learning/glossary#label) from [**unlabeled examples**](https://developers.google.com/machine-learning/glossary#unlabeled_example).

Some [**Transformer**](https://developers.google.com/machine-learning/glossary#Transformer)-based models such as [**BERT**](https://developers.google.com/machine-learning/glossary#BERT) use self-supervised learning.

Self-supervised training is a [**semi-supervised learning**](https://developers.google.com/machine-learning/glossary#semi-supervised_learning) approach.

## self-training

A variant of [**self-supervised learning**](https://developers.google.com/machine-learning/glossary#self-supervised-learning) that is particularly useful when all of the following conditions are true:

- The ratio of [**unlabeled examples**](https://developers.google.com/machine-learning/glossary#unlabeled_example) to [**labeled examples**](https://developers.google.com/machine-learning/glossary#labeled_example) in the dataset is high.
- This is a [**classification**](https://developers.google.com/machine-learning/glossary#classification_model) problem.

Self-training works by iterating over the following two steps until the model stops improving:

1. Use [**supervised machine learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning) to train a model on the labeled examples.
2. Use the model created in Step 1 to generate predictions (labels) on the unlabeled examples, moving those in which there is high confidence into the labeled examples with the predicted label.

Notice that each iteration of Step 2 adds more labeled examples for Step 1 to train on.

## semi-supervised learning

Training a model on data where some of the training examples have labels but others don't. One technique for semi-supervised learning is to infer labels for the unlabeled examples, and then to train on the inferred labels to create a new model. Semi-supervised learning can be useful if labels are expensive to obtain but unlabeled examples are plentiful.

[**Self-training**](https://developers.google.com/machine-learning/glossary#self-training) is one technique for semi-supervised learning.

## sensitive attribute

\#fairness

A human attribute that may be given special consideration for legal, ethical, social, or personal reasons.

## sentiment analysis

\#language

Using statistical or machine learning algorithms to determine a group's overall attitude—positive or negative—toward a service, product, organization, or topic. For example, using [**natural language understanding**](https://developers.google.com/machine-learning/glossary#natural_language_understanding), an algorithm could perform sentiment analysis on the textual feedback from a university course to determine the degree to which students generally liked or disliked the course.

## sequence model

\#seq

A model whose inputs have a sequential dependence. For example, predicting the next video watched from a sequence of previously watched videos.

## sequence-to-sequence task

\#language

A task that converts an input sequence of [**tokens**](https://developers.google.com/machine-learning/glossary#token) to an output sequence of tokens. For example, two popular kinds of sequence-to-sequence tasks are:

- Translators:
    - Sample input sequence: "I love you."
    - Sample output sequence: "Je t'aime."
- Question answering:
    - Sample input sequence: "Do I need my car in New York City?"
    - Sample output sequence: "No. Please keep your car at home."

## serving

A synonym for [**inferring**](https://developers.google.com/machine-learning/glossary#inference).

## shape (Tensor)

The number of elements in each [**dimension**](https://developers.google.com/machine-learning/glossary#dimensions) of a tensor. The shape is represented as a list of integers. For example, the following two-dimensional tensor has a shape of [3,4]:

```Plain
[[5, 7, 6, 4],
 [2, 9, 4, 8],
 [3, 6, 5, 1]]
```

TensorFlow uses row-major (C-style) format to represent the order of dimensions, which is why the shape in TensorFlow is [3,4] rather than [4,3]. In other words, in a two-dimensional TensorFlow Tensor, the shape is [_number of rows_, _number of columns_].

## shrinkage

\#df

A [**hyperparameter**](https://developers.google.com/machine-learning/glossary#hyperparameter) in [**gradient boosting**](https://developers.google.com/machine-learning/glossary#gradient-boosting) that controls [**overfitting**](https://developers.google.com/machine-learning/glossary#overfitting). Shrinkage in gradient boosting is analogous to [**learning rate**](https://developers.google.com/machine-learning/glossary#learning_rate) in [**gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent). Shrinkage is a decimal value between 0.0 and 1.0. A lower shrinkage value reduces overfitting more than a larger shrinkage value.

## sigmoid function

\#fundamentals

A mathematical function that "squishes" an input value into a constrained range, typically 0 to 1 or -1 to +1. That is, you can pass any number (two, a million, negative billion, whatever) to a sigmoid and the output will still be in the constrained range. A plot of the sigmoid activation function looks as follows:

The sigmoid function has several uses in machine learning, including:

- Converting the raw output of a [**logistic regression**](https://developers.google.com/machine-learning/glossary#logistic_regression) or [**multinomial regression**](https://developers.google.com/machine-learning/glossary#multinomial-regression) model to a probability.
- Acting as an [**activation function**](https://developers.google.com/machine-learning/glossary#activation_function) in some neural networks.

### Click the icon to see the math.

## similarity measure

\#clustering

In [**clustering**](https://developers.google.com/machine-learning/glossary#clustering) algorithms, the metric used to determine how alike (how similar) any two examples are.

## single program / multiple data (SPMD)

A parallelism technique where the same computation is run on different input data in parallel on different devices. The goal of SPMD is to obtain results more quickly. It is the most common style of parallel programming.

## size invariance

\#image

In an image classification problem, an algorithm's ability to successfully classify images even when the size of the image changes. For example, the algorithm can still identify a cat whether it consumes 2M pixels or 200K pixels. Note that even the best image classification algorithms still have practical limits on size invariance. For example, an algorithm (or human) is unlikely to correctly classify a cat image consuming only 20 pixels.

See also [**translational invariance**](https://developers.google.com/machine-learning/glossary#translational_invariance) and [**rotational invariance**](https://developers.google.com/machine-learning/glossary#rotational_invariance).

## sketching

\#clustering

In [**unsupervised machine learning**](https://developers.google.com/machine-learning/glossary#unsupervised_machine_learning), a category of algorithms that perform a preliminary similarity analysis on examples. Sketching algorithms use a [locality-sensitive hash function](https://wikipedia.org/wiki/Locality-sensitive_hashing) to identify points that are likely to be similar, and then group them into buckets.

Sketching decreases the computation required for similarity calculations on large datasets. Instead of calculating similarity for every single pair of examples in the dataset, we calculate similarity only for each pair of points within each bucket.

## softmax

\#fundamentals

A function that determines probabilities for each possible class in a [**multi-class classification model**](https://developers.google.com/machine-learning/glossary#multi-class). The probabilities add up to exactly 1.0. For example, the following table shows how softmax distributes various probabilities:

|   |   |
|---|---|
|Image is a...|Probability|
|dog|.85|
|cat|.13|
|horse|.02|

Softmax is also called **full softmax**.

Contrast with [**candidate sampling**](https://developers.google.com/machine-learning/glossary#candidate_sampling).

### Click the icon to see the math.

## sparse feature

\#language

\#fundamentals

A [**feature**](https://developers.google.com/machine-learning/glossary#feature) whose values are predominately zero or empty. For example, a feature containing a single 1 value and a million 0 values is sparse. In contrast, a [**dense feature**](https://developers.google.com/machine-learning/glossary#dense_feature) has values that are predominantly not zero or empty.

In machine learning, a surprising number of features are sparse features. Categorical features are usually sparse features. For example, of the 300 possible tree species in a forest, a single example might identify just a _maple tree_. Or, of the millions of possible videos in a video library, a single example might identify just "Casablanca."

In a model, you typically represent sparse features with [**one-hot encoding**](https://developers.google.com/machine-learning/glossary#one-hot_encoding). If the one-hot encoding is big, you might put an [**embedding layer**](https://developers.google.com/machine-learning/glossary#embedding_layer) on top of the one-hot encoding for greater efficiency.

## sparse representation

\#language

\#fundamentals

Storing only the _position(s)_ of nonzero elements in a sparse feature.

For example, suppose a categorical feature named `species` identifies the 36 tree species in a particular forest. Further assume that each [**example**](https://developers.google.com/machine-learning/glossary#example) identifies only a single species.

You could use a one-hot vector to represent the tree species in each example. A one-hot vector would contain a single `1` (to represent the particular tree species in that example) and 35 `0`s (to represent the 35 tree species _not_ in that example). So, the one-hot representation of `maple` might look something like the following:

Alternatively, sparse representation would simply identify the position of the particular species. If `maple` is at position 24, then the sparse representation of `maple` would simply be:

```Plain
24
```

Notice that the sparse representation is much more compact than the one-hot representation.

**Note:** You shouldn't pass a sparse representation as a direct feature input to a model. Instead, you should convert the sparse representation into a one-hot representation before training on it.

### Click the icon for a slightly more complex example.

**Click the icon if you are confused.**

## sparse vector

\#fundamentals

A vector whose values are mostly zeroes. See also [**sparse feature**](https://developers.google.com/machine-learning/glossary#sparse_features) and [**sparsity**](https://developers.google.com/machine-learning/glossary#sparsity).

## sparsity

The number of elements set to zero (or null) in a vector or matrix divided by the total number of entries in that vector or matrix. For example, consider a 100-element matrix in which 98 cells contain zero. The calculation of sparsity is as follows:

sparsity=98100=0.98

**Feature sparsity** refers to the sparsity of a feature vector; **model sparsity** refers to the sparsity of the model weights.

## spatial pooling

\#image

See [**pooling**](https://developers.google.com/machine-learning/glossary#pooling).

## split

\#df

In a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree), another name for a [**condition**](https://developers.google.com/machine-learning/glossary#condition).

## splitter

\#df

While training a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree), the routine (and algorithm) responsible for finding the best [**condition**](https://developers.google.com/machine-learning/glossary#condition) at each [**node**](https://developers.google.com/machine-learning/glossary#node-decision-tree).

## SPMD

Abbreviation for [**single program / multiple data**](https://developers.google.com/machine-learning/glossary#single-program).

## squared hinge loss

The square of the [**hinge loss**](https://developers.google.com/machine-learning/glossary#hinge-loss). Squared hinge loss penalizes outliers more harshly than regular hinge loss.

## squared loss

\#fundamentals

Synonym for [**L**](https://developers.google.com/machine-learning/glossary#L2_loss)[**2**](https://developers.google.com/machine-learning/glossary#L2_loss) [**loss**](https://developers.google.com/machine-learning/glossary#L2_loss).

## staged training

\#language

A tactic of training a model in a sequence of discrete stages. The goal can be either to speed up the training process, or to achieve better model quality.

An illustration of the progressive stacking approach is shown below:

- Stage 1 contains 3 hidden layers, stage 2 contains 6 hidden layers, and stage 3 contains 12 hidden layers.
- Stage 2 begins training with the weights learned in the 3 hidden layers of Stage 1. Stage 3 begins training with the weights learned in the 6 hidden layers of Stage 2.

See also [**pipelining**](https://developers.google.com/machine-learning/glossary#pipelining).

## state

\#rl

In reinforcement learning, the parameter values that describe the current configuration of the environment, which the [**agent**](https://developers.google.com/machine-learning/glossary#agent) uses to choose an [**action**](https://developers.google.com/machine-learning/glossary#action).

## state-action value function

\#rl

Synonym for [**Q-function**](https://developers.google.com/machine-learning/glossary#q-function).

## static

\#fundamentals

Something done once rather than continuously. The terms **static** and **offline** are synonyms. The following are common uses of **static** and **offline** in machine learning:

- **static model** (or **offline model**) is a model trained once and then used for a while.
- **static training** (or **offline training**) is the process of training a static model.
- **static inference** (or **offline inference**) is a process in which a model generates a batch of predictions at a time.

Contrast with [**dynamic**](https://developers.google.com/machine-learning/glossary#dynamic).

## static inference

\#fundamentals

Synonym for [**offline inference**](https://developers.google.com/machine-learning/glossary#offline_inference).

## stationarity

\#fundamentals

A feature whose values don't change across one or more dimensions, usually time. For example, a feature whose values look about the same in 2021 and 2023 exhibits stationarity.

In the real world, very few features exhibit stationarity. Even features synonymous with stability (like sea level) change over time.

Contrast with [**nonstationarity**](https://developers.google.com/machine-learning/glossary#nonstationarity).

## step

A forward pass and backward pass of one [**batch**](https://developers.google.com/machine-learning/glossary#batch).

See [**backpropagation**](https://developers.google.com/machine-learning/glossary#backpropagation) for more information on the forward pass and backward pass.

## step size

Synonym for [**learning rate**](https://developers.google.com/machine-learning/glossary#learning_rate).

## stochastic gradient descent (SGD)

\#fundamentals

A [**gradient descent**](https://developers.google.com/machine-learning/glossary#gradient_descent) algorithm in which the [**batch size**](https://developers.google.com/machine-learning/glossary#batch_size) is one. In other words, SGD trains on a single example chosen uniformly at random from a [**training set**](https://developers.google.com/machine-learning/glossary#training_set).

## stride

\#image

In a convolutional operation or pooling, the delta in each dimension of the next series of input slices. For example, the following animation demonstrates a (1,1) stride during a convolutional operation. Therefore, the next input slice starts one position to the right of the previous input slice. When the operation reaches the right edge, the next slice is all the way over to the left but one position down.

The preceding example demonstrates a two-dimensional stride. If the input matrix is three-dimensional, the stride would also be three-dimensional.

## structural risk minimization (SRM)

An algorithm that balances two goals:

- The desire to build the most predictive model (for example, lowest loss).
- The desire to keep the model as simple as possible (for example, strong regularization).

For example, a function that minimizes loss+regularization on the training set is a structural risk minimization algorithm.

Contrast with [**empirical risk minimization**](https://developers.google.com/machine-learning/glossary#ERM).

## subsampling

\#image

See [**pooling**](https://developers.google.com/machine-learning/glossary#pooling).

## summary

\#TensorFlow

In TensorFlow, a value or set of values calculated at a particular [**step**](https://developers.google.com/machine-learning/glossary#step), usually used for tracking model metrics during training.

## supervised machine learning

\#fundamentals

Training a [**model**](https://developers.google.com/machine-learning/glossary#model) from [**features**](https://developers.google.com/machine-learning/glossary#feature) and their corresponding [**labels**](https://developers.google.com/machine-learning/glossary#label). Supervised machine learning is analogous to learning a subject by studying a set of questions and their corresponding answers. After mastering the mapping between questions and answers, a student can then provide answers to new (never-before-seen) questions on the same topic.

Compare with [**unsupervised machine learning**](https://developers.google.com/machine-learning/glossary#unsupervised_machine_learning).

## synthetic feature

\#fundamentals

A [**feature**](https://developers.google.com/machine-learning/glossary#feature) not present among the input features, but assembled from one or more of them. Methods for creating synthetic features include the following:

- [**Bucketing**](https://developers.google.com/machine-learning/glossary#bucketing) a continuous feature into range bins.
- Creating a [**feature cross**](https://developers.google.com/machine-learning/glossary#feature_cross).
- Multiplying (or dividing) one feature value by other feature value(s) or by itself. For example, if `a` and `b` are input features, then the following are examples of synthetic features:
    - ab
    - a
        
        2
        
- Applying a transcendental function to a feature value. For example, if `c` is an input feature, then the following are examples of synthetic features:
    - sin(c)
    - ln(c)

Features created by [**normalizing**](https://developers.google.com/machine-learning/glossary#normalization) or [**scaling**](https://developers.google.com/machine-learning/glossary#scaling) alone are not considered synthetic features.

## T

## T5

\#language

A text-to-text [**transfer learning**](https://developers.google.com/machine-learning/glossary#transfer_learning) [**model**](https://developers.google.com/machine-learning/glossary#model) introduced by [Google AI in 2020](https://arxiv.org/pdf/1910.10683.pdf). T5 is an [**encoder**](https://developers.google.com/machine-learning/glossary#encoder)-[**decoder**](https://developers.google.com/machine-learning/glossary#decoder) model, based on the [**Transformer**](https://developers.google.com/machine-learning/glossary#transformer) architecture, trained on an extremely large dataset. It is effective at a variety of natural language processing tasks, such as generating text, translating languages, and answering questions in a conversational manner.

T5 gets its name from the five T's in "Text-to-Text Transfer Transformer."

## T5X

\#language

An open-source, [**machine learning**](https://developers.google.com/machine-learning/glossary#machine_learning) framework designed to build and [**train**](https://developers.google.com/machine-learning/glossary#training) large-scale natural language processing (NLP) models. [**T5**](https://developers.google.com/machine-learning/glossary#T5) is implemented on the T5X codebase (which is built on [**JAX**](https://developers.google.com/machine-learning/glossary#JAX) and [**Flax**](https://developers.google.com/machine-learning/glossary#flax)).

## tabular Q-learning

\#rl

In [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning), implementing [**Q-learning**](https://developers.google.com/machine-learning/glossary#q-learning) by using a table to store the [**Q-functions**](https://developers.google.com/machine-learning/glossary#q-function) for every combination of [**state**](https://developers.google.com/machine-learning/glossary#state) and [**action**](https://developers.google.com/machine-learning/glossary#action).

## target

Synonym for [**label**](https://developers.google.com/machine-learning/glossary#label).

## target network

\#rl

In [**Deep Q-learning**](https://developers.google.com/machine-learning/glossary#q-learning), a neural network that is a stable approximation of the main neural network, where the main neural network implements either a [**Q-function**](https://developers.google.com/machine-learning/glossary#q-function) or a [**policy**](https://developers.google.com/machine-learning/glossary#policy). Then, you can train the main network on the Q-values predicted by the target network. Therefore, you prevent the feedback loop that occurs when the main network trains on Q-values predicted by itself. By avoiding this feedback, training stability increases.

## task

A problem that can be solved using machine learning techniques, such as:

- [**classification**](https://developers.google.com/machine-learning/glossary#classification_model)
- [**regression**](https://developers.google.com/machine-learning/glossary#regression_model)
- [**clustering**](https://developers.google.com/machine-learning/glossary#clustering)
- [**anomaly detection**](https://developers.google.com/machine-learning/glossary#anomaly-detection)

## temporal data

Data recorded at different points in time. For example, winter coat sales recorded for each day of the year would be temporal data.

## Tensor

\#TensorFlow

The primary data structure in TensorFlow programs. Tensors are N-dimensional (where N could be very large) data structures, most commonly scalars, vectors, or matrices. The elements of a Tensor can hold integer, floating-point, or string values.

## TensorBoard

\#TensorFlow

The dashboard that displays the summaries saved during the execution of one or more TensorFlow programs.

## TensorFlow

\#TensorFlow

A large-scale, distributed, machine learning platform. The term also refers to the base API layer in the TensorFlow stack, which supports general computation on dataflow graphs.

Although TensorFlow is primarily used for machine learning, you may also use TensorFlow for non-ML tasks that require numerical computation using dataflow graphs.

## TensorFlow Playground

\#TensorFlow

A program that visualizes how different [**hyperparameters**](https://developers.google.com/machine-learning/glossary#hyperparameter) influence model (primarily neural network) training. Go to [http://playground.tensorflow.org](http://playground.tensorflow.org/) to experiment with TensorFlow Playground.

## TensorFlow Serving

\#TensorFlow

A platform to deploy trained models in production.

## Tensor Processing Unit (TPU)

\#TensorFlow

\#GoogleCloud

An application-specific integrated circuit (ASIC) that optimizes the performance of machine learning workloads. These ASICs are deployed as multiple [**TPU chips**](https://developers.google.com/machine-learning/glossary#TPU_chip) on a [**TPU device**](https://developers.google.com/machine-learning/glossary#TPU_device).

## Tensor rank

\#TensorFlow

See [**rank (Tensor)**](https://developers.google.com/machine-learning/glossary#rank_Tensor).

## Tensor shape

\#TensorFlow

The number of elements a [**Tensor**](https://developers.google.com/machine-learning/glossary#tensor) contains in various dimensions. For example, a [5, 10] Tensor has a shape of 5 in one dimension and 10 in another.

## Tensor size

\#TensorFlow

The total number of scalars a [**Tensor**](https://developers.google.com/machine-learning/glossary#tensor) contains. For example, a [5, 10] Tensor has a size of 50.

## TensorStore

A [library](https://google.github.io/tensorstore/) for efficiently reading and writing large multi-dimensional arrays.

## termination condition

\#rl

In [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning), the conditions that determine when an [**episode**](https://developers.google.com/machine-learning/glossary#episode) ends, such as when the agent reaches a certain state or exceeds a threshold number of state transitions. For example, in [tic-tac-toe](https://wikipedia.org/wiki/Tic-tac-toe) (also known as noughts and crosses), an episode terminates either when a player marks three consecutive spaces or when all spaces are marked.

## test

\#df

In a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree), another name for a [**condition**](https://developers.google.com/machine-learning/glossary#condition).

## test loss

\#fundamentals

A [**metric**](https://developers.google.com/machine-learning/glossary#metric) representing a model's [**loss**](https://developers.google.com/machine-learning/glossary#loss) against the [**test set**](https://developers.google.com/machine-learning/glossary#test_set). When building a [**model**](https://developers.google.com/machine-learning/glossary#model), you typically try to minimize test loss. That's because a low test loss is a stronger quality signal than a low [**training loss**](https://developers.google.com/machine-learning/glossary#training-loss) or low [**validation loss**](https://developers.google.com/machine-learning/glossary#validation-loss).

A large gap between test loss and training loss or validation loss sometimes suggests that you need to increase the [**regularization rate**](https://developers.google.com/machine-learning/glossary#regularization_rate).

## test set

A subset of the [**dataset**](https://developers.google.com/machine-learning/glossary#dataset) reserved for testing a trained [**model**](https://developers.google.com/machine-learning/glossary#model).

Traditionally, you divide examples in the dataset into the following three distinct subsets:

- a [**training set**](https://developers.google.com/machine-learning/glossary#training_set)
- a [**validation set**](https://developers.google.com/machine-learning/glossary#validation_set)
- a test set

Each example in a dataset should belong to only one of the preceding subsets. For instance, a single example should not belong to both the training set and the test set.

The training set and validation set are both closely tied to training a model. Because the test set is only indirectly associated with training, [**test loss**](https://developers.google.com/machine-learning/glossary#test-loss) is a less biased, higher quality metric than [**training loss**](https://developers.google.com/machine-learning/glossary#training-loss) or [**validation loss**](https://developers.google.com/machine-learning/glossary#validation-loss).

## text span

\#language

The array index span associated with a specific subsection of a text string. For example, the word `good` in the Python string `s="Be good now"` occupies the text span from 3 to 6.

## tf.Example

\#TensorFlow

A standard [protocol buffer](https://developers.google.com/protocol-buffers/) for describing input data for machine learning model training or inference.

## tf.keras

\#TensorFlow

An implementation of [**Keras**](https://developers.google.com/machine-learning/glossary#Keras) integrated into [**TensorFlow**](https://developers.google.com/machine-learning/glossary#TensorFlow).

## threshold (for decision trees)

\#df

In an [**axis-aligned condition**](https://developers.google.com/machine-learning/glossary#axis-aligned-condition), the value that a [**feature**](https://developers.google.com/machine-learning/glossary#feature) is being compared against. For example, 75 is the threshold value in the following condition:

```Plain
grade >= 75
```

This form of the term **threshold** is different than [**classification threshold**](https://developers.google.com/machine-learning/glossary#classification_threshold).

## time series analysis

\#clustering

A subfield of machine learning and statistics that analyzes [**temporal data**](https://developers.google.com/machine-learning/glossary#temporal_data). Many types of machine learning problems require time series analysis, including classification, clustering, forecasting, and anomaly detection. For example, you could use time series analysis to forecast the future sales of winter coats by month based on historical sales data.

## timestep

\#seq

One "unrolled" cell within a [**recurrent neural network**](https://developers.google.com/machine-learning/glossary#recurrent_neural_network). For example, the following figure shows three timesteps (labeled with the subscripts t-1, t, and t+1):

## token

\#language

In a [**language model**](https://developers.google.com/machine-learning/glossary#language-model), the atomic unit that the model is training on and making predictions on. A token is typically one of the following:

- a word—for example, the phrase "dogs like cats" consists of three word tokens: "dogs", "like", and "cats".
- a character—for example, the phrase "bike fish" consists of nine character tokens. (Note that the blank space counts as one of the tokens.)
- subwords—in which a single word can be a single token or multiple tokens. A subword consists of a root word, a prefix, or a suffix. For example, a language model that uses subwords as tokens might view the word "dogs" as two tokens (the root word "dog" and the plural suffix "s"). That same language model might view the single word "taller" as two subwords (the root word "tall" and the suffix "er").

In domains outside of language models, tokens can represent other kinds of atomic units. For example, in computer vision, a token might be a subset of an image.

## tower

A component of a [**deep neural network**](https://developers.google.com/machine-learning/glossary#deep_neural_network) that is itself a deep neural network without an output layer. Typically, each tower reads from an independent data source. Towers are independent until their output is combined in a final layer.

## TPU

\#TensorFlow

\#GoogleCloud

Abbreviation for [**Tensor Processing Unit**](https://developers.google.com/machine-learning/glossary#TPU).

## TPU chip

\#TensorFlow

\#GoogleCloud

A programmable linear algebra accelerator with on-chip high bandwidth memory that is optimized for machine learning workloads. Multiple TPU chips are deployed on a [**TPU device**](https://developers.google.com/machine-learning/glossary#TPU_device).

## TPU device

\#TensorFlow

\#GoogleCloud

A printed circuit board (PCB) with multiple [**TPU chips**](https://developers.google.com/machine-learning/glossary#TPU_chip), high bandwidth network interfaces, and system cooling hardware.

## TPU master

\#TensorFlow

\#GoogleCloud

The central coordination process running on a host machine that sends and receives data, results, programs, performance, and system health information to the [**TPU workers**](https://developers.google.com/machine-learning/glossary#TPU_worker). The TPU master also manages the setup and shutdown of [**TPU devices**](https://developers.google.com/machine-learning/glossary#TPU_device).

## TPU node

\#TensorFlow

\#GoogleCloud

A TPU resource on Google Cloud Platform with a specific [**TPU type**](https://developers.google.com/machine-learning/glossary#TPU_type). The TPU node connects to your [VPC Network](https://cloud.google.com/vpc/docs/) from a [peer VPC network](https://cloud.google.com/vpc/docs/vpc-peering). TPU nodes are a resource defined in the [Cloud TPU API](https://cloud.google.com/tpu/docs/reference/rest/v1/projects.locations.nodes).

## TPU Pod

\#TensorFlow

\#GoogleCloud

A specific configuration of [**TPU devices**](https://developers.google.com/machine-learning/glossary#TPU_device) in a Google data center. All of the devices in a TPU pod are connected to one another over a dedicated high-speed network. A TPU Pod is the largest configuration of [**TPU devices**](https://developers.google.com/machine-learning/glossary#TPU_device) available for a specific TPU version.

## TPU resource

\#TensorFlow

\#GoogleCloud

A TPU entity on Google Cloud Platform that you create, manage, or consume. For example, [**TPU nodes**](https://developers.google.com/machine-learning/glossary#TPU_node) and [**TPU types**](https://developers.google.com/machine-learning/glossary#TPU_type) are TPU resources.

## TPU slice

\#TensorFlow

\#GoogleCloud

A TPU slice is a fractional portion of the [**TPU devices**](https://developers.google.com/machine-learning/glossary#TPU_device) in a [**TPU Pod**](https://developers.google.com/machine-learning/glossary#TPU_Pod). All of the devices in a TPU slice are connected to one another over a dedicated high-speed network.

## TPU type

\#TensorFlow

\#GoogleCloud

A configuration of one or more [**TPU devices**](https://developers.google.com/machine-learning/glossary#TPU_device) with a specific TPU hardware version. You select a TPU type when you create a [**TPU node**](https://developers.google.com/machine-learning/glossary#TPU_node) on Google Cloud Platform. For example, a `v2-8` TPU type is a single TPU v2 device with 8 cores. A `v3-2048` TPU type has 256 networked TPU v3 devices and a total of 2048 cores. TPU types are a resource defined in the [Cloud TPU API](https://cloud.google.com/tpu/docs/reference/rest/v1/projects.locations.acceleratorTypes).

## TPU worker

\#TensorFlow

\#GoogleCloud

A process that runs on a host machine and executes machine learning programs on [**TPU devices**](https://developers.google.com/machine-learning/glossary#TPU_device).

## training

\#fundamentals

The process of determining the ideal [**parameters**](https://developers.google.com/machine-learning/glossary#parameter) (weights and biases) comprising a [**model**](https://developers.google.com/machine-learning/glossary#model). During training, a system reads in [**examples**](https://developers.google.com/machine-learning/glossary#example) and gradually adjusts parameters. Training uses each example anywhere from a few times to billions of times.

## training loss

\#fundamentals

A [**metric**](https://developers.google.com/machine-learning/glossary#metric) representing a model's [**loss**](https://developers.google.com/machine-learning/glossary#loss) during a particular training iteration. For example, suppose the loss function is [**Mean Squared Error**](https://developers.google.com/machine-learning/glossary#MSE). Perhaps the training loss (the Mean Squared Error) for the 10th iteration is 2.2, and the training loss for the 100th iteration is 1.9.

A [**loss curve**](https://developers.google.com/machine-learning/glossary#loss_curve) plots training loss vs. the number of iterations. A loss curve provides the following hints about training:

- A downward slope implies that the model is improving.
- An upward slope implies that the model is getting worse.
- A flat slope implies that the model has reached [**convergence**](https://developers.google.com/machine-learning/glossary#convergence).

For example, the following somewhat idealized [**loss curve**](https://developers.google.com/machine-learning/glossary#loss_curve) shows:

- A steep downward slope during the initial iterations, which implies rapid model improvement.
- A gradually flattening (but still downward) slope until close to the end of training, which implies continued model improvement at a somewhat slower pace then during the initial iterations.
- A flat slope towards the end of training, which suggests convergence.

Although training loss is important, see also [**generalization**](https://developers.google.com/machine-learning/glossary#generalization).

## training-serving skew

\#fundamentals

The difference between a model's performance during [**training**](https://developers.google.com/machine-learning/glossary#training) and that same model's performance during [**serving**](https://developers.google.com/machine-learning/glossary#serving).

## training set

\#fundamentals

The subset of the [**dataset**](https://developers.google.com/machine-learning/glossary#dataset) used to train a [**model**](https://developers.google.com/machine-learning/glossary#model).

Traditionally, examples in the dataset are divided into the following three distinct subsets:

- a training set
- a [**validation set**](https://developers.google.com/machine-learning/glossary#validation_set)
- a [**test set**](https://developers.google.com/machine-learning/glossary#test_set)

Ideally, each example in the dataset should belong to only one of the preceding subsets. For example, a single example should not belong to both the training set and the validation set.

## trajectory

\#rl

In [**reinforcement learning**](https://developers.google.com/machine-learning/glossary#reinforcement_learning), a sequence of [tuples](https://wikipedia.org/wiki/Tuple) that represent a sequence of [**state**](https://developers.google.com/machine-learning/glossary#state) transitions of the [**agent**](https://developers.google.com/machine-learning/glossary#agent), where each tuple corresponds to the state, [**action**](https://developers.google.com/machine-learning/glossary#action), [**reward**](https://developers.google.com/machine-learning/glossary#reward), and next state for a given state transition.

## transfer learning

Transferring information from one machine learning task to another. For example, in multi-task learning, a single model solves multiple tasks, such as a [**deep model**](https://developers.google.com/machine-learning/glossary#deep_model) that has different output nodes for different tasks. Transfer learning might involve transferring knowledge from the solution of a simpler task to a more complex one, or involve transferring knowledge from a task where there is more data to one where there is less data.

Most machine learning systems solve a _single_ task. Transfer learning is a baby step towards artificial intelligence in which a single program can solve _multiple_ tasks.

## Transformer

\#language

A [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network) architecture developed at Google that relies on [**self-attention**](https://developers.google.com/machine-learning/glossary#self-attention) mechanisms to transform a sequence of input embeddings into a sequence of output embeddings without relying on [**convolutions**](https://developers.google.com/machine-learning/glossary#convolution) or [**recurrent neural networks**](https://developers.google.com/machine-learning/glossary#recurrent_neural_network). A Transformer can be viewed as a stack of self-attention layers.

A Transformer can include any of the following:

- an [**encoder**](https://developers.google.com/machine-learning/glossary#encoder)
- a [**decoder**](https://developers.google.com/machine-learning/glossary#decoder)
- both an encoder and decoder

An **encoder** transforms a sequence of embeddings into a new sequence of the same length. An encoder includes N identical layers, each of which contains two sub-layers. These two sub-layers are applied at each position of the input embedding sequence, transforming each element of the sequence into a new embedding. The first encoder sub-layer aggregates information from across the input sequence. The second encoder sub-layer transforms the aggregated information into an output embedding.

A **decoder** transforms a sequence of input embeddings into a sequence of output embeddings, possibly with a different length. A decoder also includes N identical layers with three sub-layers, two of which are similar to the encoder sub-layers. The third decoder sub-layer takes the output of the encoder and applies the [**self-attention**](https://developers.google.com/machine-learning/glossary#self-attention) mechanism to gather information from it.

The blog post [Transformer: A Novel Neural Network Architecture for Language Understanding](https://ai.googleblog.com/2017/08/transformer-novel-neural-network.html) provides a good introduction to Transformers.

## translational invariance

\#image

In an image classification problem, an algorithm's ability to successfully classify images even when the position of objects within the image changes. For example, the algorithm can still identify a dog, whether it is in the center of the frame or at the left end of the frame.

See also [**size invariance**](https://developers.google.com/machine-learning/glossary#size_invariance) and [**rotational invariance**](https://developers.google.com/machine-learning/glossary#rotational_invariance).

## trigram

\#seq

\#language

An [**N-gram**](https://developers.google.com/machine-learning/glossary#N-gram) in which N=3.

## true negative (TN)

\#fundamentals

An example in which the model _correctly_ predicts the [**negative class**](https://developers.google.com/machine-learning/glossary#negative_class). For example, the model infers that a particular email message is _not spam_, and that email message really is _not spam_.

## true positive (TP)

\#fundamentals

An example in which the model _correctly_ predicts the [**positive class**](https://developers.google.com/machine-learning/glossary#positive_class). For example, the model infers that a particular email message is spam, and that email message really is spam.

## true positive rate (TPR)

\#fundamentals

Synonym for [**recall**](https://developers.google.com/machine-learning/glossary#recall). That is:

true positive rate=true positivestrue positives+false negatives

True positive rate is the y-axis in an [**ROC curve**](https://developers.google.com/machine-learning/glossary#ROC).

## U

## unawareness (to a sensitive attribute)

\#fairness

A situation in which [**sensitive attributes**](https://developers.google.com/machine-learning/glossary#sensitive_attribute) are present, but not included in the training data. Because sensitive attributes are often correlated with other attributes of one’s data, a model trained with unawareness about a sensitive attribute could still have [**disparate impact**](https://developers.google.com/machine-learning/glossary#disparate_impact) with respect to that attribute, or violate other [**fairness constraints**](https://developers.google.com/machine-learning/glossary#fairness_constraint).

## underfitting

\#fundamentals

Producing a [**model**](https://developers.google.com/machine-learning/glossary#model) with poor predictive ability because the model hasn't fully captured the complexity of the training data. Many problems can cause underfitting, including:

- Training on the wrong set of [**features**](https://developers.google.com/machine-learning/glossary#feature).
- Training for too few [**epochs**](https://developers.google.com/machine-learning/glossary#epoch) or at too low a [**learning rate**](https://developers.google.com/machine-learning/glossary#learning_rate).
- Training with too high a [**regularization rate**](https://developers.google.com/machine-learning/glossary#regularization_rate).
- Providing too few [**hidden layers**](https://developers.google.com/machine-learning/glossary#hidden_layer) in a deep neural network.

## undersampling

Removing [**examples**](https://developers.google.com/machine-learning/glossary#example) from the [**majority class**](https://developers.google.com/machine-learning/glossary#majority_class) in a [**class-imbalanced dataset**](https://developers.google.com/machine-learning/glossary#class_imbalanced_data_set) in order to create a more balanced [**training set**](https://developers.google.com/machine-learning/glossary#training_set).

For example, consider a dataset in which the ratio of the majority class to the [**minority class**](https://developers.google.com/machine-learning/glossary#minority_class) is 20:1. To overcome this class imbalance, you could create a training set consisting of _all_ of the minority class examples but only a _tenth_ of the majority class examples, which would create a training-set class ratio of 2:1. Thanks to undersampling, this more balanced training set might produce a better model. Alternatively, this more balanced training set might contain insufficient examples to train an effective model.

Contrast with [**oversampling**](https://developers.google.com/machine-learning/glossary#oversampling).

## unidirectional

\#language

A system that only evaluates the text that _precedes_ a target section of text. In contrast, a bidirectional system evaluates both the text that _precedes_ and _follows_ a target section of text. See [**bidirectional**](https://developers.google.com/machine-learning/glossary#bidirectional) for more details.

## unidirectional language model

\#language

A [**language model**](https://developers.google.com/machine-learning/glossary#language-model) that bases its probabilities only on the [**tokens**](https://developers.google.com/machine-learning/glossary#token) appearing _before_, not _after_, the target token(s). Contrast with [**bidirectional language model**](https://developers.google.com/machine-learning/glossary#bidirectional-language-model).

## unlabeled example

\#fundamentals

An example that contains [**features**](https://developers.google.com/machine-learning/glossary#feature) but no [**label**](https://developers.google.com/machine-learning/glossary#label). For example, the following table shows three unlabeled examples from a house valuation model, each with three features but no house value:

|   |   |   |
|---|---|---|
|Number of bedrooms|Number of bathrooms|House age|
|3|2|15|
|2|1|72|
|4|2|34|

In [**supervised machine learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning), models train on labeled examples and make predictions on [**unlabeled examples**](https://developers.google.com/machine-learning/glossary#unlabeled_example).

In [**semi-supervised**](https://developers.google.com/machine-learning/glossary#semi-supervised_learning) and [**unsupervised**](https://developers.google.com/machine-learning/glossary#unsupervised_machine_learning) learning, unlabeled examples are used during training.

Contrast unlabeled example with [**labeled example**](https://developers.google.com/machine-learning/glossary#labeled_example).

## unsupervised machine learning

\#clustering

\#fundamentals

Training a [**model**](https://developers.google.com/machine-learning/glossary#model) to find patterns in a dataset, typically an unlabeled dataset.

The most common use of unsupervised machine learning is to [**cluster**](https://developers.google.com/machine-learning/glossary#clustering) data into groups of similar examples. For example, an unsupervised machine learning algorithm can cluster songs based on various properties of the music. The resulting clusters can become an input to other machine learning algorithms (for example, to a music recommendation service). Clustering can help when useful labels are scarce or absent. For example, in domains such as anti-abuse and fraud, clusters can help humans better understand the data.

Contrast with [**supervised machine learning**](https://developers.google.com/machine-learning/glossary#supervised_machine_learning).

### Click the icon for additional notes.

## uplift modeling

A modeling technique, commonly used in marketing, that models the "causal effect" (also known as the "incremental impact") of a "treatment" on an "individual." Here are two examples:

- Doctors might use uplift modeling to predict the mortality decrease (causal effect) of a medical procedure (treatment) depending on the age and medical history of a patient (individual).
- Marketers might use uplift modeling to predict the increase in probability of a purchase (causal effect) due to an advertisement (treatment) on a person (individual).

Uplift modeling differs from [**classification**](https://developers.google.com/machine-learning/glossary#classification_model) or [**regression**](https://developers.google.com/machine-learning/glossary#regression_model) in that some labels (for example, half of the labels in binary treatments) are always missing in uplift modeling. For example, a patient can either receive or not receive a treatment; therefore, we can only observe whether the patient is going to heal or not heal in only one of these two situations (but never both). The main advantage of an uplift model is that it can generate predictions for the unobserved situation (the counterfactual) and use it to compute the causal effect.

## upweighting

Applying a weight to the [**downsampled**](https://developers.google.com/machine-learning/glossary#downsampling) class equal to the factor by which you downsampled.

## user matrix

\#recsystems

In [**recommendation systems**](https://developers.google.com/machine-learning/glossary#recommendation_system), an [**embedding vector**](https://developers.google.com/machine-learning/glossary#embedding_vector) generated by [**matrix factorization**](https://developers.google.com/machine-learning/glossary#matrix_factorization) that holds latent signals about user preferences. Each row of the user matrix holds information about the relative strength of various latent signals for a single user. For example, consider a movie recommendation system. In this system, the latent signals in the user matrix might represent each user's interest in particular genres, or might be harder-to-interpret signals that involve complex interactions across multiple factors.

The user matrix has a column for each latent feature and a row for each user. That is, the user matrix has the same number of rows as the target matrix that is being factorized. For example, given a movie recommendation system for 1,000,000 users, the user matrix will have 1,000,000 rows.

## V

## validation

\#fundamentals

The initial evaluation of a model's quality. Validation checks the quality of a model's predictions against the [**validation set**](https://developers.google.com/machine-learning/glossary#validation_set).

Because the validation set differs from the [**training set**](https://developers.google.com/machine-learning/glossary#training_set), validation helps guard against [**overfitting**](https://developers.google.com/machine-learning/glossary#overfitting).

You might think of evaluating the model against the validation set as the first round of testing and evaluating the model against the [**test set**](https://developers.google.com/machine-learning/glossary#test_set) as the second round of testing.

## validation loss

\#fundamentals

A [**metric**](https://developers.google.com/machine-learning/glossary#metric) representing a model's [**loss**](https://developers.google.com/machine-learning/glossary#loss) on the [**validation set**](https://developers.google.com/machine-learning/glossary#validation_set) during a particular [**iteration**](https://developers.google.com/machine-learning/glossary#iteration) of training.

See also [**generalization curve**](https://developers.google.com/machine-learning/glossary#generalization_curve).

## validation set

\#fundamentals

The subset of the [**dataset**](https://developers.google.com/machine-learning/glossary#dataset) that performs initial evaluation against a trained [**model**](https://developers.google.com/machine-learning/glossary#model). Typically, you evaluate the trained model against the [**validation set**](https://developers.google.com/machine-learning/glossary#validation_set) several times before evaluating the model against the [**test set**](https://developers.google.com/machine-learning/glossary#test_set).

Traditionally, you divide the examples in the dataset into the following three distinct subsets:

- a [**training set**](https://developers.google.com/machine-learning/glossary#training_set)
- a validation set
- a [**test set**](https://developers.google.com/machine-learning/glossary#test_set)

Ideally, each example in the dataset should belong to only one of the preceding subsets. For example, a single example should not belong to both the training set and the validation set.

## value imputation

The process of replacing a missing value with an acceptable substitute. When a value is missing, you can either discard the entire example or you can use value imputation to salvage the example.

For example, consider a dataset containing a `temperature` feature that is supposed to be recorded every hour. However, the temperature reading was unavailable for a particular hour. Here is a section of the dataset:

|   |   |
|---|---|
|Timestamp|Temperature|
|1680561000|10|
|1680564600|12|
|1680568200|missing|
|1680571800|20|
|1680575400|21|
|1680579000|21|

A system could either delete the missing example or impute the missing temperature as 12, 16, 18, or 20, depending on the imputation algorithm.

## vanishing gradient problem

\#seq

The tendency for the gradients of early [**hidden layers**](https://developers.google.com/machine-learning/glossary#hidden_layer) of some [**deep neural networks**](https://developers.google.com/machine-learning/glossary#deep_neural_network) to become surprisingly flat (low). Increasingly lower gradients result in increasingly smaller changes to the weights on nodes in a deep neural network, leading to little or no learning. Models suffering from the vanishing gradient problem become difficult or impossible to train. [**Long Short-Term Memory**](https://developers.google.com/machine-learning/glossary#Long_Short-Term_Memory) cells address this issue.

Compare to [**exploding gradient problem**](https://developers.google.com/machine-learning/glossary#exploding_gradient_problem).

## variable importances

\#df

A set of scores that indicates the relative importance of each [**feature**](https://developers.google.com/machine-learning/glossary#feature) to the model.

For example, consider a [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree) that estimates house prices. Suppose this decision tree uses three features: size, age, and style. If a set of variable importances for the three features are calculated to be {size=5.8, age=2.5, style=4.7}, then size is more important to the decision tree than age or style.

Different variable importance metrics exist, which can inform ML experts about different aspects of models.

## variational autoencoder (VAE)

\#language

A type of deep learning [**model**](https://developers.google.com/machine-learning/glossary#model) that is used for [**dimension reduction**](https://developers.google.com/machine-learning/glossary#dimension_reduction) and data compression. VAEs are based on variational inference: a technique for estimating the parameters of a probability model.

VAEs are composed of two [**neural networks**](https://developers.google.com/machine-learning/glossary#neural-network): an [**encoder**](https://developers.google.com/machine-learning/glossary#encoder) and a [**decoder**](https://developers.google.com/machine-learning/glossary#decoder). The encoder takes input (such as an image, sound, or text) and compresses it into a vector of latent variables. The decoder takes the vector of latent variables and reconstructs the original data. A loss is computed by comparing the original data to the reconstructed data, and the weights are updated via [**backpropagation**](https://developers.google.com/machine-learning/glossary#backpropagation) through both networks.

## W

## Wasserstein loss

One of the loss functions commonly used in [**generative adversarial networks**](https://developers.google.com/machine-learning/glossary#generative_adversarial_network), based on the [**earth mover's distance**](https://developers.google.com/machine-learning/glossary#earth-movers-distance) between the distribution of generated data and real data.

## weight

\#fundamentals

A value that a model multiplies by another value. [**Training**](https://developers.google.com/machine-learning/glossary#training) is the process of determining a model's ideal weights; [**inference**](https://developers.google.com/machine-learning/glossary#inference) is the process of using those learned weights to make predictions.

### Click the icon to see an example of weights in a linear model.

## Weighted Alternating Least Squares (WALS)

\#recsystems

An algorithm for minimizing the objective function during [**matrix factorization**](https://developers.google.com/machine-learning/glossary#matrix_factorization) in [**recommendation systems**](https://developers.google.com/machine-learning/glossary#recommendation_system), which allows a downweighting of the missing examples. WALS minimizes the weighted squared error between the original matrix and the reconstruction by alternating between fixing the row factorization and column factorization. Each of these optimizations can be solved by least squares [**convex optimization**](https://developers.google.com/machine-learning/glossary#convex_optimization). For details, see the [Recommendation Systems course](https://developers.google.com/machine-learning/recommendation/collaborative/matrix).

## weighted sum

\#fundamentals

The sum of all the relevant input values multiplied by their corresponding weights. For example, suppose the relevant inputs consist of the following:

|   |   |
|---|---|
|input value|input weight|
|2|-1.3|
|-1|0.6|
|3|0.4|

The weighted sum is therefore:

```Plain
weighted sum = (2)(-1.3) + (-1)(0.6) + (3)(0.4) = -2.0
```

A weighted sum is the input argument to an [**activation function**](https://developers.google.com/machine-learning/glossary#activation_function).

## wide model

A linear model that typically has many [**sparse input features**](https://developers.google.com/machine-learning/glossary#sparse_features). We refer to it as "wide" since such a model is a special type of [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network) with a large number of inputs that connect directly to the output node. Wide models are often easier to debug and inspect than [**deep models**](https://developers.google.com/machine-learning/glossary#deep_model). Although wide models cannot express nonlinearities through [**hidden layers**](https://developers.google.com/machine-learning/glossary#hidden_layer), wide models can use transformations such as [**feature crossing**](https://developers.google.com/machine-learning/glossary#feature_cross) and [**bucketization**](https://developers.google.com/machine-learning/glossary#bucketing) to model nonlinearities in different ways.

Contrast with [**deep model**](https://developers.google.com/machine-learning/glossary#deep_model).

## width

The number of [**neurons**](https://developers.google.com/machine-learning/glossary#neuron) in a particular [**layer**](https://developers.google.com/machine-learning/glossary#layer) of a [**neural network**](https://developers.google.com/machine-learning/glossary#neural_network).

## wisdom of the crowd

\#df

The idea that averaging the opinions or estimates of a large group of people ("the crowd") often produces surprisingly good results. For example, consider a game in which people guess the number of jelly beans packed into a large jar. Although most individual guesses will be inaccurate, the average of all the guesses has been empirically shown to be surprisingly close to the actual number of jelly beans in the jar.

[**Ensembles**](https://developers.google.com/machine-learning/glossary#ensemble) are a software analog of wisdom of the crowd. Even if individual models make wildly inaccurate predictions, averaging the predictions of many models often generates surprisingly good predictions. For example, although an individual [**decision tree**](https://developers.google.com/machine-learning/glossary#decision-tree) might make poor predictions, a [**decision forest**](https://developers.google.com/machine-learning/glossary#decision-forest) often makes very good predictions.

## word embedding

\#language

[**Representing**](https://developers.google.com/machine-learning/glossary#representation) each word in a word set within an [**embedding vector**](https://developers.google.com/machine-learning/glossary#embedding_vector); that is, representing each word as a vector of floating-point values between 0.0 and 1.0. Words with similar meanings have more-similar representations than words with different meanings. For example, _carrots_, _celery_, and _cucumbers_ would all have relatively similar representations, which would be very different from the representations of _airplane_, _sunglasses_, and _toothpaste_.

## X

## XLA (Accelerated Linear Algebra)

An open-source machine learning compiler for GPUs, CPUs, and ML accelerators.

The XLA compiler takes models from popular ML frameworks such as [PyTorch](https://pytorch.org/), [**TensorFlow**](https://developers.google.com/machine-learning/glossary#TensorFlow), and [**JAX**](https://developers.google.com/machine-learning/glossary#JAX), and optimizes them for high-performance execution across different hardware platforms including GPUs, CPUs, and ML [**accelerators**](https://developers.google.com/machine-learning/glossary#accelerator-chip).

## Z

## zero-shot learning

A type of machine learning [**training**](https://developers.google.com/machine-learning/glossary#training) where the [**model**](https://developers.google.com/machine-learning/glossary#model) infers a [**prediction**](https://developers.google.com/machine-learning/glossary#prediction) for a task that it was not specifically already trained on. In other words, the model is given zero task-specific training [**examples**](https://developers.google.com/machine-learning/glossary#example) but asked to do [**inference**](https://developers.google.com/machine-learning/glossary#inference) for that task.

## Z-score normalization

\#fundamentals

A [**scaling**](https://developers.google.com/machine-learning/glossary#scaling) technique that replaces a raw [**feature**](https://developers.google.com/machine-learning/glossary#feature) value with a floating-point value representing the number of standard deviations from that feature's mean. For example, consider a feature whose mean is 800 and whose standard deviation is 100. The following table shows how Z-score normalization would map the raw value to its Z-score:

|   |   |
|---|---|
|Raw value|Z-score|
|800|0|
|950|+1.5|
|575|-2.25|

The machine learning model then trains on the Z-scores for that feature instead of on the raw values.