<h1 id="16d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [method of images](../../../../../../method-of-images.md) replaces the earthed plane by an image charge $-q$ at $(-a,0,0)$. The two Coulomb potentials cancel at $x=0$, so uniqueness for the [Dirichlet problem](../../../../../../dirichlet-problem.md) makes the resulting field the physical field in $x>0$. With $\mathbf r=(x,y,z)$ and $\mathbf e_x=(1,0,0)$,

$$
\boxed{\Phi(\mathbf r)=\frac{q}{4\pi\epsilon_0}
\left(\frac1{|\mathbf r-a\mathbf e_x|}
-\frac1{|\mathbf r+a\mathbf e_x|}\right)}
$$

and

$$
\boxed{\mathbf E(\mathbf r)=\frac{q}{4\pi\epsilon_0}
\left(
\frac{\mathbf r-a\mathbf e_x}{|\mathbf r-a\mathbf e_x|^3}
-\frac{\mathbf r+a\mathbf e_x}{|\mathbf r+a\mathbf e_x|^3}
\right)}.
$$

The [electric multipole expansion](../../../../../../electric-multipole-expansion.md) from part (a) gives, for $r\gg a$,

$$
\Phi(\mathbf r)
=\frac{q}{4\pi\epsilon_0}\frac{2ax}{r^3}+O(r^{-4})
=\frac{\mathbf p\mathbin{\cdot}\mathbf r}{4\pi\epsilon_0r^3}+O(r^{-4}),
\qquad
\boxed{\mathbf p=2qa\,\mathbf e_x}.
$$

Thus the leading field is that of an [electric dipole](../../../../../../electric-dipole.md).

On the plane,

$$
E_x(0,y,z)
=-\frac{2qa}{4\pi\epsilon_0(a^2+y^2+z^2)^{3/2}}.
$$

Taking the plane normal to be $+\mathbf e_x$ and using [polar coordinates](../../../../../../polar-coordinates.md),

$$
\int_{\mathbb R^2}E_x\,dy\,dz
=-\frac{qa}{\epsilon_0}\int_0^\infty
\frac{\rho\,d\rho}{(a^2+\rho^2)^{3/2}}
=\boxed{-\frac q{\epsilon_0}}.
$$

With the outward normal of the region $x>0$, the sign is reversed. This is consistent with [Gauss's law](../../../../../../gauss-s-law.md): all electric flux from the real charge terminates on the grounded conductor.

The [electrostatic boundary condition](../../../../../../electrostatic-boundary-conditions-at-a-conductor.md) gives the induced [surface charge density](../../../../../../surface-charge-density.md)

$$
\boxed{\sigma(y,z)=\epsilon_0E_x(0,y,z)
=-\frac{qa}{2\pi(a^2+y^2+z^2)^{3/2}}},
$$

and its integral is

$$
\boxed{Q_{\rm induced}=-q}.
$$

In the plane $z=0$, the field lines leave the positive charge, meet the conductor normally, and are the right-half-plane portions of the field lines joining the real charge to its negative image.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [16D](../../16d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
