<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $D_1,D_2,D_3,D_4$ denote the open quadrants, counterclockwise from the first. Write $\theta=kx+2k^2t$. The [Lax pair](../../../../../../lax-pair.md) has the [Volterra integral equation](../../../../../../volterra-integral-equation.md) kernel $e^{-i[k(x-x')+2k^2(t-t')]\widehat\sigma_3}$, obtained by integrating its closed matrix differential form from a normalization point.

In column one, the off-diagonal factor is $e^{2i[k(x-x')+2k^2(t-t')]}$, whose modulus is $e^{-2\operatorname{Im}[k(x-x')+2k^2(t-t')]}$. Column two has the reciprocal factor. For $\mu_2$, choose the path $(0,0)\to(0,t)\to(x,t)$, so both differences are nonnegative. Column one requires $\operatorname{Im}k\geq0$ and $\operatorname{Im}k^2\geq0$, giving $D_1$; column two requires the opposite inequalities, giving $D_4$.

For $\mu_1$, the time path starts at $T$ and runs backward, while the spatial path runs rightward. Its column-one conditions are $\operatorname{Im}k\geq0$, $\operatorname{Im}k^2\leq0$, giving $D_2$; column two is bounded in $D_3$.

Finally, $\mu_3$ integrates spatially from infinity to $x$, where $x-x'\leq0$. Column one is bounded in the lower half-plane and column two in the upper half-plane. Normalization at $(\infty,T)$ is equivalent to normalization at $(\infty,t)$ because the decaying potential vanishes on the vertical path at infinity. Thus

$$
\boxed{\mu_1:(D_2,D_3),\qquad\mu_2:(D_1,D_4),\qquad\mu_3:(\mathbb C_-,\mathbb C_+).}
$$

The [Volterra integral equation](../../../../../../volterra-integral-equation.md) Neumann series converges locally uniformly under the usual integrable smooth scattering assumptions, proving holomorphic dependence in the open domains and continuous boundary values. These are the [Volterra analyticity sectors for a half-line NLS Lax pair](../../../../../../volterra-analyticity-sectors-for-a-half-line-nls-lax-pair.md); at $x=0$, absence of a spatial segment allows the larger time-only domains used for $A,B$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
