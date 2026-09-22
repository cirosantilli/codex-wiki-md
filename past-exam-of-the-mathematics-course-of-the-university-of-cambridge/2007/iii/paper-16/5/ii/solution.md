<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For an $n$-dimensional [singular simplex](../../../../../../singular-simplex.md) $\sigma$ and a degree-$p$ [singular cochain](../../../../../../singular-cochain.md) $\alpha$, use the front-face/back-face convention

$$
\sigma\frown\alpha=\alpha(\sigma|[v_0,\ldots,v_p])\,\sigma|[v_p,\ldots,v_n],
$$

and set it to zero for $p>n$. Extend linearly over $R$. Passing to [homology](../../../../../../homology-split.md) classes of cycles and [cohomology](../../../../../../cohomology-split.md) classes of cocycles defines the [cap product](../../../../../../cap-product.md) $H_n(X;R)\times H^p(X;R)\to H_{n-p}(X;R)$.

For a continuous map $f$, the [cochain pullback](../../../../../../cochain-pullback.md) satisfies $(f^*\alpha)(\tau)=\alpha(f\circ\tau)$, and the induced chain map sends $\sigma$ to $f\circ\sigma$. Since composition commutes with restrictions to faces,

$$
\begin{aligned}
f_*(\sigma\frown f^*\alpha)
&=\alpha(f\circ\sigma|[v_0,\ldots,v_p])\,(f\circ\sigma|[v_p,\ldots,v_n])\\
&=(f\circ\sigma)\frown\alpha.
\end{aligned}
$$

The identity holds on chains, so it descends directly to classes and proves the [naturality of the cap product](../../../../../../naturality-of-the-cap-product.md): $f_*(x\frown f^*\alpha)=f_*(x)\frown\alpha$. No additional well-definedness verification is required here.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
