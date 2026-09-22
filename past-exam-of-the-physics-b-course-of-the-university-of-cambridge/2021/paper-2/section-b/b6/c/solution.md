<h1 id="section-b/b6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a slender [elastic beam](../../../../../../elastic-beam.md), the [Euler-Bernoulli beam equation](../../../../../../euler-bernoulli-beam-equation.md) assumes small [strain](../../../../../../strain.md), small deflection slopes and cross-sections that remain plane and normal to the deflected centreline. A fibre at signed distance $y$ from the [neutral axis](../../../../../../neutral-axis.md) has longitudinal [strain](../../../../../../strain.md) $\epsilon_{xx}=-y\kappa$, where $\kappa$ is the centreline [curvature](../../../../../../curvature.md). [Hooke's law](../../../../../../hooke-s-law.md) gives $\sigma_{xx}=-Ey\kappa$, with [Young's modulus](../../../../../../young-s-modulus.md) $E$.

Choose the internal bending-moment sign so that $M=-\int y\sigma_{xx}\,dA$. Then

$$
\boxed{M=EI_A\kappa,\qquad I_A=\int_Ay^2\,dA.}
$$

Here $I_A$ is the [second moment of area](../../../../../../second-moment-of-area.md), with units $\mathrm{m^4}$, not the mass [moment of inertia](../../../../../../moment-of-inertia.md) of a rotating body. For a uniform material under pure bending, zero axial resultant places the [neutral axis](../../../../../../neutral-axis.md) through the section's [centroid](../../../../../../centroid.md).

For small slopes, $\kappa\simeq w''(x)$. Combining the moment-curvature relation with transverse [force](../../../../../../force-split.md) and moment balance gives, with a consistent load sign convention,

$$
\boxed{\frac{d^2}{dx^2}\left(EI_A\frac{d^2w}{dx^2}\right)=q(x).}
$$

For constant stiffness this becomes $EI_Aw^{(4)}=q$. The [bending stiffness](../../../../../../bending-stiffness.md) $EI_A$ has units $\mathrm{N\,m^2}$. [Boundary conditions](../../../../../../boundary-condition.md) specify displacement and slope at a clamped end, or [bending moment](../../../../../../bending-moment.md) and shear [force](../../../../../../force-split.md) at a free end.

For a cantilever of length $\ell$ carrying a transverse end load $F$, take deflection positive towards the load. The moment magnitude is $M(x)=F(\ell-x)$, and integration with $w(0)=w'(0)=0$ gives

$$
w(x)=\frac{Fx^2(3\ell-x)}{6EI_A},\qquad
\boxed{w(\ell)=\frac{F\ell^3}{3EI_A}.}
$$

The free-end moment vanishes and the tip shear supplies the applied load. For a rectangular section of width $b$ and bending thickness $h$, $I_A=bh^3/12$, so increasing thickness strongly increases bending resistance. The model ceases to be reliable for large deflections, plastic [strains](../../../../../../strain.md) or short thick beams where shear deformation matters.

## ↑ Ancestors (15)

1. [C](../c.md)
2. [B6](../../b6.md)
3. [Section B](../../../section-b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2021](../../../../split.md)
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
