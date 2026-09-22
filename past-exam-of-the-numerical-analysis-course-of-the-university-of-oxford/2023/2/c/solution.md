<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Clearing the denominators in the [rational interpolation](../../../../rational-interpolation.md) conditions gives

$$
\boxed{\sum_{j=0}^m a_jx_i^j+
f_i\sum_{j=0}^{\ell-1}b_jx_i^j=f_ix_i^\ell,
\qquad i=0,\ldots,n.}
$$

These are $n+1$ linear equations for $(m+1)+\ell=n+1$ unknowns. The $i$th row of the coefficient [matrix](../../../../matrix.md), in the order $a_0,\ldots,a_m,b_0,\ldots,b_{\ell-1}$, is

$$
\left(1,x_i,\ldots,x_i^m,\ f_i,f_ix_i,\ldots,f_ix_i^{\ell-1}\right).
$$

This [rational interpolation linearization](../../../../rational-interpolation-linearization.md) is equivalent to the original fraction conditions only if $r(x_i)\ne0$ at every [interpolation node](../../../../interpolation-node.md). If $r(x_i)=0$, the cleared equation merely forces $q(x_i)=0$, leaving the fraction undefined.

For $f_i=x_i^{m+1}$, the coefficient row becomes

$$
(1,x_i,\ldots,x_i^m,x_i^{m+1},\ldots,x_i^{m+\ell})
=(1,x_i,\ldots,x_i^n).
$$

This is the [Vandermonde matrix](../../../../vandermonde-matrix.md), whose [determinant](../../../../determinant.md) is $\prod_{0\leq i<j\leq n}(x_j-x_i)\ne0$. Equivalently, a vector in its [null space](../../../../kernel-of-a-linear-map-split.md) would define a degree-at-most-$n$ [polynomial](../../../../polynomial-split.md) vanishing at all $n+1$ distinct [interpolation nodes](../../../../interpolation-node.md), which is zero by the preceding uniqueness proof. Thus the cleared [linear system](../../../../system-of-linear-equations.md) has exactly one solution.

There is also a constructive description of that solution. Define the [monic polynomial](../../../../monic-polynomial.md)

$$
W(x)=\prod_{i=0}^n(x-x_i).
$$

The [polynomial](../../../../polynomial-split.md) $x^{m+1}r(x)-q(x)$ is monic of degree $n+1$ and vanishes at every [interpolation node](../../../../interpolation-node.md). It must therefore equal $W(x)$. By [polynomial division](../../../../polynomial-division.md), write uniquely

$$
W(x)=x^{m+1}R(x)+S(x),\qquad\deg S\leq m.
$$

The quotient $R$ is monic of degree $\ell$, and

$$
\boxed{r(x)=R(x),\qquad q(x)=-S(x)}
$$

is the unique coefficient solution. This does not assert that $R$ is nonzero at every [interpolation node](../../../../interpolation-node.md).

For a counterexample with $m=0$, $\ell=1$, choose $x_0=0,x_1=1$ and the specified data $f_i=x_i$, so $f_0=0,f_1=1$. The cleared equations reduce to

$$
a_0=0,\qquad a_0+b_0=1,
$$

giving the unique solution $q(x)=0$, $r(x)=x-1$. But at $x_1=1$ the quotient is $0/0$. Indeed, any genuine [rational interpolant](../../../../rational-interpolant.md) of this prescribed form would need $r(0)\ne0$; then $q(0)/r(0)=0$ forces the constant numerator to be zero. At a nonzero denominator its value at $1$ would also be zero, never one. Cancelling the common factor in the cleared candidate would merely give the identically zero [rational function](../../../../rational-function.md), which still fails the data. Hence

$$
\boxed{(x_0,f_0)=(0,0),\ (x_1,f_1)=(1,1):
\quad\text{unique cleared solution, but no rational interpolant}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
