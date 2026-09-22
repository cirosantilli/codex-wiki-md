<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The inequality in the printed rule is reversed. With the stated definition of $L$, a larger score favors group one. For example, in one dimension take $\mu_1=1$, $\mu_2=-1$, $\Sigma=1$, equal priors and $x=1$. The score is $2$, and $f_1(1)>f_2(1)$, whereas the printed rule assigns group two. The correct [Bayes classifier](../../../../../../bayes-classifier.md) follows from minimizing the error cost as follows.

Let $R$ be the region assigned to group one, let $f_i$ be its [multivariate normal density](../../../../../../multivariate-normal-density.md), and let each misclassification cost $c>0$, with zero cost for correct classification. The expected cost is

$$
c\left[\pi_1\int_{R^c}f_1(x)\,dx+\pi_2\int_Rf_2(x)\,dx\right]
=c\pi_1+c\int_R\bigl[\pi_2f_2(x)-\pi_1f_1(x)\bigr]\,dx.
$$

The permitted integral-minimization result therefore selects $R=\{x:\pi_1f_1(x)>\pi_2f_2(x)\}$. Points of equality may be assigned to either group without changing the risk. Equivalently, the [Bayes classifier](../../../../../../bayes-classifier.md) chooses the larger posterior probability.

For positive priors and a common positive-definite [covariance matrix](../../../../../../covariance-matrix.md), the normalization constants cancel in the [likelihood ratio](../../../../../../likelihood-ratio.md). Expanding the two quadratic forms gives

$$
\begin{aligned}
\log\frac{f_1(x)}{f_2(x)}
&=-\frac12\left[(x-\mu_1)^T\Sigma^{-1}(x-\mu_1)-(x-\mu_2)^T\Sigma^{-1}(x-\mu_2)\right]\\
&=(\mu_1-\mu_2)^T\Sigma^{-1}x-\frac12(\mu_1-\mu_2)^T\Sigma^{-1}(\mu_1+\mu_2)\\
&=L^Tx-\frac12L^T(\mu_1+\mu_2).
\end{aligned}
$$

Thus the correct [Gaussian Bayes classifier](../../../../../../gaussian-bayes-classifier.md), choosing group one on ties, is

$$
\boxed{\text{choose group 1 if }L^Tx-\tfrac12L^T(\mu_1+\mu_2)\geq\log(\pi_2/\pi_1);\quad\text{otherwise choose group 2}.}
$$

This proves the intended classification result with the necessary correction. Equal error costs remove $c$ from the decision, while [prior odds](../../../../../../prior-odds.md) determine the threshold.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
