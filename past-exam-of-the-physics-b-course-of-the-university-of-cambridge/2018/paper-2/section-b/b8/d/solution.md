<h1 id="section-b/b8/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For a slender [elastic beam](../../../../../../elastic-beam.md) undergoing small bending, assume plane cross-sections remain plane and normal to the [neutral axis](../../../../../../neutral-axis.md). Fibres a signed distance $z$ from that axis have longitudinal [strain](../../../../../../strain.md) $\varepsilon_{xx}=-z/R$, where $R$ is the local [radius of curvature](../../../../../../radius-of-curvature.md). [Hooke's law](../../../../../../hooke-s-law.md) gives [stress](../../../../../../stress.md) $\sigma_{xx}=-Ez/R$, where $E$ is [Young's modulus](../../../../../../young-s-modulus.md). Zero resultant axial [force](../../../../../../force-split.md) places the [neutral axis](../../../../../../neutral-axis.md) through the section's [centroid](../../../../../../centroid.md) for a homogeneous beam.

The [bending moment](../../../../../../bending-moment.md) is the moment of this [stress](../../../../../../stress.md) distribution. Its magnitude is

$$
\boxed{M=\frac{EI_A}{R},\qquad I_A=\int_{\rm section}z^2\,dA.}
$$

The [second moment of area](../../../../../../second-moment-of-area.md) $I_A$ has units $\mathrm{m^4}$, and the [bending stiffness](../../../../../../bending-stiffness.md) $EI_A$ has units $\mathrm{N\,m^2}$. A rectangular section of width $b$ and depth $h$ has $I_A=bh^3/12$, so placing more material far from the [neutral axis](../../../../../../neutral-axis.md) strongly resists bending. This is the purpose of an I-section.

For small deflection $y(x)$, the signed [curvature](../../../../../../curvature.md) is approximately $y''$. A consistent variational sign convention follows from the [elastic energy](../../../../../../elastic-energy.md) and a transverse load $q(x)$:

$$
\Pi[y]=\frac12\int EI_A(y'')^2\,dx-\int qy\,dx,
\qquad \boxed{(EI_Ay'')''=q.}
$$

For constant [bending stiffness](../../../../../../bending-stiffness.md) this is the [Euler-Bernoulli beam equation](../../../../../../euler-bernoulli-beam-equation.md) $EI_Ay''''=q$. A clamped end fixes $y=y'=0$; a simply supported end has $y=0$ and zero [bending moment](../../../../../../bending-moment.md); an unloaded free end has zero moment and shear, $y''=y'''=0$ for uniform $EI_A$. Endpoint loads replace the corresponding zero-force [boundary conditions](../../../../../../boundary-condition.md).

For a cantilever of length $L$ carrying a tip [force](../../../../../../force-split.md) $F$, choose positive deflection along $F$. The internal bending gives $EI_Ay''=F(L-x)$, with $y(0)=y'(0)=0$. Two integrations give

$$
y(x)=\frac{Fx^2(3L-x)}{6EI_A},
\qquad \boxed{y(L)=\frac{FL^3}{3EI_A}.}
$$

This approximation requires small slopes, elastic strains and a length large compared with section dimensions. Shear deformation, rotary inertia, plastic yielding and large [rotations](../../../../../../rotation-mathematics.md) require extensions. Adding inertia gives [flexural waves](../../../../../../flexural-wave.md) with $\omega^2=(EI_A/\rho_m A_s)k^4$ for a uniform beam, where $\rho_m A_s$ is [mass](../../../../../../mass.md) per unit length.

## ↑ Ancestors (15)

1. [D](../d.md)
2. [B8](../../b8.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the physics B course of the University of Cambridge](../../../../../split.md)
7. [Physics B course of the University of Cambridge](../../../../../../physics-b-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../../split.md)
