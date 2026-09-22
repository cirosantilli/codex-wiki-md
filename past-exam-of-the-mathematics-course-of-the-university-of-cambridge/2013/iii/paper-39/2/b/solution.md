<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A_\delta=\sup_{K\ge0}K^\delta C(K)<\infty$. The [call-price decay and moment threshold](../../../../../../call-price-decay-and-moment-threshold.md) follows by splitting the preceding [integral](../../../../../../integral.md) at one. Since $(S-K)_+\le S$, for $0<\varepsilon<\delta$,

$$
\int_0^1 K^{\varepsilon-1}C(K)\,dK\le\frac{\mathbb ES}{\varepsilon}.
$$

For $K\ge1$, the decay bound gives

$$
\int_1^\infty K^{\varepsilon-1}C(K)\,dK
\le A_\delta\int_1^\infty K^{\varepsilon-1-\delta}\,dK
=\frac{A_\delta}{\delta-\varepsilon}.
$$

The [power payoff static call representation](../../../../../../power-payoff-static-call-representation.md) therefore yields

$$
\boxed{M(1+\varepsilon)\le(1+\varepsilon)\mathbb ES
+\frac{\varepsilon(1+\varepsilon)A_\delta}{\delta-\varepsilon}<\infty.}
$$

The $\varepsilon=0$ case is the given finite first moment. The strict endpoint matters: a [Pareto distribution](../../../../../../pareto-distribution.md) with $\mathbb P(S>x)=x^{-(1+\delta)}$ for $x\ge1$ has $C(K)=K^{-\delta}/\delta$ for $K\ge1$, but its moment of order $1+\delta$ is infinite. Thus the stated decay condition does not generally imply the endpoint moment.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 39](../../../paper-39-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
