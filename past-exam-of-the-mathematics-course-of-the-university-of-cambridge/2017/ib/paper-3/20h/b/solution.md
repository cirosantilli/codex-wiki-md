<h1 id="20h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the one-column design as $x\in\mathbb R^n\setminus\{0\}$ and $S=x^Tx$. Maximizing the [normal linear model](../../../../../../normal-linear-model.md) likelihood first gives $\widehat\beta=x^TY/S$. Its minimized [residual sum of squares](../../../../../../residual-sum-of-squares.md) is $R=\|Y-x\widehat\beta\|^2$. For variance $v>0$, the remaining log likelihood is $-\tfrac n2\log v-R/(2v)$ plus a constant, whose maximum is at

$$
\boxed{\widehat\sigma^2=\frac Rn.}
$$

Here $R>0$ almost surely because $n>1$ and the true variance is positive. In the exceptional data case $R=0$, the likelihood is unbounded as $v\downarrow0$, so there is no positive-variance maximum.

Let $P=xx^T/S$, the [orthogonal projection matrix](../../../../../../orthogonal-projection-matrix.md) onto the design column. Then $\widehat\beta-\beta=x^T\varepsilon/S$ and $Y-x\widehat\beta=(I-P)\varepsilon$. These are orthogonal linear projections of an isotropic [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md), hence independent. An orthonormal coordinate system adapted to $x$ makes the residual squared length a sum of $n-1$ independent squared standard normals. Thus the [joint distribution of least-squares and variance estimators](../../../../../../joint-distribution-of-least-squares-and-variance-estimators.md) is the product law

$$
\boxed{\widehat\beta\sim N\!\left(\beta,\frac{\sigma^2}{S}\right),\qquad \frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-1},\qquad\widehat\beta\ \text{and}\ \widehat\sigma^2\ \text{are independent}.}
$$

In particular the maximum likelihood variance estimator is biased: $\mathbb E\widehat\sigma^2=(n-1)\sigma^2/n$; the unbiased residual estimator uses denominator $n-1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [20H](../../20h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
