<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [divergence theorem](../../../../../../divergence-theorem.md) states $\int_V\nabla\cdot\mathbf F\,dV=\oint_{\partial V}\mathbf F\cdot\mathbf n\,dS$. With the [Poisson equation for Newtonian gravity](../../../../../../poisson-equation-for-newtonian-gravity.md), this gives

$$
\oint_{\partial V}\nabla\phi\cdot\mathbf n\,dS=4\pi GM(V),
$$

or gravitational-acceleration flux $\oint\mathbf g\cdot\mathbf n\,dS=-4\pi GM(V)$.

Use cylindrical radius $R=r\sin\theta$, so $r(1+|\cos\theta|)=r+|z|$. An arbitrary reference length in the logarithm only adds a constant potential. Off the equatorial plane, the radial part of $\nabla^2\log[r(1+|\cos\theta|)]$ is $1/r^2$. Writing $c=\cos\theta$, its angular part is $r^{-2}d[(1-c^2)d\log(1+|c|)/dc]/dc=-1/r^2$ on either open hemisphere. The two cancel: there is no volume density away from $z=0$.

At the plane, $\partial_z\phi|_{0^+}=v_0^2/R$ and $\partial_z\phi|_{0^-}=-v_0^2/R$. Applying the gravitational flux law to a thin pillbox gives $4\pi G\Sigma=\partial_z\phi|_{0^+}-\partial_z\phi|_{0^-}$. Consequently

$$
\boxed{\Sigma(R)=\frac{v_0^2}{2\pi GR},\qquad
\rho(R,z)=\frac{v_0^2}{2\pi GR}\delta(z).}
$$

This is the [Mestel disk potential-density pair](../../../../../../mestel-disk-potential-density-pair.md). There is no additional point mass at the origin: the enclosed mass tends to zero linearly as the enclosing radius shrinks.

At $z=0$, $\phi=v_0^2\log R$ up to a constant, so radial circular balance gives

$$
\boxed{v_{\mathrm{circ}}^2=R\,\partial_R\phi=v_0^2.}
$$

On a sphere of radius $r$, $\partial_r\phi=v_0^2/r$ at every nonsingular angular point. Its flux is $4\pi v_0^2r$, and hence

$$
\boxed{M(<r)=\frac{v_0^2r}{G}.}
$$

Direct integration of the [surface density](../../../../../../surface-density-of-a-disk.md) confirms $2\pi\int_0^r\Sigma(R)R\,dR=v_0^2r/G$. Thus $v_{\mathrm{circ}}^2=GM(<r)/r$ even though the source is a [razor-thin disk](../../../../../../razor-thin-disk-approximation.md). This equality is a special scale-free property of the [Mestel disk](../../../../../../mestel-disk.md), not evidence that the source is spherical. In a general disk, matter outside the orbit and nonspherical interior forces prevent this enclosed-mass formula for the local [circular speed](../../../../../../circular-speed.md). The model has infinite total mass, so its potential is defined by differences rather than a zero at infinity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
