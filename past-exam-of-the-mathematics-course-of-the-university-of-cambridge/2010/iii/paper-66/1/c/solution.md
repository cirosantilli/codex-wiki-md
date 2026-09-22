<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write the first-order surface [velocity](../../../../../../velocity.md) as $\mathbf u_1=\mathbf U_1+\boldsymbol\Omega_1\times\mathbf x+\mathbf g$, where the previous derivative gives

$$
\mathbf g=\frac{3f}{2a}(\mathbf I-\mathbf n\mathbf n)\mathbf U_0.
$$

As a test field, choose a sphere translating with arbitrary [velocity](../../../../../../velocity.md) $\widehat{\mathbf V}$. Its surface [velocity](../../../../../../velocity.md) is $\widehat{\mathbf V}$ and its [traction](../../../../../../traction.md) is $\widehat{\boldsymbol\sigma}\mathbf n=-3\mu\widehat{\mathbf V}/(2a)$. The [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) gives

$$
\int_{r=a}\mathbf u_1\cdot\widehat{\boldsymbol\sigma}\mathbf n\,dS
=\int_{r=a}\widehat{\mathbf V}\cdot\boldsymbol\sigma_1\mathbf n\,dS=0.
$$

Terms at infinity vanish because both [velocities](../../../../../../velocity.md) decay. Since $\int\mathbf n\,dS=0$, the rotation term has zero surface average. The arbitrary test [velocity](../../../../../../velocity.md) therefore gives the [first-order mobility of a nearly spherical particle](../../../../../../first-order-mobility-of-a-nearly-spherical-particle.md):

$$
\boxed{\mathbf U_1=-\frac1{4\pi a^2}\int_{r=a}\mathbf g\,dS
=\frac{3}{8\pi a^3}\int_{r=a}f(\mathbf n)(\mathbf n\mathbf n-\mathbf I)\mathbf U_0\,dS.}
$$

For the ellipsoidal perturbation, the second spherical moment gives $\int f\,dS=(4\pi a^3/3)\operatorname{tr}\mathbf D=0$. The supplied fourth moment gives, componentwise,

$$
\int f n_i n_j\,dS
=\frac{4\pi a^3}{15}\left(\delta_{ij}\operatorname{tr}\mathbf D+D_{ij}+D_{ji}\right)
=\frac{8\pi a^3}{15}D_{ij}.
$$

Substitution yields

$$
\boxed{\mathbf U_1=\frac15\mathbf D\mathbf U_0=\frac15\mathbf U_0\cdot\mathbf D,}
$$

where the last notation uses symmetry of the [tensor](../../../../../../tensor.md).

One can also use a rotating-sphere test with surface [traction](../../../../../../traction.md) $-3\mu\widehat{\boldsymbol\Omega}\times\mathbf n$. Its reciprocal integral, together with zero first-order [torque](../../../../../../torque.md), gives

$$
\boldsymbol\Omega_1=-\frac{3}{8\pi a^3}\int_{r=a}\mathbf n\times\mathbf g\,dS
=-\frac{9}{16\pi a^4}\int_{r=a}f(\mathbf n)\mathbf n\times\mathbf U_0\,dS.
$$

Here $f(-\mathbf n)=f(\mathbf n)$, so the last integrand is odd and its integral vanishes. Thus **$\boldsymbol\Omega_1=0$**. Inversion symmetry forbids a translation-to-rotation coupling for this centred ellipsoidal perturbation.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
