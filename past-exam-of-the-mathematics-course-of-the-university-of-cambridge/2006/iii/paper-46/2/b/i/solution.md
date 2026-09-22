<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use a [multivariate normal distribution](../../../../../../../multivariate-normal-distribution.md) within each species, a common positive-definite [covariance matrix](../../../../../../../covariance-matrix.md), equal [prior odds](../../../../../../../prior-odds.md) and equal misclassification costs. Assume the training observations are independent and representative of the populations. Substituting the [sample means](../../../../../../../sample-mean.md) and pooled [sample covariance matrix](../../../../../../../sample-covariance-matrix.md) gives a fitted [linear discriminant analysis](../../../../../../../linear-discriminant-analysis.md) rule, rather than a rule with known population parameters.

The determinant of the pooled covariance is $8$, so

$$
S^{-1}=\frac18\begin{pmatrix}4&2\\2&3\end{pmatrix},\qquad
L=S^{-1}(\bar x_f-\bar x_a)=\begin{pmatrix}1/2\\-5/4\end{pmatrix}.
$$

The midpoint of the [sample means](../../../../../../../sample-mean.md) is $(4,6)^T$, whose scalar product with $L$ is $-11/2$. Hence the fitted log [likelihood ratio](../../../../../../../likelihood-ratio.md) is

$$
\boxed{q(x)=\frac12x_1-\frac54x_2+\frac{11}{2}=\frac{2x_1-5x_2+22}{4}.}
$$

**Assign fattus when $q(x)>0$ and apathus when $q(x)<0$; either assignment is optimal on $q(x)=0$ under equal priors.** The separating line is $x_2=0.4x_1+4.4$, with fattus below it. As a sign check, the scores at the two [sample means](../../../../../../../sample-mean.md) are $19/4$ and $-19/4$, respectively. This uses the corrected [Gaussian Bayes classifier](../../../../../../../gaussian-bayes-classifier.md) from (a).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [Paper 46](../../../../paper-46-split.md)
5. [Iii](../../../../split.md)
6. [2006](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
