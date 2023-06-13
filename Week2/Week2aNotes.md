# Machine Learning Paradigms
1.  Supervised Learning: In supervised learning, the algorithm is trained on a labeled dataset, which means each example in the dataset includes both the input features and the corresponding correct output (target variable or label). The goal of supervised learning is to learn a mapping from input features to output labels so that the algorithm can make accurate predictions on new, unseen data.
> [!example] A supervised learning algorithm could be trained to predict a student's proficiency level in English based on features such as vocabulary knowledge, grammar test scores, and listening comprehension. The training dataset would consist of student profiles with known proficiency levels (e.g., beginner, intermediate, advanced).
>Example 2: A supervised learning algorithm might be used to predict whether an email is spam or not based on features like the subject line and email content. The training dataset would consist of emails with known spam or non-spam labels.

2.  Unsupervised Learning: In unsupervised learning, the algorithm is trained on an unlabeled dataset, meaning the input data has no associated output labels. The goal of unsupervised learning is to discover underlying patterns or structures in the data, such as grouping similar data points together (clustering) or reducing the dimensionality of the data (dimensionality reduction).
> [!example] An unsupervised learning algorithm might be used to group students into different learning styles or profiles based on their performance and preferences across various learning activities (e.g., reading, listening, speaking, and writing), without any prior information about the students' learning styles. The algorithm would need to find patterns and relationships within the performance data itself.
Example 2: An unsupervised learning algorithm might be used to group news articles into topics based on their content, without any prior information about the topic of each article. The algorithm would need to find patterns and relationships within the text data itself.

3.  Reinforcement Learning: Reinforcement learning is a type of machine learning where an agent learns to make decisions by interacting with an environment. The agent receives feedback in the form of rewards or penalties and aims to maximize the cumulative reward over time. The learning process involves exploring the environment, trying different actions, and updating the agent's knowledge based on the feedback received.
> [!example] A reinforcement learning algorithm could be employed to personalize a language learning app for each student. The algorithm would adapt the content and difficulty of the exercises based on the student's performance and learning progress, receiving positive feedback when the student successfully completes a task and negative feedback when the student struggles or disengages.
Example 2: A reinforcement learning algorithm might be used to train a robot to navigate through a maze. The robot would learn by trial and error, receiving a positive reward when it reaches the goal and a negative reward when it hits a wall or takes too long to find the goal.

4.  Semi-Supervised Learning: Semi-supervised learning is a combination of supervised and unsupervised learning, where the algorithm is trained on a dataset that includes both labeled and unlabeled data. The goal is to leverage the unlabeled data to improve the performance of the model, especially when labeled data is scarce or expensive to obtain.
> [!example] In a semi-supervised learning scenario for automated essay grading, an algorithm could be trained on a small dataset of essays with known grades and a larger dataset of unlabeled essays. The algorithm would use the labeled data to learn the relationship between essay content and grade, while also leveraging the information in the unlabeled data to refine its understanding of the underlying patterns and improve its grading accuracy.
Example 2: In a semi-supervised learning scenario for sentiment analysis, an algorithm could be trained on a small dataset of movie reviews with known sentiment labels (positive or negative) and a larger dataset of unlabeled reviews. The algorithm would use the labeled data to learn the relationship between review content and sentiment, while also leveraging the information in the unlabeled data to refine its understanding of the underlying patterns.


# Machine Learning Inputs / Feature Types

Numerical: These are quantitative data and involve measures or counts, such as height or salary. They can be represented as integers or real numbers.

Categorical: These are qualitative data which take on a fixed number of classes or categories. They are further divided into nominal (no order implied, e.g., car colors) and ordinal features (order matters, e.g., movie ratings).

Ordinal: These are a type of categorical feature where the order among the values is significant, such as 'low', 'medium', 'high'.

Binary: A special case of categorical features where a variable only has two categories, e.g., 'Yes'/'No', 'True'/'False'.

Time-series: These are a collection of data points collected at constant time intervals. These are important in forecasting, trend analysis, etc.

# Machine Learning Supervised Learning Tasks

Classification: The task of predicting a discrete class label. For example, determining whether an email is spam or not.

Regression: The task of predicting a continuous quantity. For example, predicting the price of a house based on different features like area, location, number of rooms, etc.

Ranking: The task of ordering entities from the ones most likely to be positive to the ones least likely to be positive. For example, page ranking used in search engines.

Anomaly Detection: Although this can be unsupervised, supervised anomaly detection involves training a model on a normal behavior and predicting anomalies based on that.

Sequence Prediction: Predicting the next value in a sequence, like the next word in a sentence or the stock market's status tomorrow.

# Machine Learning Unsupervised Learning Tasks

Clustering: The task of grouping a set of objects in such a way that objects in the same group are more similar to each other than to those in other groups.

Dimensionality Reduction: The task of reducing the number of random variables under consideration, by obtaining a set of principal variables.

Association Rule Learning: The task of discovering interesting relations between variables in large databases. A typical example of this is market basket analysis.

Anomaly Detection: Identifying unusual data points in your dataset. It's useful in identifying fraud, detecting unusual behavior, etc.


# One-Hot Encoding: 
This is a process of converting categorical data variables so they can be provided to machine learning algorithms to improve predictions. With one-hot, we convert each categorical value into a new categorical column and assign a binary value of 1 or 0. Each integer value is represented as a binary vector. All the values are zero, and the index is marked with a 1.

Example: If we have a 'color' feature with three categories 'red', 'green', 'blue'. In one-hot encoding, it will be represented as:

'red' -> [1, 0, 0]

'green' -> [0, 1, 0]

'blue' -> [0, 0, 1]

# Normalization: 
 is a scaling technique in which values are shifted and rescaled so that they end up ranging between 0 and 1. It is also known as Min-Max scaling. It's essential when features have different ranges and scales, as many machine learning algorithms perform better when numerical input variables are scaled to a standard range.

Formula: Xnew = (X - Xmin) / (Xmax - Xmin)

Where Xnew is the normalized value, X is the original value, Xmin is the smallest value in the feature column, and Xmax is the largest value.