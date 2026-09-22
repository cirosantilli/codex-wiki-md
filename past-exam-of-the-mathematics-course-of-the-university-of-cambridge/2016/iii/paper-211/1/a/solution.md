<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [natural filtration](../../../../../../natural-filtration.md) of $S$ is the [natural Brownian filtration](../../../../../../natural-brownian-filtration.md): since $\sigma>0$, the equation $W_t=(\log(S_t/S_0)-\mu t)/\sigma$ recovers the entire [Brownian motion](../../../../../../brownian-motion-split.md) history from the [stock](../../../../../../stock.md) history. For $s<t$, [independent increments](../../../../../../independent-increments.md) and the [moment-generating function of a normal distribution](../../../../../../moment-generating-function-of-a-normal-distribution.md) give

$$
\mathbb E[S_t\mid\mathcal F_s^S]
=S_s\mathbb E e^{\mu(t-s)+\sigma(W_t-W_s)}
=S_s e^{(\mu+\sigma^2/2)(t-s)}.
$$

All these [expectations](../../../../../../expected-value.md) are finite. Since $S_s>0$, the [martingale](../../../../../../martingale-split.md) identity holds for every $s<t$ exactly when the last exponential equals one. **The required logarithmic drift is**

$$
\boxed{\mu=-\frac{\sigma^2}{2}.}
$$

This is the distinction between the [drift](../../../../../../drift-coefficient.md) of $\log S$ and the [drift](../../../../../../drift-coefficient.md) of $S$: here the latter is zero.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
