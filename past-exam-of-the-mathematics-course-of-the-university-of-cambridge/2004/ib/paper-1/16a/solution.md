<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

Let $F(z)=p(z)/q(z)$. Its only possible finite [poles](../../../../../pole.md) are the distinct nonreal roots $\alpha_j$, and the [residue](../../../../../residue.md) of $F(z)e^{iz}$ there is $p(\alpha_j)e^{i\alpha_j}/q'(\alpha_j)$; this is zero if the numerator cancels that [pole](../../../../../pole.md). Close the real segment by a positively oriented semicircle in the upper half-plane, where $|e^{iz}|=e^{-\operatorname{Im}z}$ decays.

For sufficiently large radius $R$, all roots lie strictly inside or outside the contour as appropriate, and the degree bound gives $|F(z)|\leq C/R$ uniformly on the arc. Parametrizing by $z=Re^{i\theta}$ bounds the arc integral by

$$
C\int_0^\pi e^{-R\sin\theta}\,d\theta
\leq2C\int_0^{\pi/2}e^{-2R\theta/\pi}\,d\theta\leq\frac{C\pi}{R}\longrightarrow0.
$$

Here $\sin\theta\geq2\theta/\pi$ on $[0,\pi/2]$, and symmetry handles the other half. The [residue theorem](../../../../../residue-theorem.md) therefore gives

$$
\boxed{\int_{-\infty}^{\infty}\frac{p(x)}{q(x)}e^{ix}\,dx
=2\pi i\sum_{\operatorname{Im}\alpha_j>0}\frac{p(\alpha_j)e^{i\alpha_j}}{q'(\alpha_j)}.}
$$

To justify that this is the ordinary improper integral rather than just its symmetric principal value, note $F(x)=O(|x|^{-1})$ and $F'(x)=O(|x|^{-2})$. On either tail, [integration by parts](../../../../../integration-by-parts.md) writes the integral as a vanishing endpoint term $F(x)e^{ix}/i$ minus an absolutely convergent integral involving $F'$. Thus both one-sided limits exist. When the degree bound is stricter the original integral is already absolutely convergent. This proves the [Fourier integral of a rational function with simple nonreal poles](../../../../../fourier-integral-of-a-rational-function-with-simple-nonreal-poles.md) formula with all tail and arc limits accounted for.

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
