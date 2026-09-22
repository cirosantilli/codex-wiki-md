<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $g=f\mu$. At every prime, $f(p)^2=1$, so the [triangle inequality for pretentious distance](../../../../../../triangle-inequality-for-pretentious-distance.md) gives

$$
\mathbb D(f,n^{it};x)+\mathbb D(g,n^{iu};x)
\geq\mathbb D(\mu,n^{i(t+u)};x).
$$

The standard [strong aperiodicity of the Möbius function](../../../../../../strong-aperiodicity-of-the-mobius-function.md) states, for example with $T=(\log x)^{1/10}$, that

$$
\inf_{|v|\leq2T}\mathbb D(\mu,n^{iv};x)^2\longrightarrow\infty.
$$

Indeed, its left side is controlled by the prime sum $\sum_{p\leq x}(1+\cos(v\log p))/p$, uniformly in this range.

Choose $t$ and $u$ minimizing the two distances in [Halász theorem](../../../../../../halasz-theorem.md). The displayed triangle inequality implies that at least one of $M(f;x,T)$ and $M(g;x,T)$ tends to infinity. Halász's bound, and $T\to\infty$, then show that at least one of

$$
\frac1x\left|\sum_{n\leq x}f(n)\right|,
\qquad
\frac1x\left|\sum_{n\leq x}f(n)\mu(n)\right|
$$

tends to zero. Their minimum is consequently $o(1)$, which is the claimed $o(x)$ estimate before normalization.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [2](../../2.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
