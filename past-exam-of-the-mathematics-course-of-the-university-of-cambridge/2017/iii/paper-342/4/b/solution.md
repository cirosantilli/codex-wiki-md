<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $n$ point from the sphere into the exterior fluid, so the surface position relative to the centre is $r=an$. The physical surface velocity is

$$
u|_S=\Omega\times an+u'.
$$

Free rotation means the actual body is [torque-free](../../../../../../torque-free.md): the total [hydrodynamic torque](../../../../../../hydrodynamic-torque.md) $T=\int_San\times(\sigma\cdot n)dS$ vanishes. Use the auxiliary [rotating sphere in Stokes flow](../../../../../../rotating-sphere-in-stokes-flow.md) with arbitrary $\widehat\Omega$, boundary velocity $\widehat u=\widehat\Omega\times an$ and the given [traction](../../../../../../traction.md) $\widehat\sigma\cdot n=-3\mu\widehat\Omega\times n$. The auxiliary flow is the decaying exterior rotation of a sphere, not a rigid rotation of the entire infinite fluid.

The left-hand cross-work in the [Lorentz reciprocal theorem for Stokes flow](../../../../../../lorentz-reciprocal-theorem-for-stokes-flow.md) is

$$
\int_S\widehat u\cdot\sigma\cdot n\,dS
=\widehat\Omega\cdot T=0.
$$

The other cross-work becomes

$$
0=-3\mu\int_S(\Omega\times an+u')\cdot(\widehat\Omega\times n)dS.
$$

The spherical integral identities are

$$
\int_S n_i n_j\,dS=\frac{4\pi a^2}{3}\delta_{ij},\qquad
\int_SdS=4\pi a^2.
$$

Using $(\Omega\times n)\cdot(\widehat\Omega\times n)=\Omega\cdot\widehat\Omega-(\Omega\cdot n)(\widehat\Omega\cdot n)$, the rotational contribution is $-8\pi\mu a^3\Omega\cdot\widehat\Omega$. The slip contribution is $-3\mu\widehat\Omega\cdot\int_S n\times u'\,dS$. Since $\widehat\Omega$ is arbitrary, the [torque-free rotation of a spherical squirmer](../../../../../../torque-free-rotation-of-a-spherical-squirmer.md) satisfies

$$
\boxed{\Omega=-\frac{3}{8\pi a^3}\int_S n\times u'\,dS.}
$$

The viscosity cancels, as expected for a kinematically prescribed slip in a linear viscous problem. If the freely moving sphere also has a translation $U$, its added cross-work is zero because the auxiliary rotating sphere has zero total force, $\int_S\widehat\sigma\cdot n\,dS=0$. Thus translation does not alter this rotational formula. Without the torque-free assumption an external-torque contribution would have to be retained.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
