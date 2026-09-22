<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a nonnegative continuous event time $T$, the [survivor function](../../../../../../survival-function.md) is $F(t)=\mathbb P(T>t)$, and its [probability density function](../../../../../../probability-density-function.md) is

$$
\boxed{f(t)=-F'(t).}
$$

The [hazard function](../../../../../../hazard-function.md) is the instantaneous event rate conditional on being event-free at that time:

$$
\boxed{h(t)=\lim_{\epsilon\downarrow0}\frac{\mathbb P(t\le T<t+\epsilon\mid T\ge t)}{\epsilon}=\frac{f(t)}{F(t)}\quad(F(t)>0).}
$$

If the event is certain to occur in finite time, the density is proper: $\int_0^\infty f(t)\,dt=1$, so $F(t)\to0$. Since $F(0)=1$ and $F'=-hF$, the [cumulative hazard function](../../../../../../cumulative-hazard-function.md) is $H(t)=-\log F(t)$. Therefore **a certain eventual event requires unbounded integrated hazard**:

$$
\boxed{\lim_{t\to\infty}\int_0^t h(u)\,du=+\infty.}
$$

If the lifetime has a finite upper endpoint, the same divergence occurs as that endpoint is approached, and $H$ is interpreted as infinite beyond it.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
