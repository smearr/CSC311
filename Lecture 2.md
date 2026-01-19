
# Decision Trees

Series of nested if/else statements

We use a greedy approach to construct decision trees. 
- Start with the whole training set and an empty decision tree.
- Pick a feature and candidate split that would most reduce a loss.
- Split on that feature and recurse on subpartitions.

# Information Theory


## Entropy - Quantifying Uncertainty

In statistics, the entropy of a discrete random variable is a number that quantifies the uncertainty inherent in its possible outcomes: $$H(X) = -\sum_{x \in X} p(x)\cdot log_{2}p(x)$$
### Example:

What is the entropy of a loaded coin with probability $p = \frac{2}{18} = \frac{1}{9}$? What about $p = \frac{10}{18}$?

$$-\frac{8}{9}\log_2\frac{8}{9} -\frac{1}{9}\log_2\frac{1}{9} \approx \frac{1}{2}$$
is the uncertainty of a loaded coin with probability 1/9. Coins with a lower entropy have a more certain outcome.

# Entropy of a Joint Distribution

$$H(X) = -\sum_{x \in X}\sum_{y \in Y} p(x,y)\log_2p(x,y)$$
# Conditional Entropy and Expected Conditional Entropy
$$H(X) = -\sum_{x \in X}\sum_{y \in Y} p(x,y)\log_2p(y|x)$$
![[Pasted image 20260118210330.png]]
![[Pasted image 20260118221254.png]]
