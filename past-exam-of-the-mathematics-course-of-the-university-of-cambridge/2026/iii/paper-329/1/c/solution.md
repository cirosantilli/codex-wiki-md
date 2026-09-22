<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) to $\mathbf u_1$ and the test flow around a sphere rotating with arbitrary $\widehat{\boldsymbol\Omega}$. On $r=a$,

$$
\widehat{\mathbf u}=\widehat{\boldsymbol\Omega}\times\mathbf x,
\qquad
\widehat{\boldsymbol\sigma}\mathbf n=-3\mu\widehat{\boldsymbol\Omega}\times\mathbf n.
$$

The reciprocal integral containing $\widehat{\mathbf u}\cdot\boldsymbol\sigma_1\mathbf n$ vanishes by the first-order torque condition. Since $\partial_r\mathbf u_0=-2\boldsymbol\Omega_0\times\mathbf n$, the first-order boundary velocity is

$$
\mathbf u_1=\mathbf U_1+a\boldsymbol\Omega_1\times\mathbf n+3f\boldsymbol\Omega_0\times\mathbf n.
$$

The translational term integrates to zero. Therefore, for every $\widehat{\boldsymbol\Omega}$,

$$
\int_{r=a}\left(a\boldsymbol\Omega_1\times\mathbf n+3f\boldsymbol\Omega_0\times\mathbf n\right)
\cdot(\widehat{\boldsymbol\Omega}\times\mathbf n)\,dS=0.
$$

Now

$$
\int_{r=a}(\mathbf A\times\mathbf n)\cdot(\mathbf B\times\mathbf n)\,dS
=\frac{8\pi a^2}{3}\mathbf A\cdot\mathbf B.
$$

For $f=a(\mathbf n\cdot\mathbf D\mathbf n)$, tracelessness of $mathbf D$ and the stated fourth-moment identity give

$$
\int_{r=a}f(\boldsymbol\Omega_0\times\mathbf n)
\cdot(\widehat{\boldsymbol\Omega}\times\mathbf n)\,dS
=-\frac{8\pi a^3}{15}\widehat{\boldsymbol\Omega}\cdot\mathbf D\boldsymbol\Omega_0.
$$

It follows that

$$
\boxed{\boldsymbol\Omega_1=\frac35\mathbf D\boldsymbol\Omega_0},
\qquad \alpha=\frac35.
$$

A centered ellipsoid has inversion symmetry. An applied axial couple is unchanged under inversion, whereas a translational velocity is reversed, so uniqueness of [Stokes flow](../../../../../../stokes-flow-split.md) forces

$$
\boxed{\mathbf U_1=0}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
