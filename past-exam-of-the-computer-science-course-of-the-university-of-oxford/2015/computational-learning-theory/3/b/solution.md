<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [weighted decision stump optimization](../../../../../weighted-decision-stump-optimization.md) with the convention $\operatorname{sign}(0)=+1$, and write $w_j=D((x_j,y_j))$. For each coordinate $i$, sort the examples by their $i$th coordinate and group all equal coordinate values. For a threshold between the $k$th and $(k+1)$st distinct values, the [decision stump](../../../../../decision-stump.md) predicts $-1$ on the left and $+1$ on the right. Its weighted [misclassification risk](../../../../../misclassification-risk.md) is

$$
\boxed{E_i(k)=\sum_{j\text{ left},\ y_j=+1}w_j
+\sum_{j\text{ right},\ y_j=-1}w_j.}
$$

Start with a threshold below the minimum observed value. Every prediction is then $+1$, and the initial error is $\sum_{y_j=-1}w_j$. Sweep the threshold from left to right. When it passes an entire group $G$ of equal coordinate values, that group's prediction changes from $+1$ to $-1$, so update

$$
\boxed{E\leftarrow E+\sum_{j\in G,\ y_j=+1}w_j-\sum_{j\in G,\ y_j=-1}w_j.}
$$

Record the smallest value and a threshold achieving it, including the final threshold above all observations, which predicts $-1$ everywhere on the sample. Representatives can be chosen strictly between successive distinct values; the two outer representatives are finite real numbers below the minimum and above the maximum.

Every threshold has exactly the same sample predictions as one of these representatives. In particular, if a threshold equals an observed value, the equality group is on the $+1$ side under the chosen [sign function](../../../../../sign-function.md) convention, which duplicates the representative immediately before that group. Thus the sweep includes every possible sample labelling by the stated [decision stump](../../../../../decision-stump.md). Repeating for all $n$ coordinates and returning the globally smallest error proves optimality.

Sorting costs $O(m\log m)$ per coordinate and the grouped sweep costs $O(m)$. The overall [time complexity](../../../../../time-complexity.md) is

$$
\boxed{O(nm\log m),}
$$

with $O(m)$ working storage when coordinates are processed one at a time. Pre-sorted coordinate orders can be reused across repeated [AdaBoost](../../../../../adaboost.md) rounds, leaving $O(nm)$ work per round for changing weights. The paper allows only the orientation $\operatorname{sign}(x_i-b)$; reversing its polarity would enlarge the [hypothesis class](../../../../../concept-class.md) and is unnecessary here.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
