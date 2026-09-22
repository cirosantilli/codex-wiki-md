<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume a sharp interface, uniformly mixed warm upper air with fixed [reduced gravity](../../../../../../reduced-gravity-split.md) $g'=g\Delta\rho/\rho_0$, cool ambient air entering below, no wind, no wall heat exchange, negligible source volume, and quasi-steady [Boussinesq](../../../../../../boussinesq-approximation.md) flow through the small vents. Neglect the interior approach [velocity](../../../../../../velocity.md). The hydrostatic buoyancy head between the two vents is $\rho_0g'h$.

Both openings carry the same [volume flux](../../../../../../volumetric-flow-rate.md) $q_v$. The [discharge coefficient](../../../../../../discharge-coefficient.md) law gives a pressure loss $\rho_0q_v^2/(2C_d^2A^2)$ at each opening. Adding the two losses gives $q_v=C_dA\sqrt{g'h}$, not the single-opening value with an extra factor $\sqrt2$. Cool replacement air displaces the warm layer, so $S\dot h=-q_v$. With $h(0)=H$, integrate to obtain

$$
\boxed{h(t)=\left(\sqrt H-\frac{C_dA\sqrt{g'}}{2S}t\right)^2,\quad
0\leq t\leq t_e=\frac{2S\sqrt H}{C_dA\sqrt{g'}}.}
$$

The ideal model sets $h=0$ thereafter. The formula applies only while the parenthesis is nonnegative; squaring a negative value would invent renewed filling. A finite aperture or a diffuse final interface invalidates the idealization near exhaustion.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
