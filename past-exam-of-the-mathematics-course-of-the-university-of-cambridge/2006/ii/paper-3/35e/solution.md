<h1 id="35e/solution">Solution</h1>

↑ **Parent:** [35E](../35e.md)

Use metric signature $(+---)$ and write $u^a=\dot x^a$, $U=\sqrt{\eta_{ab}u^au^b}$. For an orientation-preserving affine change $s'=\alpha s+\beta$, with $\alpha>0$, $u'^a=u^a/\alpha$ and $ds'=\alpha ds$. Homogeneity of both terms of the [Lagrangian](../../../../../lagrangian.md) therefore leaves $L\,ds$ unchanged. Proper-time parametrization is used again when deriving the final equation.

Under $A_a\mapsto A_a+\partial_a\chi$, the action changes by $-q\int d\chi=-q[\chi(x_f)-\chi(x_i)]$. **The fixed-endpoint variational principle is gauge invariant; the action itself can change by a boundary term.** This is the precise version of the printed invariance claim. Negative $\alpha$ reverses orientation and requires a corresponding reorientation of the path, rather than the simple positive-parameter calculation above.

The [canonical momentum](../../../../../canonical-momentum.md) is

$$
\boxed{P_a=-m\frac{u_a}{U}-qA_a.}
$$

The [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) gives $-m\frac{d}{ds}(u_a/U)-q\partial_bA_a u^b=-q\partial_aA_bu^b$. Hence, with $F_{ab}=\partial_aA_b-\partial_bA_a$ and [proper time](../../../../../proper-time.md) $U=1$,

$$
\boxed{m\ddot x^a=qF^a{}_bu^b,\qquad F^a{}_b=\eta^{ac}F_{cb}.}
$$

Antisymmetry verifies the consistency condition directly: $\frac{d}{ds}(u_au^a)=2u_a\dot u^a=(2q/m)u^aF_{ab}u^b=0$.

For the uncharged [Lagrangian](../../../../../lagrangian.md) in the same sign convention, $p_a=-mu_a/U$, so $P_a=p_a-qA_a$. Equivalently $P_a+qA_a$ is the gauge-invariant kinetic covector in this convention. This illustrates [electromagnetic minimal coupling](../../../../../electromagnetic-minimal-coupling.md): replace the free canonical momentum by the gauge-covariant combination when introducing the field. The physical contravariant kinetic four-momentum is conventionally $mu^a$; its sign must not be confused with the covector obtained by differentiating the particular negative-length [Lagrangian](../../../../../lagrangian.md) used here.

## ↑ Ancestors (10)

1. [35E](../35e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
