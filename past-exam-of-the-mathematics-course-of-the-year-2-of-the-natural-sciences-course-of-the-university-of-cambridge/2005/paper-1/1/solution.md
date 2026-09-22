<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $r>0$, the [chain rule](../../../../chain-rule.md) gives $\partial r/\partial x_i=x_i/r$. Differentiating the radial factor gives $d\phi/dr=e^{ikr}(ikr-1)/(4\pi r^2)$, so in [Cartesian coordinates](../../../../cartesian-coordinate-system.md)

$$
\boxed{\nabla\phi=\frac{e^{ikr}(ikr-1)}{4\pi r^3}(x,y,z).}
$$

The origin is excluded because the scalar field is singular there.

The [Stokes theorem](../../../../stokes-theorem.md) states $\int_S(\nabla\times\mathbf F)\cdot\mathbf n\,dS=\oint_{\partial S}\mathbf F\cdot d\boldsymbol\ell$ for a sufficiently smooth vector field and oriented surface with piecewise smooth boundary. The boundary orientation follows the right-hand rule relative to $\mathbf n$.

For the [convective acceleration identity](../../../../convective-acceleration-identity.md), use the [Levi-Civita symbol](../../../../levi-civita-symbol.md) contraction $\epsilon_{ijk}\epsilon_{k\ell m}=\delta_{i\ell}\delta_{jm}-\delta_{im}\delta_{j\ell}$. It gives

$$
[\mathbf F\times(\nabla\times\mathbf F)]_i=\epsilon_{ijk}F_j\epsilon_{k\ell m}\partial_\ell F_m=F_j\partial_iF_j-F_j\partial_jF_i=\frac12\partial_i(F_jF_j)-[(\mathbf F\cdot\nabla)\mathbf F]_i.
$$

Rearranging proves the required vector identity.

For [orthogonal coordinates](../../../../orthogonal-coordinates.md), define the [scale factors of orthogonal coordinates](../../../../scale-factors-of-orthogonal-coordinates.md) $h_i=|\partial\mathbf r/\partial q_i|$ and tangent [unit vectors](../../../../unit-vector.md) $\mathbf e_i=h_i^{-1}\partial\mathbf r/\partial q_i$. They form an [orthonormal basis](../../../../orthonormal-basis.md), and $d\mathbf r=\sum_i h_i\mathbf e_i\,dq_i$. Equating $d\psi=\sum_i\partial_{q_i}\psi\,dq_i$ with $\nabla\psi\cdot d\mathbf r$ identifies each component. Thus the [gradient in orthogonal coordinates](../../../../gradient-in-orthogonal-coordinates.md) is

$$
\boxed{\nabla\psi=\sum_{i=1}^3\frac1{h_i}\frac{\partial\psi}{\partial q_i}\mathbf e_i.}
$$

This holds on a regular coordinate chart where all scale factors are positive.

## ↑ Ancestors (12)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2005](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
