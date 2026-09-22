<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The response is the species [categorical variable](../../../../../categorical-variable.md), while the four measurements are candidate predictors. The dot in the formula means all other columns of the data frame. The fitted object is a [classification tree](../../../../../classification-tree.md): it recursively partitions predictor space by binary threshold rules and assigns a species and class-probability vector to each terminal region. Sepal width was available but was not selected in the displayed tree.

At a node $t$, let $n_{tk}$ be the number of observations of class $k$ and $n_t=\sum_kn_{tk}$. The [multinomial likelihood](../../../../../multinomial-likelihood.md) is maximized by $\widehat p_{tk}=n_{tk}/n_t$. The fitted class is one attaining the largest proportion, with a software convention resolving ties. The [classification-tree deviance](../../../../../classification-tree-deviance.md) is

$$
D(t)=-2\sum_kn_{tk}\log\widehat p_{tk},\qquad0\log0=0.
$$

A pure node has zero deviance. At each nonterminal node, consider candidate split points between distinct observed predictor values, and choose the split with the largest decrease $D(t)-D(t_L)-D(t_R)$. Repeating this local maximization constructs a binary [decision tree](../../../../../decision-tree.md); it does not solve a global optimization over all trees. Growth stops when nodes are pure or size/deviance controls prohibit further splitting. Mixed leaves with five or six observations can therefore remain. The node number $j$ has children $2j$ and $2j+1$, and a terminal-node marker means that no further split was retained.

The [probability](../../../../../probability.md) triples are in class order $(c,s,v)$, not $(s,c,v)$. For example, the pure left leaf has [probability](../../../../../probability.md) vector $(0,1,0)$ and predicts $s$, while the 54-observation node has counts $(49,0,5)$ and predicts $c$. The root counts are $(50,50,50)$, giving $D=300\log3\simeq329.584$ and a tied majority class. Its reported choice of $c$ does not indicate a more common class.

The complete derived decision rule is shown below. Each leaf includes its fitted class and the observed class counts, so both the branching logic and its remaining errors are visible. For the observed data, the printed strict inequalities leave no equality cases because the thresholds fall between measurement values. A consistent right-branch convention at equality extends the rule to new specimens.

<a id="3/image-six-leaf-iris-classification-tree-with-fitted-classes-and-class-counts-at-every-terminal-node"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-39-iris-tree.png)

**[Figure 1](#3/image-six-leaf-iris-classification-tree-with-fitted-classes-and-class-counts-at-every-terminal-node). Six-leaf iris classification tree with fitted classes and class counts at every terminal node**.

The six terminal nodes contain the class counts

$$
\begin{array}{c|r|rrr|c|r}
\text{node}&n&c&s&v&\text{prediction}&\text{errors}\\\hline
2&50&0&50&0&s&0\\
24&5&4&0&1&c&1\\
25&43&43&0&0&c&0\\
13&6&2&0&4&v&2\\
14&6&1&0&5&v&1\\
15&40&0&0&40&v&0
\end{array}
$$

Thus the training [misclassification error](../../../../../misclassification-rate.md) is

$$
\boxed{\frac{1+2+1}{150}=\frac4{150}\simeq0.02667.}
$$

The terminal [classification-tree deviance](../../../../../classification-tree-deviance.md) is instead

$$
\begin{aligned}
D_{\mathrm{tree}}={}&-2\left(4\log\frac45+\log\frac15\right)
-2\left(2\log\frac26+4\log\frac46\right)\\
&-2\left(\log\frac16+5\log\frac56\right)
\simeq5.004+7.638+5.407=18.049.
\end{aligned}
$$

The displayed residual mean deviance divides this by $150-6=144$, yielding approximately $0.1253$. This is the summary's reporting convention, not a normal-error residual mean square or an automatic chi-squared calibration with 144 [statistical degrees of freedom](../../../../../statistical-degrees-of-freedom.md). The two summary measures answer different questions: deviance depends on the fitted [probability](../../../../../probability.md) of each observed class, while misclassification counts only whether the majority-class prediction is correct. Both are training quantities. [Cross-validation](../../../../../cross-validation.md) or independent test data, rather than the displayed training error, are needed to assess prediction on new specimens; [cost-complexity tree pruning](../../../../../cost-complexity-tree-pruning.md) can select a less elaborate tree if predictive performance warrants it.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
