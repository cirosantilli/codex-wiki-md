<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [force flux at infinity in Stokes flow](../../../../force-flux-at-infinity-in-stokes-flow.md). With an outward normal from a large sphere, the [force](../../../../force-split.md) on the body is $\mathbf F=\int_{S_R}\sigma\mathbf n\,dS$. Let $C=3a/4$. The leading far-field [velocity](../../../../velocity.md) and [pressure](../../../../pressure-split.md) are

$$
u_i=C\left(\frac{U_i}{r}+\frac{(\mathbf U\cdot\mathbf x)x_i}{r^3}\right)+O(r^{-3}),\qquad
p=2\mu C\frac{\mathbf U\cdot\mathbf x}{r^3}.
$$

Their [rate-of-strain tensor](../../../../strain-rate-tensor.md) is

$$
e_{ij}=C(\mathbf U\cdot\mathbf x)\left(\frac{\delta_{ij}}{r^3}-\frac{3x_ix_j}{r^5}\right)+O(r^{-4}).
$$

In the [Newtonian fluid stress tensor](../../../../newtonian-fluid-stress-tensor.md) $\sigma_{ij}=-p\delta_{ij}+2\mu e_{ij}$, the isotropic pieces cancel. Consequently,

$$
\sigma\mathbf n=-\frac{6\mu C}{R^2}(\mathbf U\cdot\mathbf n)\mathbf n+O(R^{-4}).
$$

The [second spherical moment integral](../../../../second-spherical-moment-integral.md) $\int n_in_j\,d\Omega=(4\pi/3)\delta_{ij}$ follows from rotational symmetry and $\sum_i n_i^2=1$. Since $dS=R^2d\Omega$, taking $R\to\infty$ gives the [Stokes drag law](../../../../stokes-s-law.md):

$$
\boxed{\mathbf F=-6\mu C\frac{4\pi}{3}\mathbf U=-6\pi\mu a\mathbf U.}
$$

The omitted dipole contributes a surface integral of order $R^{-2}$ and vanishes in this limit. The sign refers to the fluid's drag on the moving sphere.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the advanced fluid dynamics course of the University of Oxford](../../../split.md)
5. [Advanced fluid dynamics course of the University of Oxford](../../../../advanced-fluid-dynamics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
