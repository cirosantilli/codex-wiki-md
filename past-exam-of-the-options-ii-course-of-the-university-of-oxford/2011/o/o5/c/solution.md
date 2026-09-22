<h1 id="o/o5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the residual mean square

$$
\boxed{s^2=\frac{\|Y-X\widehat\theta\|^2}{n-p}.}
$$

To justify its denominator, let $H=X(X^TX)^{-1}X^T$, the [orthogonal projection matrix](../../../../../orthogonal-projection-matrix.md) onto the column space of $X$. Then the residual is $(I-H)\epsilon$. The [idempotent matrix](../../../../../idempotent-matrix.md) $I-H$ has rank $n-p$, so diagonalizing it with an [orthogonal matrix](../../../../../orthogonal-matrix.md) gives

$$
\frac{\|Y-X\widehat\theta\|^2}{\sigma^2}\sim\chi^2_{n-p}.
$$

Consequently $\mathbb Es^2=\sigma^2$, making $s^2$ an [unbiased estimator](../../../../../unbiased-estimator.md). If specifically asked for [maximum likelihood estimation](../../../../../maximum-likelihood-estimation-split.md), maximizing over $\sigma^2$ gives the alternative $\widehat\sigma^2_{\rm ML}=\|Y-X\widehat\theta\|^2/n$, which is biased downward by the factor $(n-p)/n$.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [O5](../../o5.md)
3. [O](../../../o.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the options II course of the University of Oxford](../../../../split.md)
6. [Options II course of the University of Oxford](../../../../../options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
