<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The weight is strictly positive and all its [polynomial](../../../polynomial-split.md) moments are finite. Thus the given integral is a [inner product](../../../inner-product-split.md): for a nonzero [polynomial](../../../polynomial-split.md), its square is positive on a nonempty interval, so its weighted integral is strictly positive.

In the [finite-dimensional vector space](../../../finite-dimensional-vector-space.md) $V_n$, subtract the [orthogonal projection onto a finite-dimensional subspace](../../../orthogonal-projection-onto-a-finite-dimensional-subspace.md) of $x^n$ onto $V_{n-1}$:

$$
\phi_n=x^n-\operatorname{proj}_{V_{n-1}}x^n.
$$

This is monic, since the subtracted [polynomial](../../../polynomial-split.md) has lower degree, and is orthogonal to every lower-degree [polynomial](../../../polynomial-split.md). If $\phi_n,\psi_n$ were two such [monic polynomials](../../../monic-polynomial.md), their difference would lie in $V_{n-1}$ and be orthogonal to that space. Taking its [inner product](../../../inner-product-split.md) with itself gives zero, hence the difference vanishes. This proves existence and uniqueness for every $n$, with $\phi_0=1$.

Odd moments vanish because the weight is even; the even moments are

$$
\int_{\mathbb R}e^{-|x|}x^{2k}dx
=2\int_0^\infty e^{-x}x^{2k}dx=2(2k)!.
$$

Consequently $\phi_1=x$, while a monic quadratic orthogonal to $x$ has no linear term, and orthogonality to one gives its constant term $-4/2=-2$. Thus

$$
\boxed{\phi_0=1,\qquad\phi_1=x,\qquad\phi_2=x^2-2.}
$$

Finally $(-1)^n\phi_n(-x)$ is also monic and orthogonal to every lower-degree [polynomial](../../../polynomial-split.md), by the change of variable $x\mapsto-x$. Uniqueness implies $\phi_n(-x)=(-1)^n\phi_n(x)$. In particular $\phi_{2007}$ is odd and

$$
\boxed{[x^{2000}]\phi_{2007}=0.}
$$

This is [parity of monic orthogonal polynomials for an even weight](../../../parity-of-monic-orthogonal-polynomials-for-an-even-weight.md).

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2007](../../2007-split.md)
3. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../split.md)
4. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
5. [Year 2 of the mathematics course of the University of Oxford](../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
6. [Mathematics course of the University of Oxford](../../../mathematics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
