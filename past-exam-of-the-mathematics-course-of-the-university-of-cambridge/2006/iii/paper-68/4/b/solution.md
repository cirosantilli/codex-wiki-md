<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a partition $0=x_0<x_1<\cdots<x_N=1$, with the usual nodal [piecewise-linear hat functions](../../../../../../piecewise-linear-hat-function.md) $\phi_i$, including the half hats at the endpoints. Write $u_h=\sum_{i=0}^NU_i\phi_i$ with $U_0=1$. Differentiating the [Ritz method](../../../../../../rayleigh-ritz-method.md) energy with respect to $U_i$, $1\le i\le N$, gives

$$
\sum_{j=0}^NA_{ij}U_j=0,\qquad A_{ij}=\int_0^1(\phi_i'\phi_j'+x\phi_i\phi_j)dx.
$$

On an element $[a,b]$ of length $\ell$, its two basis functions are $(b-x)/\ell$ and $(x-a)/\ell$. Direct integration yields the element [matrix](../../../../../../matrix.md)

$$
\boxed{A^{[a,b]}=\frac1\ell\begin{pmatrix}1&-1\\-1&1\end{pmatrix}
+\frac\ell{12}\begin{pmatrix}3a+b&a+b\\a+b&a+3b\end{pmatrix}.}
$$

For example the first weighted diagonal is $\int_a^bx(b-x)^2/\ell^2\,dx=\ell(3a+b)/12$; the off-diagonal is $\int_a^bx(b-x)(x-a)/\ell^2\,dx=\ell(a+b)/12$. This gives the [affine-weighted hat mass matrix](../../../../../../affine-weighted-hat-mass-matrix.md) and explicit equations on any partition by assembling adjacent elements.

For the uniform choice $h=1/N$, $x_i=ih$, the assembled interior equations are

$$
\boxed{\left[-\frac1h+\frac h{12}(2x_i-h)\right]U_{i-1}
+\left[\frac2h+\frac{2hx_i}{3}\right]U_i
+\left[-\frac1h+\frac h{12}(2x_i+h)\right]U_{i+1}=0,\quad1\le i<N.}
$$

The last node contributes only one element, so its equation is

$$
\boxed{\left[-\frac1h+\frac h{12}(2-h)\right]U_{N-1}
+\left[\frac1h+\frac h3-\frac{h^2}{12}\right]U_N=0,\qquad U_0=1.}
$$

In the first interior equation the known $U_0$ term moves to the right, giving $1/h-h^2/12$. For $N=1$ only the endpoint equation is needed. The last row enforces the weak [Neumann boundary condition](../../../../../../neumann-boundary-condition.md), so no artificial value outside the interval is introduced. The [matrix](../../../../../../matrix.md) on $U_1,\ldots,U_N$ is a [symmetric positive-definite matrix](../../../../../../symmetric-positive-definite-matrix.md): its [quadratic form](../../../../../../quadratic-form.md) is $a(v_h,v_h)>0$ for every nonzero trial variation $v_h$. The discrete minimizer is therefore unique.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 68](../../../paper-68-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
