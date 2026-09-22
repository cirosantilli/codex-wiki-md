<h1 id="6h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The estimator $U=X_1X_2$ is [unbiased](../../../../../../unbiased-estimator.md) for $p^2$ because the [independent random variables](../../../../../../independent-random-variables.md) $X_1,X_2$ satisfy $\mathbb E[X_1X_2]=p^2$. Given $T=t$, all placements of the $t$ successes are equally likely, so

$$
\mathbb E[X_1X_2\mid T=t]
=\frac{\binom{n-2}{t-2}}{\binom nt}
=\frac{t(t-1)}{n(n-1)}.
$$

Thus the Rao-Blackwellized estimator is

$$
\boxed{\widehat{p^2}=\frac{T(T-1)}{n(n-1)}}.
$$

It is unbiased by the tower property. Since $n\geq3$ and $p\in(0,1)$, the event $T=2$ has positive probability, and conditionally on it $X_1X_2$ takes both zero and one with positive probability. Hence $\mathbb E[\operatorname{Var}(X_1X_2\mid T)]>0$, so the new estimator has strictly smaller variance.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6H](../../6h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
