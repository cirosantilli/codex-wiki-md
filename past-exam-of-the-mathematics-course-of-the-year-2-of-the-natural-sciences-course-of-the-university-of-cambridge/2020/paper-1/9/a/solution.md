<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Label the equilibrium vertices in the order $+x,-x,+y,-y,+z,-z$, and write their [displacements](../../../../../displacement.md) as $\mathbf u_i(t)\in\mathbb R^3$. Their eighteen Cartesian components are [generalized coordinates](../../../../../generalized-coordinate.md). Linearize the axial Hookean [springs](../../../../../spring.md) about the unstressed equilibrium. For an edge with unit direction $\mathbf n_{ij}$, its first-order extension is $\mathbf n_{ij}\cdot(\mathbf u_i-\mathbf u_j)$, so the quadratic [potential energy](../../../../../potential-energy.md) is

$$
V=\frac k2\sum_{\langle ij\rangle}[\mathbf n_{ij}\cdot(\mathbf u_i-\mathbf u_j)]^2.
$$

Three [zero modes](../../../../../zero-mode.md) are [translations](../../../../../translation-geometry.md): for each Cartesian [unit vector](../../../../../unit-vector.md) $\mathbf e_\alpha$, take $\mathbf u_i=\mathbf e_\alpha$ at every vertex. Three more are infinitesimal [rotations](../../../../../rotation-mathematics.md) $\mathbf u_i=\mathbf e_\alpha\times\mathbf r_i$. Explicitly, in the stated vertex order, their [displacement](../../../../../displacement.md) [vectors](../../../../../vector.md) are

$$
R_x:\quad (\mathbf0,\mathbf0,\mathbf e_z,-\mathbf e_z,-\mathbf e_y,\mathbf e_y),
$$



$$
R_y:\quad (-\mathbf e_z,\mathbf e_z,\mathbf0,\mathbf0,\mathbf e_x,-\mathbf e_x),
$$



$$
R_z:\quad (\mathbf e_y,-\mathbf e_y,-\mathbf e_x,\mathbf e_x,\mathbf0,\mathbf0).
$$

[Translations](../../../../../translation-geometry.md) leave each [displacement](../../../../../displacement.md) difference zero. For [rotations](../../../../../rotation-mathematics.md),

$$
\mathbf n_{ij}\cdot[\boldsymbol\Omega\times(\mathbf r_i-\mathbf r_j)]=0
$$

because the equilibrium edge [vector](../../../../../vector.md) is parallel to $\mathbf n_{ij}$. Hence every [spring](../../../../../spring.md) has zero first-order extension in all six patterns, and the [stiffness matrix](../../../../../stiffness-matrix.md) annihilates them.

The [translations](../../../../../translation-geometry.md) have nonzero summed [displacement](../../../../../displacement.md), while all the [rotations](../../../../../rotation-mathematics.md) have zero sum. The three rotational patterns are themselves independent because the vertices do not lie on a single line. Thus

$$
\boxed{\text{there are at least six independent zero modes: three translations and three rotations}.}
$$

These are the [rigid-motion zero modes of a spring framework](../../../../../rigid-motion-zero-modes-of-a-spring-framework.md). The rotational [displacements](../../../../../displacement.md) describe infinitesimal rigid [rotations](../../../../../rotation-mathematics.md); an arbitrary finite [rotation](../../../../../rotation-mathematics.md) would require its nonlinear [displacement](../../../../../displacement.md) field.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [9](../../9.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
