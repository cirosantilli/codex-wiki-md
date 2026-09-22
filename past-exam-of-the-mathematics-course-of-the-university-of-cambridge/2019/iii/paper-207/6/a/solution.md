<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [frailty random variable](../../../../../../frailty-random-variable.md) is an unobserved positive multiplicative risk factor. A proportional frailty model has

$$
h(t\mid U)=Uh_0(t),
\qquad
S(t\mid U)=e^{-UH_0(t)}.
$$

The scale of $U$ is not separately identifiable from $h_0$: multiplying $U$ by a constant and dividing $h_0$ by it leaves the model unchanged. We may therefore normalize $\mathbb EU=1$, which lets $h_0$ represent the mean initial hazard multiplier and makes relative frailty interpretable.

If $U\sim\operatorname{Exponential}(1)$ and $h_0(t)=\lambda$, then the [Laplace transform](../../../../../../laplace-transform.md) of $U$ gives

$$
S(t)=\mathbb E[e^{-U\lambda t}]
=\frac1{1+\lambda t},
\qquad
h(t)=-\frac d{dt}\log S(t)
=\boxed{\frac\lambda{1+\lambda t}}.
$$

Thus $h(0)=\lambda$, while $h(t)\to0$ as $t\to\infty$. Survivors become increasingly enriched for low-frailty individuals.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
