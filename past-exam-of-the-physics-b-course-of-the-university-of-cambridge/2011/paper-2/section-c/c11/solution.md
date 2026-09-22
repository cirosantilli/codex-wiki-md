<h1 id="section-c/c11/solution">Solution</h1>

↑ **Parent:** [C11](../c11.md)

Let $s$ denote distance from the [neutral axis](../../../../../neutral-axis.md) within a cross section. Bending to radius $R$ gives longitudinal [strain](../../../../../strain.md) $s/R$, so [Hooke's law](../../../../../hooke-s-law.md) gives [stress](../../../../../stress.md) $Es/R$. Its moment is

$$
\boxed{B=\int_A s\frac{Es}{R}\,dA=\frac{EI}{R},\qquad I=\int_A s^2dA.}
$$

Here $E$ is [Young's modulus](../../../../../young-s-modulus.md) and $I$ is the _[second moment of area](../../../../../second-moment-of-area.md)_, not a mass [moment of inertia](../../../../../moment-of-inertia.md). For the stated square orientation, $I=a^4/12$.

For [self-weight deflection of a square cantilever](../../../../../self-weight-deflection-of-a-square-cantilever.md), the downward load per unit length is $q=\rho a^2g$. A free-end segment from $x$ to $l$ has shear-force magnitude $F(x)=q(l-x)$ and bending-moment magnitude $B(x)=q(l-x)^2/2$. Thus, with the given sign conventions,

$$
-F'(x)=q=B''(x).
$$

Using the small-slope [curvature](../../../../../curvature.md) $1/R\simeq y''$ for downward deflection,

$$
\boxed{y''''=\beta,\qquad\beta=\frac q{EI}=\frac{12\rho g}{Ea^2}.}
$$

The clamp fixes position and slope, and the unloaded free end has zero moment and shear:

$$
y(0)=y'(0)=0,\qquad y''(l)=y'''(l)=0.
$$

Four integrations yield

$$
y(x)=\frac\beta{24}x^2(x^2-4lx+6l^2),\qquad
\boxed{y(l)=\frac{\beta l^4}{8}=\frac{3\rho g l^4}{2Ea^2}\quad\text{downwards}.}
$$

The linear beam model requires small slopes and [strains](../../../../../strain.md); the strong $l^4$ dependence eventually invalidates that approximation if other dimensions and material properties are fixed.

## ↑ Ancestors (14)

1. [C11](../c11.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2011](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
