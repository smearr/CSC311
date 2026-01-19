
#### AI vs ML vs DL

Artificial Intelligence: Create intelligent machines that perceive, reason, and act like humans.

Machine Learning: Build algorithms that process and learn from data.

Deep Learning: Using deep neural networks to automatically learn from data.


#### Types of Machine Learning Problems

- Supervised Learning: have labeled examples of the correct behaviour, input/output response data.
	- Regression (height prediction)
	- classification (sentiment classifcation)
- Unsupervised Learning: no labeled examples, instead looking for patterns in data. (clustering)
- Reinforcement Learning: learning system receives a reward for correct trial and errors.

#### Supervised Learning

##### Examples
- Age prediction:
	- Input: portrait of a person
	- output: their age

##### Notation Input

**Input**: represented via a vector $x \in \mathbb{R}^{D}$
$$x = \begin{pmatrix}
x_{1} \\
x_{2} \\
\vdots \\ 
x_{D}
\end{pmatrix}
$$
Each scalar $x_i$ in the the vector x is a feature, a numerical value describing the input or the feature that the model uses to guess the output. 
###### Example 1:

| Fruit  | W   | H   |
| ------ | --- | --- |
| Orange | 6.8 | 7.4 |
| Orange | 7.1 | 7.5 |
| Orange | 7.6 | 7.8 |
| Orange | 7.2 | 7.2 |
| Lemon  | 7.2 | 9.3 |
| Lemon  | 7.3 | 9.5 |
The $D$ in this example is $D=2$. $x = \begin{matrix} 6.8 \\ 7.4 \end{matrix}$

##### Notation Output 

**Target Output:** represented with $t$.
- In regression, t is a real number (stock price)
- In classification, t is an element of a discrete set.

**Predicted Output**: represented with $y$.

###### Training Data Set

The training data set consists of (input, target output) example pairs or ($x^{(1)}$, $t^{(1)}$). The superscripts represent indices of the data. and the subscript is the index of the vector data. i.e. $x^{1}_{2}$


###### Supervised Learning Models

**Hypothesis:** is a specific function of $f$, that maps x to an output prediction y.

**Learning:** is the process of choosing a hypothesis $f$ using the training data. 

**Inference:** is the process of using a hypothesis f, to make predictions.
![[Pasted image 20260118144304.png]]

###### Accuracy and Error

Accuracy = $\frac{\text{Num Correct Predictions}}{\text{Num total predictions}}$
Error = 1 - Accuracy


#### Nearest Neighbours

#### 1-NN

The boundary is where a point is **equally close to two training points of different classes**.

#### K-NN

The boundary where k points are equally close to two training points of different classes.



#### Terminology
- Decision Boundary: Set of points in the input space x ∈ RD where a classifier’s output is ambiguous.
- Accuracy: The percentage of correctly classified data points over some labelled data set.
- Error: The percentage of incorrectly classified data points over some labelled data set.
- Training Set: A subset of the labelled data points used for learning a hypothesis.
- Validation Set: A subset of the labelled data points set aside for choosing/tuning hyperparameters.
- Test Set: A subset of the labelled data points set aside for estimating how well a model generalizes to unseen data. To achieve a good estimate, this data set should not be used to make any decisions about the model, and should ideally be used only once.

#### Choosing K

If k is too small, we are overfitting the data and the model will be sensitive to outliers.

If k is too large, we are underfitting the data and the model will be too simple and fail to capture important regularities.

Balancing K requires using the validation set to tune the hyperparameter

Nearest neighbours can be sensitive to the ranges of different features. So we normalize each dimension to be zero mean and unit variance. Normalize.





