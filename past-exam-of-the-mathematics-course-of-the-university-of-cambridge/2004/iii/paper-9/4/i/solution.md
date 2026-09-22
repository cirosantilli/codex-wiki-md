<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a [harmonic function](../../../../../../harmonic-function.md) $u$, put $g=u_x-iu_y$. Its [Wirtinger derivative](../../../../../../wirtinger-derivatives.md) is

$$
\frac{\partial g}{\partial\overline z}
=\frac12\bigl(u_{xx}+u_{yy}+i(u_{xy}-u_{yx})\bigr)=0,
$$

so the [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) make $g$ holomorphic. In the [simply connected domain](../../../../../../simply-connected-domain.md) it has a single-valued primitive

$$
F(z)=\int_{z_0}^{z}g(\zeta)\,d\zeta.
$$

The integral is [path independent](../../../../../../path-independence.md): local [holomorphic primitives](../../../../../../holomorphic-primitive.md) make its value invariant under [path](../../../../../../continuous-path.md) [homotopies](../../../../../../homotopy.md), and being [simply connected](../../../../../../simply-connected-space.md) makes any two [paths](../../../../../../continuous-path.md) with the given endpoints [homotopic](../../../../../../homotopy.md), as in Question 3.

Since $F'=g$, the [real part](../../../../../../real-part.md) satisfies $(\operatorname{Re}F)_x=u_x$ and $(\operatorname{Re}F)_y=\operatorname{Re}(ig)=u_y$. Hence $\operatorname{Re}F-u$ is constant on the [connected](../../../../../../connected-space.md) domain. Adding a real constant corrects it, producing **a single-valued holomorphic $f$ with $\operatorname{Re}f=u$**. The [imaginary part](../../../../../../imaginary-part.md) is a [harmonic conjugate](../../../../../../harmonic-conjugate.md) and is unique up to an additive real constant. This is the [global harmonic conjugate criterion by vanishing periods](../../../../../../global-harmonic-conjugate-criterion-by-vanishing-periods.md) in the [simply connected](../../../../../../simply-connected-space.md) case.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
