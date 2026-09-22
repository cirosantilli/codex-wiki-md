<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $L$ be the streamwise evolution scale, $\delta$ the jet width, and $U_c$ its velocity scale. A slender jet has $\varepsilon=\delta/L\ll1$; mean [incompressibility](../../../../../../incompressible-flow.md) gives $V=O(\varepsilon U_c)$. Both mean advection terms are then $O(U_c^2/L)$. For turbulent parcels crossing a transverse distance $l$, retention of their original streamwise momentum gives a fluctuation $\hat u\sim-lU_y$; a comparable transverse fluctuating speed gives the down-gradient [mixing length](../../../../../../mixing-length.md) closure

$$
\overline{\hat u\hat v}=-l^2|U_y|U_y=-\nu_TU_y,
\qquad\nu_T=l^2|U_y|.
$$

The [mixing length](../../../../../../mixing-length.md) is an effective distance of momentum retention, with statistical coefficients absorbed into $l$; it is not the net transverse displacement of a mean streamline. This closure models the [Reynolds stress](../../../../../../reynolds-stress.md) rather than deriving it exactly.

In a slender equilibrium jet, the fluctuation magnitude inferred from momentum balance is $u'^2\sim U_c^2\delta/L=\varepsilon U_c^2$. The transverse [Reynolds stress](../../../../../../reynolds-stress.md) gradient then has size $u'^2/\delta\sim U_c^2/L$, whereas the streamwise normal-stress gradient is $u'^2/L\sim\varepsilon U_c^2/L$. At sufficiently high [Reynolds number](../../../../../../reynolds-number.md), molecular transverse diffusion is smaller provided

$$
\frac{\nu U_c/\delta^2}{U_c^2/L}=\frac1{\mathrm{Re}_L\varepsilon^2}\ll1,
\qquad\mathrm{Re}_L=\frac{U_cL}\nu.
$$

Streamwise molecular diffusion is smaller still by $\varepsilon^2$. A free jet has ambient mean pressure constant to leading order; transverse momentum corrections imply only a higher-order mean streamwise pressure force. Thus high speed must be accompanied by the slender-jet ordering, not used alone to discard every other term.

For a symmetric jet decreasing away from the centre, $U_y<0$ on $y>0$ and $U_y>0$ on $y<0$. Accordingly $\overline{\hat u\hat v}=\operatorname{sgn}(y)l^2(U_y)^2$ off the centreline, and the leading equation is

$$
\boxed{UU_x+VU_y=-\partial_y\overline{\hat u\hat v}
=-\operatorname{sgn}(y)\,\partial_y\{l^2(U_y)^2\}.}
$$

At the centreline the signed form requires the stress to tend continuously to zero; otherwise differentiation would add a distributional term. The undifferentiated [Reynolds stress](../../../../../../reynolds-stress.md) form is the appropriate global equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
