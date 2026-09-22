<h1 id="10a/solution">Solution</h1>

↑ **Parent:** [10A](../10a.md)

[Stokes theorem](../../../../../stokes-theorem.md) equates the circulation around the induced [boundary orientation](../../../../../boundary-orientation.md) of an [oriented surface](../../../../../oriented-surface.md) to the normal flux of [curl](../../../../../curl.md):

$$
\boxed{\oint_{\partial S}\mathbf F\cdot d\mathbf x=\int_S(\nabla\times\mathbf F)\cdot d\mathbf S.}
$$

The usual version requires a piecewise smooth oriented surface and a [vector field](../../../../../vector-field.md) continuously differentiable on a neighbourhood of it. We use the upward orientation wherever the surface is a graph; each outer circle is counterclockwise viewed from above, and an inner circle is clockwise.

Write $\rho=(x^2+y^2)^{1/2}$. The [surface of revolution](../../../../../surface-of-revolution.md) has $z=\sqrt{\rho^2+1-\lambda}$ with $0\le z\le1$. For $0<\lambda<1$, it is a disk-shaped cap of a [two-sheeted hyperboloid](../../../../../two-sheeted-hyperboloid.md), running from $\rho=0,z=\sqrt{1-\lambda}$ to $\rho=\sqrt\lambda,z=1$. For $\lambda=1$, it is a [right circular cone](../../../../../right-circular-cone.md), $z=\rho$, including its apex. For $\lambda>1$, it is an annular strip of a [one-sheet hyperboloid](../../../../../one-sheet-hyperboloid.md), between the circles $\rho=\sqrt{\lambda-1},z=0$ and $\rho=\sqrt\lambda,z=1$.

<a id="10a/image-disk-cap-cone-and-annular-hyperboloid-strip-in-the-three-positive-parameter-regimes-of-stokes-theorem"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3-stokes-surfaces.png)

**[Figure 2](#10a/image-disk-cap-cone-and-annular-hyperboloid-strip-in-the-three-positive-parameter-regimes-of-stokes-theorem). Disk cap, cone and annular hyperboloid strip in the three positive-parameter regimes of Stokes' theorem**.

For $z>0$, differentiation of the graph gives $z_x=x/z$ and $z_y=y/z$, so the upward [vector surface element of a graph](../../../../../vector-surface-element-of-a-graph.md) and its scalar area are

$$
\boxed{d\mathbf S=\left(-\frac xz,-\frac yz,1\right)dx\,dy,\qquad
 dS=\sqrt{1+\frac{x^2+y^2}{z^2}}\,dx\,dy.}
$$

For $\lambda>1$ this graph expression is singular at the lower circle because the surface has a vertical tangent there, rather than a singular geometric surface. A regular parametrization is

$$
\mathbf X(z,\phi)=(\sqrt{z^2+\lambda-1}\cos\phi,\sqrt{z^2+\lambda-1}\sin\phi,z),\qquad
\mathbf X_z\times\mathbf X_\phi=-\rho\mathbf e_\rho+z\mathbf e_z.
$$

It proves that the graph [surface integral](../../../../../surface-integral.md) is interpreted by its integrable endpoint limit. The same parametrization works away from the pole or apex in the other regimes.

Direct differentiation of the first [vector field](../../../../../vector-field.md) gives

$$
\boxed{\nabla\times\mathbf F=(0,0,2).}
$$

Its [surface integral](../../../../../surface-integral.md) is twice the projected area, namely $2\pi\lambda$ for $0<\lambda\le1$ and $2\pi[\lambda-(\lambda-1)]=2\pi$ for $\lambda>1$. On an oriented circle of radius $R$, $\mathbf F\cdot d\mathbf x=R^2d\phi$. The outer circulation is $2\pi\lambda$; an inner circle, when present, contributes $-2\pi(\lambda-1)$. Thus

$$
\boxed{\oint_{\partial S}\mathbf F\cdot d\mathbf x=\int_S(\nabla\times\mathbf F)\cdot d\mathbf S=2\pi\min(\lambda,1).}
$$

At $\lambda=1$, excise a small apex circle of radius $\varepsilon$, apply [Stokes theorem](../../../../../stokes-theorem.md) to the smooth truncated cone, and let $\varepsilon\to0$. The removed flux and its inner circulation are both $2\pi\varepsilon^2$, so the limiting equality holds. This avoids silently applying a smooth-surface theorem at the cone's nonsmooth apex.

The second [vector field](../../../../../vector-field.md) is the [azimuthal inverse-radius vector field](../../../../../azimuthal-inverse-radius-vector-field.md), $\mathbf G=\mathbf e_\phi/\rho$. Away from the axis,

$$
\partial_x\left(\frac x{x^2+y^2}\right)=\frac{y^2-x^2}{(x^2+y^2)^2}
=\partial_y\left(\frac{-y}{x^2+y^2}\right),\qquad
\boxed{\nabla\times\mathbf G=\mathbf0\quad(\rho>0).}
$$

The other two [curl](../../../../../curl.md) components vanish because the field is independent of $z$ and has zero $z$ component. On any positively oriented circle around the axis, $\mathbf G\cdot d\mathbf x=d\phi$, so its circulation is $2\pi$, independent of radius. Therefore

$$
\boxed{\oint_{\partial S}\mathbf G\cdot d\mathbf x=
\begin{cases}2\pi,&0<\lambda\le1,\\0,&\lambda>1.\end{cases}}
$$

For $\lambda>1$ the surface avoids the axis, so [Stokes theorem](../../../../../stokes-theorem.md) applies directly and returns zero [curl](../../../../../curl.md) flux. For $0<\lambda<1$ the disk cap meets the axis, and for $\lambda=1$ the apex lies on it: $\mathbf G$ is undefined there, so the neighbourhood hypothesis of [Stokes theorem](../../../../../stokes-theorem.md) fails. Removing a small circle gives cancelling inner and outer circulations; the inner circulation remains $-2\pi$ as its radius tends to zero. Hence it cannot be discarded as it could for $\mathbf F$. A nonzero circulation here is compatible with zero [curl](../../../../../curl.md) away from the excluded axis.

## ↑ Ancestors (10)

1. [10A](../10a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
