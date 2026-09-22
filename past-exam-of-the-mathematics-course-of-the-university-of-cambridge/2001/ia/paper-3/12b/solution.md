<h1 id="12b/solution">Solution</h1>

↑ **Parent:** [12B](../12b.md)

Let $\phi_1,\phi_2$ be two sufficiently regular solutions with the same source and boundary data, and set $w=\phi_1-\phi_2$. Then $\nabla^2w=0$ and $\alpha\partial_nw+w=0$. [Green's first identity](../../../../../green-s-first-identity.md) gives

$$
\int_V|\nabla w|^2\,dV
=\int_{\partial V}w\,\partial_nw\,dS
=-\int_{\partial V}\alpha(\partial_nw)^2\,dS\le0.
$$

The left side is nonnegative, so it vanishes. Thus $w$ is constant on each connected component. Its [normal derivative](../../../../../normal-derivative.md) is zero, and the [boundary condition](../../../../../boundary-condition.md) then forces that constant to be zero. This proves **at most one solution**. The [Poisson uniqueness with a nonnegative Robin normal coefficient](../../../../../poisson-uniqueness-with-a-nonnegative-robin-normal-coefficient.md) proof never divides by $\alpha$, so it includes the points or boundary portions where $\alpha=0$.

For the exponential-sine modes, direct differentiation gives

$$
\partial_x^2(e^{\pm\ell x}\sin\ell y)=\ell^2e^{\pm\ell x}\sin\ell y,
\qquad
\partial_y^2(e^{\pm\ell x}\sin\ell y)=-\ell^2e^{\pm\ell x}\sin\ell y.
$$

Their sum is zero, so both modes are [harmonic functions](../../../../../harmonic-function.md) for every real $\ell$.

For the square, the horizontal Dirichlet data suggest [separation of variables](../../../../../separation-of-variables.md) in the form $\phi(x,y)=F(x)\sin(ky)$, where the positive integer $k$ makes the sine vanish at both horizontal edges. The [Laplace equation](../../../../../laplace-equation.md) gives $F''-k^2F=0$, hence $F=A\cosh(kx)+B\sinh(kx)$. At $x=0$, the outward normal points in the negative $x$ direction. The [Robin boundary condition](../../../../../robin-boundary-condition.md) is therefore $F(0)-F'(0)=0$, or $A=kB$. The right edge requires $F(\pi)=1$, fixing the remaining coefficient. The resulting [separated Laplace mode with a Robin edge](../../../../../separated-laplace-mode-with-a-robin-edge.md) is

$$
\boxed{\phi(x,y)=\frac{k\cosh(kx)+\sinh(kx)}{k\cosh(k\pi)+\sinh(k\pi)}\sin(ky).}
$$

The denominator is positive for $k>0$. The function satisfies the [Laplace equation](../../../../../laplace-equation.md) and all four [boundary conditions](../../../../../boundary-condition.md) directly; for example its left-edge value and $x$ derivative agree, giving the correct outward-normal Robin sign. It extends regularly to the corners.

On the left edge the uniqueness coefficient is $\alpha=1$; on the other three edges it is $\alpha=0$ with the prescribed Dirichlet value. The same [Green's first identity](../../../../../green-s-first-identity.md) argument applies to the square's piecewise smooth boundary, whose corners have zero boundary measure. Thus **this is the unique regular solution**, or equivalently the unique finite-energy solution with these boundary traces. Unbounded corner singularities are outside that boundary-value class.

## ↑ Ancestors (10)

1. [12B](../12b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
