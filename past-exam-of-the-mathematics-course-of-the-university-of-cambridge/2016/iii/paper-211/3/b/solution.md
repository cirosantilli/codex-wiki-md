<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For fixed $\gamma$, [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) is justified by bounded $P$ and $X$. At the unconstrained [minimizer](../../../../../../global-minimizer.md) $H_\gamma$, the first-order condition is

$$
p\,e^{\gamma(H_\gamma\cdot p-x)}
=\mathbb E\!\left[P e^{\gamma(X-H_\gamma\cdot P)}\right].
$$

Define the strictly positive, bounded [pricing kernel](../../../../../../state-price-density.md)

$$
Z_\gamma=\frac{e^{\gamma(X-H_\gamma\cdot P)}}{e^{\gamma(H_\gamma\cdot p-x)}}.
$$

The first-order condition says $\mathbb E[Z_\gamma P]=p$, so $Z_\gamma\in\mathcal Z$. When taking the requested [partial derivative](../../../../../../partial-derivative.md), hold $H$ fixed and only afterwards set $H=H_\gamma$. Writing $A_\gamma=H_\gamma\cdot p-x$, we obtain

$$
\begin{aligned}
\left.\partial_\gamma F_\gamma(H)\right|_{H=H_\gamma}
&=e^{\gamma A_\gamma}\left[A_\gamma+
\mathbb E\{Z_\gamma(X-H_\gamma\cdot P)\}\right]\\
&=e^{\gamma A_\gamma}\big[\mathbb E(Z_\gamma X)-x\big].
\end{aligned}
$$

The assumed dual bound applies to this particular [pricing kernel](../../../../../../state-price-density.md). **Thus**

$$
\boxed{\left.\partial_\gamma F_\gamma(H)\right|_{H=H_\gamma}\leq0.}
$$

No derivative of the map $\gamma\mapsto H_\gamma$ is needed; confusing a [partial derivative](../../../../../../partial-derivative.md) with a derivative along the minimizing path would add an unnecessary hypothesis.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
