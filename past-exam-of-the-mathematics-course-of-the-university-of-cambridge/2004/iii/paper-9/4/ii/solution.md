<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Take **$u(z)=\log|z|$**. In [polar coordinates](../../../../../../polar-coordinates.md) its [Laplacian](../../../../../../laplacian.md) is $u_{rr}+r^{-1}u_r=-r^{-2}+r^{-2}=0$, so it is [harmonic](../../../../../../harmonic-function.md) on the [annulus](../../../../../../annulus-mathematics.md). If $u=\operatorname{Re}f$ for a single-valued [holomorphic function](../../../../../../holomorphic-function.md), the [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) would give $f'=u_x-iu_y=1/z$. But for $1<\rho<2$,

$$
\oint_{|z|=\rho}f'(z)\,dz=0,\qquad
\oint_{|z|=\rho}\frac{dz}{z}=2\pi i.
$$

The first equality follows by evaluating the primitive $f$ around a closed curve. This contradiction verifies the absence of a global [harmonic conjugate](../../../../../../harmonic-conjugate.md).

For the final function, the quotient of squared distances is $|z+1|^2/|z-1|^2$. On $|z|>1$, both $1+1/z$ and $1-1/z$ lie in the open right half-plane, so their [principal logarithms](../../../../../../principal-complex-logarithm.md) are single-valued and holomorphic. Define

$$
\boxed{f(z)=2\operatorname{Log}(1+1/z)-2\operatorname{Log}(1-1/z)
=4\sum_{m=0}^{\infty}\frac{z^{-(2m+1)}}{2m+1}.}
$$

The series converges locally uniformly outside the unit [circle](../../../../../../circle.md), and

$$
\operatorname{Re}f(z)=2\log|z+1|-2\log|z-1|
=\log\frac{(x+1)^2+y^2}{(x-1)^2+y^2}.
$$

Thus this is the required single-valued [holomorphic function](../../../../../../holomorphic-function.md), even on the larger domain $|z|>1$. Its [derivative](../../../../../../derivative.md) is $2/(z+1)-2/(z-1)$, whose two periods around the holes cancel. The [logarithmic cancellation on an exterior annulus](../../../../../../logarithmic-cancellation-on-an-exterior-annulus.md) explains why this example succeeds while $\log|z|$ fails; using independent multivalued logarithms of $z+1$ and $z-1$ would conceal that cancellation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 9](../../../paper-9-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
