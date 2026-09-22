<h1 id="o/o2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the full-column-rank [design matrix](../../../../../../design-matrix.md), the normal-error [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is the least-squares estimator

$$
\boxed{\widehat\theta=(X^TX)^{-1}X^TY.}
$$

Indeed maximizing the Gaussian likelihood over $\theta$ minimizes $\|Y-X\theta\|^2$, whose [normal equations](../../../../../../normal-equation.md) are $X^TX\widehat\theta=X^TY$; rank $p$ makes $X^TX$ invertible. Substitution of the model gives

$$
\widehat\theta=\theta+(X^TX)^{-1}X^T\epsilon.
$$

Since $\mathbb E\epsilon=0$, it follows that $\boxed{\mathbb E\widehat\theta=\theta}$, proving unbiasedness.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [A](../../a.md)
3. [O2](../../../o2.md)
4. [O](../../../../o.md)
5. [2012](../../../../../2012-split.md)
6. [Past exam of the options I course of the University of Oxford](../../../../../split.md)
7. [Options I course of the University of Oxford](../../../../../../options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
