<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a single species both panels of the figure in [c](../c.md) contribute, now with $j=1$. They are the $s$-channel annihilation and $t$-channel scalar exchange, where the [Mandelstam variables](../../../../mandelstam-variables.md) are $s=(p_1+p_2)^2$, $t=(p_1-p_3)^2$, $u=(p_1-p_4)^2$ and $s+t+u=4m^2$. Fix the external-state order consistently with [c](../c.md). The exchange of identical external [fermionic operators](../../../../fermionic-operator.md) gives a relative minus sign:

$$
\boxed{\mathcal M=-g^2\left(\frac{(\bar v_2u_1)(\bar u_3v_4)}{s-M^2+i0}-\frac{(\bar u_3u_1)(\bar v_2v_4)}{t-M^2+i0}\right).}
$$

Changing the convention for ordering all external states can change the overall sign, but not this relative [fermionic sign](../../../../fermionic-sign.md).

The exchange $p_1\leftrightarrow-p_4$ must include [crossing symmetry](../../../../crossing-symmetry.md) the associated external [spinors](../../../../spinor.md), as well as continuing the [four-momenta](../../../../four-momentum.md). It interchanges $s$ and $t$, leaves $u$ fixed, and interchanges the two spinor pairings. Hence the analytically continued [invariant scattering amplitude](../../../../invariant-scattering-amplitude.md) is antisymmetric:

$$
\boxed{\mathcal M\longmapsto-\mathcal M,\qquad \overline{|\mathcal M|^2}(s,t)=\overline{|\mathcal M|^2}(t,s).}
$$

The first relation is understood with consistently chosen spinor crossing phases. It is not a substitution of negative-energy arguments into the original positive-energy $u$ spinors without changing external states.

Without repeating the [spin sum](../../../../spin-sum.md) calculation, [c](../c.md) fixes the square of the first diagram. [Crossing symmetry](../../../../crossing-symmetry.md) fixes the second by $s\leftrightarrow t$. Consequently the strongest immediate inference is

$$
\boxed{\overline{|\mathcal M|^2}=g^4\left[\frac{(s-4m^2)^2}{(s-M^2)^2}+\frac{(t-4m^2)^2}{(t-M^2)^2}+\frac{C(s,t)}{(s-M^2)(t-M^2)}\right],\quad C(s,t)=C(t,s).}
$$

The [interference](../../../../interference-wave-propagation.md) function is not determined by the separate diagram squares. In particular **adding the two squares and dropping [interference](../../../../interference-wave-propagation.md) is unjustified**. The [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) applied to the arrays of spin amplitudes also gives $|C(s,t)|\leq2|(s-4m^2)(t-4m^2)|$ on the physical scattering region.

For completeness, its value can be checked with one contracted [trace](../../../../matrix-trace.md), without another diagram calculation. The cross product is

$$
K=\frac14\operatorname{tr}[(\not p_2-m)(\not p_1+m)(\not p_3+m)(\not p_4-m)]
=-\frac12st-2m^2(s+t)+8m^4.
$$

The relative minus in the [invariant scattering amplitude](../../../../invariant-scattering-amplitude.md) gives $C=-2K$. Thus the fully evaluated result, beyond the symmetry inference alone, is

$$
\boxed{\overline{|\mathcal M|^2}=g^4\left[\frac{(s-4m^2)^2}{(s-M^2)^2}+\frac{(t-4m^2)^2}{(t-M^2)^2}+\frac{st+4m^2(s+t)-16m^4}{(s-M^2)(t-M^2)}\right].}
$$

Every term respects the inferred $s,t$ symmetry. In the massless limit the [interference](../../../../interference-wave-propagation.md) numerator reduces to $st$, which is nonzero at a generic scattering angle.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
