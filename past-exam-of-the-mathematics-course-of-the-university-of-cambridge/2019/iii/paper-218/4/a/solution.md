<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[LDA](../../../../../../linear-discriminant-analysis.md) assumes $Y\in\{1,\ldots,L\}$ with prior probabilities $\pi_l>0$ and

$$
X\mid Y=l\sim N_p(\mu_l,\Sigma),
$$

where the class means may differ but the nonsingular covariance matrix is common. Bayes' rule chooses the class maximizing $\log\pi_l+\log f_l(x)$. Cancelling terms common to every class gives the discriminant

$$
\delta_l(x)=x^T\Sigma^{-1}\mu_l
-\frac12\mu_l^T\Sigma^{-1}\mu_l+\log\pi_l.
$$

The boundary between classes $l$ and $m$ is $\delta_l(x)=\delta_m(x)$, an affine hyperplane with normal $\Sigma^{-1}(\mu_l-\mu_m)$. Hence the Bayes rule $\arg\max_l\delta_l(x)$ is a linear classifier.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
