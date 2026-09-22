<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The formula makes species the categorical response and the dot denotes all four other columns as candidate predictors. The [classification tree](../../../../../classification-tree.md) is grown by recursive binary partitioning, not by fitting a [linear regression](../../../../../linear-regression-split.md) to numerical species codes. At a node $t$, count observations of each class, $n_{tk}$, and set $\widehat p_{tk}=n_{tk}/n_t$. These are the multinomial maximum-likelihood probabilities. The [classification-tree deviance](../../../../../classification-tree-deviance.md) is

$$
D(t)=-2\sum_kn_{tk}\log\widehat p_{tk},\qquad0\log0=0.
$$

For each candidate predictor and threshold, calculate $D(t)-D(t_L)-D(t_R)$ and choose the largest permitted decrease. Continue recursively until a node is pure or the stopping controls prevent another split, for example because it has too few observations or insufficient deviance to warrant further growth. Only petal length, petal width and sepal length appear in the selected splits; sepal width was available but did not win a split. This greedy construction need not find a globally optimal tree. The default deviance criterion and [recursive partitioning](../../../../../recursive-partitioning.md) are documented in the [tree package manual](https://cran.r-project.org/web/packages/tree/tree.pdf).

Each node number encodes its position: node $j$ has left and right children $2j$ and $2j+1$. The reported sample size is the number reaching the node; its deviance is calculated from that node's class counts. The fitted class is the class with largest fitted probability, with a convention resolving ties. The root's three counts are equal, so its displayed class is only a tie choice. An asterisk marks a terminal node, where prediction stops.

The resulting rule is displayed below. A left edge satisfies the stated strict inequality and a right edge its complement. None of the recorded training values lies exactly at these midpoint thresholds; the diagram adopts the right branch at equality for prediction.

<a id="3/image-the-fitted-six-leaf-iris-classification-tree-with-split-thresholds-and-training-errors"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-46-classification-tree.png)

**[Figure 1](#3/image-the-fitted-six-leaf-iris-classification-tree-with-split-thresholds-and-training-errors). The fitted six-leaf iris classification tree, with split thresholds and training errors**.

Its six terminal regions have the following derived class counts, in the order setosa, versicolor, virginica:

$$
\begin{array}{c|c|c|c}
\text{node}&\text{class counts}&\text{predicted class}&\text{errors}\\\hline
2&(50,0,0)&\text{setosa}&0\\
24&(0,4,1)&\text{versicolor}&1\\
25&(0,43,0)&\text{versicolor}&0\\
13&(0,2,4)&\text{virginica}&2\\
14&(0,1,5)&\text{virginica}&1\\
15&(0,0,40)&\text{virginica}&0
\end{array}
$$

The root split identifies all 50 setosa observations. Among the remaining specimens, the petal-width split is the principal separation of versicolor from virginica; further petal-length and sepal-length splits refine it. The leaf errors add to **$4/150\simeq2.67\%$**. The leaf deviances add to

$$
5.0040+7.6382+5.4067\simeq18.0489.
$$

Dividing by the software's residual degrees-of-freedom convention $150-6=144$ gives **$18.0489/144\simeq0.1253$**, as reported. The root deviance is $-2(150)\log(1/3)=300\log3\simeq329.6$. The deviance is a [likelihood](../../../../../likelihood-function.md) measure, whereas the error rate counts wrong majority-class predictions; these are different fit summaries.

Both quantities are in-sample, so the low error does not establish prediction accuracy on new specimens. [Cost-complexity tree pruning](../../../../../cost-complexity-tree-pruning.md), with tree size chosen by [cross-validation](../../../../../cross-validation.md), can remove weak splits and reduce [overfitting](../../../../../overfitting.md). An [independent](../../../../../independent-random-variables.md) [test set](../../../../../test-set.md) is needed for a final estimate of the selected tree's [prediction error](../../../../../prediction-error.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
