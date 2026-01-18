
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

