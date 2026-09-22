<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

A [phase diagram](../../../../../phase-diagram.md) partitions a space of thermodynamic controls into regions with distinct equilibrium phases. Its boundaries indicate [phase coexistence](../../../../../phase-coexistence.md) or [continuous phase transitions](../../../../../continuous-phase-transition.md); a [critical point](../../../../../critical-point.md) is a termination of coexistence where the distinction between phases disappears. A concrete three-dimensional control space is $(T,\Delta,h)$ for the [Blume–Capel model](../../../../../blume-capel-model.md): a spin can be $0$ or $\pm1$, the exchange favors aligned nonzero spins, and $\Delta$ controls the energetic cost of nonzero spins. Varying $\Delta$ changes the balance between a continuous ordering transition and a [first-order phase transition](../../../../../first-order-phase-transition.md). Their meeting is a [tricritical point](../../../../../tricritical-point.md).

Locally, the same structure is displayed by the [Landau free energy](../../../../../landau-free-energy.md)

$$
f(M)=\frac r2M^2+\frac u4M^4+\frac v6M^6-hM,\qquad v>0,
$$

with three controls $(r,u,h)$. For $u>0$, the line $r=h=0$ consists of ordinary [critical points](../../../../../critical-point.md). For $u<0$, equal free energies of $M=0$ and a nonzero stationary point require

$$
r+uM^2+vM^4=0,\qquad \frac r2M^2+\frac u4M^4+\frac v6M^6=0.
$$

Eliminating $r$ gives the [tricritical three-phase line](../../../../../tricritical-three-phase-line.md)

$$
\boxed{M^2=-\frac{3u}{4v},\qquad r=\frac{3u^2}{16v},\qquad h=0.}
$$

Here $M=0$ and both signs of $M$ coexist, with a discontinuous [order parameter](../../../../../order-parameter.md). Below this line, or below $r=0$ when $u>0$, the plane $h=0$ is an ordered [phase coexistence](../../../../../phase-coexistence.md) sheet: crossing it reverses the sign of $M$. Two [tricritical wings](../../../../../tricritical-wing.md) also extend to nonzero $h$, separating weakly and strongly magnetized states of the same sign. Their ordinary [critical points](../../../../../critical-point.md) satisfy $f'=f''=f'''=0$. Since $f'''=6uM+20vM^3$, their [tricritical wing critical edges](../../../../../tricritical-wing-critical-edge.md) are

$$
M_c^2=-\frac{3u}{10v},\qquad r_c=\frac{9u^2}{20v},\qquad h_c=\frac{6u^2}{25v}M_c.
$$

At these edges $f''''=-12u>0$, giving an ordinary quartic critical expansion around $M_c$. All these structures end at **the tricritical point $r=u=h=0$**. The diagrams show both the zero-field section and the genuinely three-dimensional coexistence structure.

<a id="1/image-scalar-landau-phase-diagram-zero-field-transitions-tricritical-wings-and-ordinary-critical-edges"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-51-landau-phase-diagram.png)

**[Figure 1](#1/image-scalar-landau-phase-diagram-zero-field-transitions-tricritical-wings-and-ordinary-critical-edges). Scalar Landau phase diagram: zero-field transitions, tricritical wings and ordinary critical edges**.

For the final [critical exponent](../../../../../critical-exponent.md) calculation, take $r=at$ with $a>0$, $t=(T-T_c)/T_c$, and hold the other controls fixed. At an ordinary [critical point](../../../../../critical-point.md), the quartic term dominates the sextic term. For $h=0$ and $r<0$,

$$
M^2=-r/u,\qquad f_{\rm eq,s}=-r^2/(4u),
$$

whereas on the disordered side the singular contribution is zero. Two temperature derivatives give a finite jump in [heat capacity](../../../../../heat-capacity.md), so $\alpha=0$. At $r=0$, the [equation of state](../../../../../equation-of-state.md) is $h=uM^3+O(M^5)$, so $\delta=3$.

Along the tricritical trajectory $u=0$, the nonzero minimum obeys $M^4=-r/v$ and

$$
f_{\rm eq,s}=\frac r2\sqrt{-r/v}+\frac v6(-r/v)^{3/2}
=-\frac{(-r)^{3/2}}{3\sqrt v}.
$$

Thus two temperature derivatives produce $|t|^{-1/2}$. At $r=u=0$, $h=vM^5$. Therefore the [mean-field critical exponents](../../../../../mean-field-critical-exponent.md) are

$$
\boxed{(\alpha,\delta)_{\rm ordinary}=(0,3),\qquad(\alpha,\delta)_{\rm tricritical}=(1/2,5).}
$$

With $A$ the thermodynamic [free energy](../../../../../thermodynamic-free-energy.md), the physical sign is $C=-T\partial_T^2 A$, rather than the positive sign printed in the paper. This correction affects the sign of the [heat capacity](../../../../../heat-capacity.md), not its [critical exponent](../../../../../critical-exponent.md). The tricritical result assumes that the independent quartic control is tuned to zero; a generic trajectory through nearby ordinary critical points need not have these exponents.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 51](../../paper-51-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
