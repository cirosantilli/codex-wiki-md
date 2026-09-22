<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For the weighted [inner product](../../../../../inner-product-split.md), $(x^j,x^k)=1/(j+k+2)$. Start [Gram-Schmidt process](../../../../../gram-schmidt-process.md) with the monomials and choose monic normalization:

$$
\phi_0=1,\qquad
\phi_1=x-\frac{(x,1)}{(1,1)}=x-\frac23.
$$

Its squared [norm](../../../../../norm.md) is $1/4-4/9+2/9=1/36$. Next $(x^2,1)/(1,1)=1/2$ and

$$
(x^2,\phi_1)=\frac15-\frac16=\frac1{30},
\qquad\frac{(x^2,\phi_1)}{\|\phi_1\|_2^2}=\frac65.
$$

Therefore

$$
\boxed{\phi_0=1,\qquad\phi_1=x-\frac23,\qquad
\phi_2=x^2-\frac65x+\frac3{10}.}
$$

Subtracting these [orthogonal](../../../../../orthogonal-vectors.md) projections gives [orthogonality](../../../../../orthogonal-vectors.md) by construction; independent nonzero rescalings would give equivalent unnormalized [orthogonal](../../../../../orthogonal-vectors.md) [polynomials](../../../../../polynomial-split.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
