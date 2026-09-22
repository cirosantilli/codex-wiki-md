<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

In a convenient cardinal parameter normalization, take the unit $m$-cube and project by the sum of its coordinates. Its pushforward density is the [unit-direction univariate box spline](../../../../../unit-direction-univariate-box-spline.md)

$$
B_m(x)=\int_{[0,1]^m}\delta\!\left(x-\sum_{r=1}^m u_r\right)du_1\cdots du_m.
$$

Equivalently, with $B_1=\mathbf1_{[0,1)}$ at its discontinuity points,

$$
\boxed{B_m=B_1*\cdots*B_1,\qquad B_m(x)=\int_0^1B_{m-1}(x-u)\,du.}
$$

Here there are $m$ [convolution](../../../../../convolution.md) factors; some conventions instead index the [spline](../../../../../spline-mathematics.md) by its degree $m-1$. The half-open convention for $m=1$ assigns knot values consistently and does not change the pushforward measure.

**Support and positivity.** A sum of $m$ numbers in $[0,1]$ lies in $[0,m]$, so the closed support is finite. For $0<x<m$, the interval of $u\in(0,1)$ with $0<x-u<m-1$ has positive length. Induction in the [convolution](../../../../../convolution.md) recurrence therefore gives $B_m(x)>0$ in the interior. For $m\geq2$, $B_m(0)=B_m(m)=0$: strict positivity includes the open support interval, not its endpoints.

**[Partition of unity](../../../../../partition-of-unity.md).** The translates of $B_1$ cover the line exactly once under the half-open convention. Nonnegativity permits interchange of sum and integral, and induction gives

$$
\sum_{j\in\mathbb Z}B_m(x-j)
=\int_0^1\sum_{j\in\mathbb Z}B_{m-1}(x-u-j)\,du
=1.
$$

Thus $\boxed{\sum_jB_m(x-j)=1}$, a locally finite sum. Each $B_m$ also has integral one, although [partition of unity](../../../../../partition-of-unity.md) does not mean its maximum value is one.

For $m\geq2$, repeated integration gives the explicit truncated-power form

$$
B_m(x)=\frac1{(m-1)!}\sum_{j=0}^m(-1)^j\binom mj(x-j)_+^{m-1}.
$$

On each unit knot interval this is a [polynomial](../../../../../polynomial-split.md) of degree at most $m-1$, and on $(0,1)$ it is $x^{m-1}/(m-1)!$, so the degree is attained. Each truncated power has $m-2$ continuous [derivatives](../../../../../derivative.md); the [derivative](../../../../../derivative.md) of order $m-1$ jumps at the first knot. Therefore the dependence on the projected box dimension is

$$
\boxed{\text{degree }m-1,\qquad \text{continuity }C^{m-2},\qquad
\text{support width }m\text{ in unit knot intervals}.}
$$

For $m=1$ the pieces are constants and the function is discontinuous at the knots. If geometric width is measured under orthogonal projection onto the unit diagonal instead, the projected coordinate is $x/\sqrt m$, so the physical support width is $\sqrt m$; its unit-mass density is $\sqrt m B_m(\sqrt m\,x)$. These are different scalings of the same cardinal [spline](../../../../../spline-mathematics.md), not different [continuity](../../../../../continuous-function.md) or degree claims.

For a bivariate [box spline](../../../../../box-spline.md), choose a spanning direction [matrix](../../../../../matrix.md) $\Xi=(\xi_1,\ldots,\xi_m)$ in the plane and project the unit cube by $u\mapsto\Xi u$. Define its normalization by

$$
\int_{\mathbb R^2}M_\Xi(x)\varphi(x)\,dx
=\int_{[0,1]^m}\varphi(\Xi u)\,du.
$$

The support is the [zonotope](../../../../../zonotope.md) $\sum_r[0,1]\xi_r$, and the [polynomial](../../../../../polynomial-split.md) pieces generally have total degree $m-2$. The grid comes from the chosen direction families and their lattice translates. Two independent directions, with repetitions, give tensor-product [B-splines](../../../../../b-spline.md) on a parallelogram grid. Three families such as $e_1,e_2,e_1+e_2$ give a three-direction triangular grid; an affine change of basis can make it the usual equilateral triangular grid. The four families $e_1,e_2,e_1+e_2,e_1-e_2$ give the criss-cross square grid and the [quadratic four-direction box spline](../../../../../quadratic-four-direction-box-spline.md). Changing the direction [matrix](../../../../../matrix.md) and repeating directions therefore changes the grid, support and smoothness while retaining the box-projection construction.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 68](../../paper-68-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
