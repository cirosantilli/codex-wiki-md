<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $S_0>0$, the [stochastic exponential](../../../../../../doleans-dade-exponential.md) solution stays strictly positive. Put $U_t=\sqrt{S_t}$. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
\boxed{dU_t=\frac12U_t\sigma_t\,dW_t-\frac18U_t\sigma_t^2\,dt.}
$$

Thus $U$ is a nonnegative local [supermartingale](../../../../../../supermartingale.md). To justify the true [supermartingale](../../../../../../supermartingale.md) property, stop where $U$ or its stochastic integral exceeds successive bounds. The stopped [Itô formula](../../../../../../ito-s-lemma.md) gives $\mathbb E[U_{T\wedge\tau_m}\mid\mathcal F_t]\leq U_{t\wedge\tau_m}$ for $T\geq t$. The conditional [Fatou lemma](../../../../../../fatou-s-lemma.md) and $\tau_m\uparrow\infty$ yield

$$
\boxed{\mathbb E[U_T\mid\mathcal F_t]\leq U_t.}
$$

In particular $\mathbb EU_T\leq U_0<\infty$. The case $S_0=0$ is the identically zero process. This is the [square-root stock supermartingale](../../../../../../square-root-stock-supermartingale.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
