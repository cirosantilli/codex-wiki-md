<h1 id="6a/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The infective equation is

$$
Y'=Y\{\beta X-(\mu+\nu)\}.
$$

Since $X\leq N$, the threshold population is

$$
N_c=\frac{\mu+\nu}{\beta}.
$$

If $N<N_c$ and $\delta=\mu+\nu-\beta N>0$, then

$$
Y'\leq-\delta Y,
\qquad Y(t)\leq Y(0)e^{-\delta t}\longrightarrow0.
$$

Also

$$
Z(t)=e^{-\mu t}Z(0)+\nu\int_0^t e^{-\mu(t-s)}Y(s)\,ds\longrightarrow0.
$$

Any steady state with $Y>0$ would require $X=N_c>N$, which is impossible. Thus the infection cannot be maintained, and both infected and immune populations tend to zero from every admissible initial condition.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6A](../../6a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
