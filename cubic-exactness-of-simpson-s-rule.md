<h1 id="cubic-exactness-of-simpson-s-rule">Cubic exactness of Simpson's rule</h1>

↑ **Parent:** [Simpson's rule](simpson-s-rule.md)

[Polynomial interpolation](polynomial-interpolation.md) makes [Simpson's rule](simpson-s-rule.md) exact for every [polynomial](polynomial-split.md) of [polynomial degree](degree-of-a-polynomial.md) at most two. To understand the extra [polynomial degree](degree-of-a-polynomial.md), centre the coordinate at the [midpoint](midpoint.md): $y=x-m$, with endpoints $-h,h$. For any [cubic polynomial](cubic-polynomial.md) $p$, let $p_2$ be its interpolating [quadratic polynomial](quadratic-polynomial.md). The [polynomial](polynomial-split.md) $p-p_2$ vanishes at all three [quadrature nodes](quadrature-node.md), so

$$
p(x)-p_2(x)=A(x-a)(x-m)(x-b)=A y(y^2-h^2),
$$

where $A$ is the coefficient of $x^3$ in $p$. As a [function](function-split.md) of $y$, this is an [odd function](odd-function.md), whose [integral](integral-split.md) over the symmetric [interval](interval-mathematics.md) $[-h,h]$ is zero. Hence integrating $p_2$ also integrates $p$ exactly. This is the symmetry mechanism in the [nodal-polynomial criterion for quadrature exactness](nodal-polynomial-criterion-for-quadrature-exactness.md).

In the worked example, the [polynomial](polynomial-split.md) difference factors as

$$
f(x)-p_2(x)=(x+1)(x-1/2)(x-2)
=y^3-\frac94y.
$$

Its [definite integrals](definite-integral.md) on $[-1,1/2]$ and $[1/2,2]$ are respectively $81/64$ and $-81/64$. Their cancellation concerns signed [integrals](integral-split.md), rather than pointwise accuracy of [polynomial interpolation](polynomial-interpolation.md).

The [degree of precision of a quadrature rule](degree-of-precision-of-a-quadrature-rule.md) stops at three: on the same [interval](interval-mathematics.md), the [monomial](monomial.md) $x^4$ gives $S(x^4)=69/8$, whereas $\int_{-1}^{2}x^4\,dx=33/5$. Their difference, exact [integral](integral-split.md) minus approximation, is $-81/40$.

## ↑ Ancestors (8)

1. [Simpson's rule](simpson-s-rule.md)
2. [Quadrature rule](quadrature-rule.md)
3. [Numerical integration](numerical-integration-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)
