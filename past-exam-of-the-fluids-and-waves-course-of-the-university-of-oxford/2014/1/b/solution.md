<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use instantaneous [polar coordinates](../../../../polar-coordinates.md) centered on the moving [circular cylinder](../../../../circular-cylinder.md), but measure the fluid [velocity](../../../../velocity.md) in the laboratory frame. Impermeability equates the normal components of body and fluid [velocity](../../../../velocity.md):

$$
(\mathbf u-U\mathbf e_x)\cdot\mathbf e_r=0\quad(r=a).
$$

Since $\mathbf e_x\cdot\mathbf e_r=\cos\theta$ and $u_r=\phi_r$, the [no-penetration boundary condition](../../../../no-penetration-boundary-condition.md) is

$$
\boxed{\phi_r(a,\theta)=U\cos\theta.}
$$

The [velocity potential](../../../../velocity-potential.md) obeys the exterior [Laplace equation](../../../../laplace-equation.md), by [incompressibility](../../../../incompressible-flow.md). The boundary data have only the first cosine harmonic. A decaying harmonic potential of this form is $\phi=C\cos\theta/r$. Matching its radial derivative gives $-C/a^2=U$, so $C=-Ua^2$. The zero [circulation](../../../../circulation-physics.md) condition rules out an angular potential term, and the integrated boundary condition gives zero net [volume flux](../../../../volumetric-flow-rate.md), ruling out a radial logarithmic source term. The remaining decaying harmonics have zero coefficients by the boundary data. Hence

$$
\boxed{\phi=-\frac{Ua^2}{r}\cos\theta.}
$$

Using the [streamfunction in polar coordinates](../../../../streamfunction-in-polar-coordinates.md), $u_r=r^{-1}\psi_\theta$, $u_\theta=-\psi_r$, gives

$$
\boxed{\psi=\frac{Ua^2}{r}\sin\theta,\qquad
u_r=\frac{Ua^2}{r^2}\cos\theta,\quad u_\theta=\frac{Ua^2}{r^2}\sin\theta.}
$$

One may also obtain both functions as the real and imaginary parts of $w(z)=-Ua^2/z$, a [two-dimensional potential doublet](../../../../two-dimensional-potential-doublet.md). The [velocity](../../../../velocity.md) decays as $r^{-2}$ and the source of this singular representation lies inside the excluded body. These are the fields used to calculate the [added mass of a circular cylinder](../../../../added-mass-of-a-circular-cylinder.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the fluids and waves course of the University of Oxford](../../../split.md)
5. [Fluids and waves course of the University of Oxford](../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
