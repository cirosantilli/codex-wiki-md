<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $H:X\to Y$ be a [homeomorphism](../../../../../../homeomorphism.md) with $H\circ f=g\circ H$. This is [topological conjugacy](../../../../../../topological-conjugacy.md). Choose a [compatible metric](../../../../../../compatible-metric.md) $e$ on $Y$ and pull it back to $X$:

$$
d_H(x,x')=e(Hx,Hx').
$$

Because $H$ is a [homeomorphism](../../../../../../homeomorphism.md), $d_H$ is a [compatible metric](../../../../../../compatible-metric.md). The conjugacy identity implies $Hf^k=g^kH$ for every $k\geq0$, so the corresponding [Bowen metrics](../../../../../../bowen-metric.md) satisfy

$$
(d_H)_n(x,x')=\max_{0\leq k<n}e(g^kHx,g^kHx')=e_n(Hx,Hx').
$$

The [bijection](../../../../../../bijection.md) $H$ therefore transports [separated sets](../../../../../../separated-subset-of-a-metric-space.md) in either direction without changing their separation, and $s_n(d_H,\epsilon)=s_n(e,\epsilon)$. Their exponential growth rates, and then their limits as $\epsilon\downarrow0$, agree. Part (a) lets us replace $d_H$ by any [compatible metric](../../../../../../compatible-metric.md) on $X$. Hence

$$
\boxed{h_{\mathrm{top}}(f)=h_{\mathrm{top}}(g).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
