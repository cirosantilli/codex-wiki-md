<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The [homogeneous coordinate ring](../../../../homogeneous-coordinate-ring.md) of the Segre [image](../../../../image-of-a-function.md) is the subalgebra $k[x_iy_j]\subseteq k[x_0,\ldots,x_n,y_0,\ldots,y_m]$, grading each [product](../../../../product-of-numbers.md) $x_iy_j$ as degree one. Its degree-$t$ part is precisely the space of [polynomials](../../../../polynomial-split.md) bihomogeneous of bidegree $(t,t)$.

Indeed, every [product](../../../../product-of-numbers.md) of $t$ generators has those two degrees. Conversely, any [monomial](../../../../monomial.md) of bidegree $(t,t)$ can pair its $t$ individual $x$ factors with its $t$ individual $y$ factors, expressing it as a [product](../../../../product-of-numbers.md) of generators. The distinct resulting [monomials](../../../../monomial.md) are [linearly independent](../../../../linear-independence.md). Counting them gives

$$
\boxed{P_X(t)=\binom{t+n}{n}\binom{t+m}{m}.}
$$

In fact this agrees with the [Hilbert function](../../../../hilbert-function.md) for every integer $t\geq0$. Its [leading coefficient](../../../../leading-coefficient-of-a-polynomial.md) is $1/(n!m!)$, so the two degree quantities are

$$
\boxed{\deg P_X=n+m,\qquad\deg X=\frac{(n+m)!}{n!m!}=\binom{n+m}{n}.}
$$

Thus the Segre [variety](../../../../algebraic-variety-split.md) has [dimension](../../../../dimension-of-an-algebraic-set.md) $n+m$ and embedded projective degree $\binom{n+m}{n}$.

This gives the [Segre Hilbert polynomial and degree](../../../../segre-hilbert-polynomial-and-degree.md) directly from its graded [monomials](../../../../monomial.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebraic Geometry course of the University of Oxford](../../../split.md)
5. [Algebraic Geometry course of the University of Oxford](../../../../algebraic-geometry-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
