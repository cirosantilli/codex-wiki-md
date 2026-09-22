<h1 id="19h/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Minimizing $\|Y-X\theta\|^2$ gives the [normal equations](../../../../../../normal-equation.md) $X^TX\widehat\theta=X^TY$. Full column rank makes $X^TX$ invertible, so

$$
\boxed{\widehat\theta=(X^TX)^{-1}X^TY.}
$$

With the [hat matrix](../../../../../../hat-matrix.md) $H=X(X^TX)^{-1}X^T$, the residual is $\widehat\varepsilon=(I-H)\varepsilon$. The symmetric projection $I-H$ has rank $n-p$, hence

$$
\boxed{\frac{\widehat\varepsilon^T\widehat\varepsilon}{\sigma^2}
\sim\chi^2_{n-p},\qquad
\widehat{\sigma}^2=\frac{\widehat\varepsilon^T\widehat\varepsilon}{n-p}}
$$

and the latter estimator is unbiased.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
