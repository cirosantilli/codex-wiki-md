<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Strong Markov property](../../../../../../strong-markov-property.md) and part (b) show that, before $\tau=\tau_x\wedge\tau_y$,

$$
F(V_t)=\mathbb P(\tau_x>\tau_y\mid\mathcal F_t).
$$

Thus $F(V_{t\wedge\tau})$ is a bounded [martingale](../../../../../../martingale-split.md). From the given stochastic differential equation,

$$
d[V]_t=\frac{(1-V_t)^2}{Y_t^2}dt.
$$

The [Itô formula](../../../../../../ito-s-lemma.md) says that the drift of $F(V_t)$ is

$$
\frac1{2Y_t^2}\left[(1-v)^2F''(v)+\left(\frac{d-1}{v}+(3-d)v-2\right)F'(v)\right]_{v=V_t}dt.
$$

It must vanish. Dividing by $(1-v)^2/2$ and using the algebraic identity supplied in the question gives

$$
\boxed{F''(v)+\left(\frac{d-1}{v}+\frac{2d-4}{1-v}\right)F'(v)=0,
\qquad v<0.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
