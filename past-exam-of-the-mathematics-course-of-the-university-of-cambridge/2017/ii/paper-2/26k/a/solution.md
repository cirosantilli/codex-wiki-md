<h1 id="26k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $r=1-\alpha\in(0,1)$. The variable $Y=X_1-\theta$ has density $ry^{r-1}$ on $(0,1)$, so $\mathbb EY^j=r/(r+j)$. Thus

$$
\boxed{\mathbb EX_1=\theta+\frac r{r+1},\qquad
\operatorname{Var}(X_1)=\frac r{(r+2)(r+1)^2}.}
$$

The [unbiased estimator](../../../../../../unbiased-estimator.md) is

$$
\boxed{\widetilde\theta_n=\overline X_n-\frac{1-\alpha}{2-\alpha},\qquad c(\alpha)=-\frac{1-\alpha}{2-\alpha}.}
$$

Taking [expectations](../../../../../../expected-value.md) verifies that its [bias](../../../../../../bias-of-an-estimator.md) is zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [26K](../../26k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
