<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $x=\cos\theta$ in the [weighted inner product](../../../../weighted-inner-product.md). Since $T_r(\cos\theta)=\cos(r\theta)$,

$$
(T_r,T_s)=\int_0^\pi\cos(r\theta)\cos(s\theta)\,d\theta
=\begin{cases}\pi,&r=s=0,\\\pi/2,&r=s\geq1,\\0,&r\ne s.\end{cases}
$$

The last equality follows by the product-to-sum [trigonometric identity](../../../../trigonometric-identity.md) and integration. Thus these are nonzero mutually [orthogonal polynomials](../../../../orthogonal-polynomial-split.md). The first $n+1$ are [linearly independent](../../../../linear-independence.md), and the [vector space](../../../../vector-space-split.md) $P_n$ has dimension $n+1$; therefore $\boxed{P_n=\operatorname{span}(T_0,\ldots,T_n)}$.

For any $q\in P_n$, the function of the real parameter $t$

$$
\|u-p_n-tq\|_2^2=\|u-p_n\|_2^2-2t(u-p_n,q)+t^2\|q\|_2^2
$$

has a minimum at $t=0$. Its [derivative](../../../../derivative.md) there vanishes, proving $\boxed{(u-p_n,q)=0}$. This is precisely the defining orthogonality of an [orthogonal projection](../../../../orthogonal-projection.md), or a [least-squares polynomial in an orthogonal-polynomial basis](../../../../least-squares-polynomial-in-an-orthogonal-polynomial-basis.md). Conversely, this condition and the [Pythagorean theorem for inner product spaces](../../../../pythagorean-theorem-in-an-inner-product-space.md) give $\|u-q\|_2^2=\|u-p_n\|_2^2+\|p_n-q\|_2^2$, proving the minimum and its uniqueness.

Expand $p_n=\sum_{r=0}^n a_rT_r$ in the [basis](../../../../basis.md) already established and take the [inner product](../../../../inner-product-split.md) with $T_s$. [Orthogonality](../../../../orthogonal-vectors.md) leaves $a_s(T_s,T_s)=(u,T_s)$, so

$$
\boxed{a_r=\frac{(u,T_r)}{(T_r,T_r)},\qquad p_n=\sum_{r=0}^n a_rT_r.}
$$

In particular $a_0=\pi^{-1}\int_0^\pi u(\cos\theta)\,d\theta$ and $a_r=2\pi^{-1}\int_0^\pi u(\cos\theta)\cos(r\theta)\,d\theta$ for $r\geq1$. These are the corresponding [Chebyshev series](../../../../chebyshev-series.md) coefficients with the constant coefficient convention used in this question.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the approximation of functions course of the University of Oxford](../../../split.md)
5. [Approximation of functions course of the University of Oxford](../../../../approximation-of-functions-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
