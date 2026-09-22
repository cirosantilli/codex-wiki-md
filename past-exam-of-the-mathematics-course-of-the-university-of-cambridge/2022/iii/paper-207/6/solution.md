<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

A [proportional frailty model](../../../../../proportional-frailty-model.md) specifies

$$
h(t\mid U=u)=u h_0(t),
\qquad
S(t\mid U=u)=e^{-uH_0(t)}.
$$

Its population [survival function](../../../../../survival-function.md) is the [Laplace transform](../../../../../laplace-transform.md) of the frailty density,

$$
\overline S(t)=\int_0^\infty e^{-uH_0(t)}g(u)\,du.
$$

If $m=\mathbb EU<\infty$, replacing $U$ by $U/m$ and $h_0$ by $m h_0$ leaves their product, and hence the model, unchanged. The normalization $\mathbb EU=1$ identifies this otherwise arbitrary scale and makes $h_0(0)$ the initial population hazard when $H_0(0)=0$.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 207](../../paper-207-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
