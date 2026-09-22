<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $t\ge0$ and $\theta>0$, the [exponential distribution](../../../../../../exponential-distribution.md) has [probability density function](../../../../../../probability-density-function.md) $f(t)=\theta e^{-\theta t}$. Integrating the [probability density function](../../../../../../probability-density-function.md) gives the [survivor function](../../../../../../survival-function.md) $S(t)=P(T>t)=e^{-\theta t}$. The [hazard function](../../../../../../hazard-function.md) divides instantaneous failure density by the [probability](../../../../../../probability.md) of having survived, and the [integrated hazard](../../../../../../cumulative-hazard-function.md) accumulates this rate. Thus

$$
\boxed{f(t)=\theta e^{-\theta t},\quad S(t)=e^{-\theta t},\quad h(t)=f(t)/S(t)=\theta,\quad H(t)=\int_0^t h(u)\,du=\theta t=-\log S(t).}
$$

The [probability density function](../../../../../../probability-density-function.md) is zero for $t<0$, and the [survivor function](../../../../../../survival-function.md) is one there.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 40](../../../paper-40-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
