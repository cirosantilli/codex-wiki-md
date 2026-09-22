<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Solving the [geometric Brownian motion](../../../../../../geometric-brownian-motion.md) equation over $[t,T]$ gives

$$
S_T=S_t\exp\left(\sigma_0(W_T-W_t)-\frac12\sigma_0^2(T-t)\right).
$$

The [Brownian increment](../../../../../../brownian-increment.md) is independent of $\mathcal F_t$ and has a [normal distribution](../../../../../../normal-distribution.md) with variance $T-t$. Its exponential [moment-generating function](../../../../../../moment-generating-function.md) therefore gives

$$
C(t,T)=\sqrt{S_t}\,e^{-\sigma_0^2(T-t)/4}
\mathbb E\left[e^{\sigma_0(W_T-W_t)/2}\mid\mathcal F_t\right]
=\sqrt{S_t}\,e^{-\sigma_0^2(T-t)/8}.
$$

The required deterministic price function is

$$
\boxed{F(t,T,s,v)=\sqrt{s}\exp\left(-\frac18v^2(T-t)\right).}
$$

This includes $s=0$, $v=0$ and $t=T$. For $s>0$ and $t<T$, it is continuous and strictly decreasing in $v\geq0$, with range $(0,\sqrt{s}]$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
