<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [orthogonal projection](../../../../../orthogonal-projection.md) is $p_n=\sum_{r=0}^n(u,\phi_r)\phi_r$. Subtract it from $u$ and use the [orthonormal basis](../../../../../orthonormal-basis.md) relations to obtain

$$
0\leq\|u-p_n\|_2^2=\|u\|_2^2-\sum_{r=0}^n(u,\phi_r)^2.
$$

This is the requested [Bessel inequality](../../../../../bessel-s-inequality.md).

For the infinite tail, use completeness of the orthonormal [polynomial](../../../../../polynomial-split.md) family in the usual weighted [L2 space](../../../../../l2-space-is-a-hilbert-space.md). The relevant density facts are that continuous functions are dense for the finite measure $w(x)\,dx$, and the [Weierstrass approximation theorem](../../../../../weierstrass-approximation-theorem.md) makes [polynomials](../../../../../polynomial-split.md) uniformly dense in continuous functions on the compact interval. Since $\int w<\infty$, uniform approximation also gives weighted [L2 norm](../../../../../l2-norm.md) approximation. [Parseval's identity](../../../../../parseval-identity.md) therefore gives

$$
\boxed{\|u-p_n\|_2^2=\sum_{r=n+1}^\infty(u,\phi_r)^2.}
$$

Here finiteness of the weight integral is also necessary for the constant [polynomial](../../../../../polynomial-split.md) to belong to the stated Hilbert space. Without completeness of the polynomial family, an additional squared component orthogonal to every [polynomial](../../../../../polynomial-split.md) would remain; [Bessel inequality](../../../../../bessel-s-inequality.md) alone does not justify equality.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the approximation theory and finite element methods course of the University of Oxford](../../../../split.md)
6. [Approximation theory and finite element methods course of the University of Oxford](../../../../../approximation-theory-and-finite-element-methods-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
