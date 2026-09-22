<h1 id="15e/solution">Solution</h1>

↑ **Parent:** [15E](../15e.md)

Fixed endpoint variations yield the Euler–Lagrange equation

$$
F_r-\frac d{dz}F_{r'}=0.
$$

When $F$ is independent of $z$, differentiation gives

$$
\frac d{dz}(F-r'F_{r'})=r'\left(F_r-\frac d{dz}F_{r'}\right)=0.
$$

This is the [Beltrami identity](../../../../../beltrami-identity.md). Denote the constant by $1/k$ when nonzero; for a general Lagrangian a zero constant is also possible.

The film area is $S=2\pi\int_{-H}^Hr\sqrt{1+r'^2}\,dz$. Suppressing its harmless positive factor $2\pi$, take $F=r\sqrt{1+r'^2}$. The Euler–Lagrange equation reduces to

$$
\boxed{rr''=1+r'^2,\qquad r(-H)=r(H)=R.}
$$

The [first integral](../../../../../first-integral.md) is $r/\sqrt{1+r'^2}=1/k$ with $k>0$. Hence $1+r'^2=k^2r^2$ and, using the [differential equation](../../../../../differential-equation-split.md) without dividing by $r'$, $r''=k^2r$. The positive solution obeying that [first integral](../../../../../first-integral.md) is $r=k^{-1}\cosh(k(z-z_0))$. Equal endpoint radii force $z_0=0$, giving

$$
\boxed{r(z)=k^{-1}\cosh(kz),\qquad R=k^{-1}\cosh(kH).}
$$

Thus every smooth positive stationary film in this axisymmetric class is a [catenoid](../../../../../catenoid.md).

Put $u=kH>0$. The boundary equation is $R/H=f(u)=\cosh u/u$. The [function](../../../../../function-split.md) tends to infinity at both endpoints of $(0,\infty)$, and

$$
f'(u)=\frac{u\sinh u-\cosh u}{u^2}.
$$

Its minimum occurs when $u=\coth u$. The [function](../../../../../function-split.md) $u-\coth u$ is strictly increasing, with [derivative](../../../../../derivative.md) $1+\operatorname{csch}^2u>0$, and has limits $-\infty$ and $+\infty$. It therefore has exactly one positive zero $A$. At this point $1/A=\tanh A$, so $f(A)=\sinh A$. This proves the [catenoid existence threshold for equal rings](../../../../../catenoid-existence-threshold-for-equal-rings.md):

$$
\boxed{R/H<\sinh A\Longrightarrow\text{no smooth connected catenoid solution}.}
$$

At equality there is one stationary solution and above it two. The equation describes candidates for an area minimum, not a guarantee that both branches minimize. The thinner-neck branch is unstable to suitable axisymmetric variations; topology-changing collapse can also compete with [connected](../../../../../connected-space.md) films. In particular two separate planar disks have area $2\pi R^2$. The derived threshold concerns existence of the smooth annular stationary film; it does not exclude such disconnected competitors.

## ↑ Ancestors (10)

1. [15E](../15e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
