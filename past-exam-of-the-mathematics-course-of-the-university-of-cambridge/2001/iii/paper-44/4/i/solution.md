<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Far downslope let the typical height be $H(X)$ and the cross-slope half-width be $W(X)$. Slenderness gives $W\ll X$ and slowly varying longitudinal thickness. In a steady [porous gravity current](../../../../../../porous-gravity-current.md), the longitudinal spreading term is smaller than [advection](../../../../../../advection.md) by the ratio $H/X$, while longitudinal [diffusion](../../../../../../diffusion.md) relative to transverse [diffusion](../../../../../../diffusion.md) is of order $(W/X)^2$. Thus the leading balance is

$$
\partial_Xh^\beta=\partial_Y(h^\beta h_Y).
$$

Integrating across the finite current, with zero flux through its dry side edges, makes the leading downslope [volume flux](../../../../../../volumetric-flow-rate.md) constant:

$$
\int h^\beta\,dY=\text{constant},\qquad H^\beta W\sim\text{constant}.
$$

Balancing the two differential terms gives

$$
\frac{H^\beta}{X}\sim\frac{H^{\beta+1}}{W^2},\qquad W^2\sim HX.
$$

Eliminate $H\propto W^{-1/\beta}$ to find the [far-downslope width of a constant-flux porous current](../../../../../../far-downslope-width-of-a-constant-flux-porous-current.md):

$$
\boxed{Y_N(X)\propto X^\gamma,\qquad
\gamma=\frac{\beta}{2\beta+1}.}
$$

The typical height is correspondingly $H\propto X^{-1/(2\beta+1)}$. For every $\beta>0$, the width exponent is less than one half, so $W/X\to0$ and $H/X\to0$, consistent with the discarded longitudinal terms. The [porosity](../../../../../../porosity.md) exponent $\alpha$ drops out because it enters storage, which has zero time derivative in this steady problem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
