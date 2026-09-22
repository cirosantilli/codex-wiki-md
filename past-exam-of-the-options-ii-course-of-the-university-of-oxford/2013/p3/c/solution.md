<h1 id="p3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The degree-zero [polynomial](../../../../polynomial-split.md) is constant and therefore even. Assume inductively that $p_j(-x)=(-1)^jp_j(x)$ for $j<k$. Define $q_k(x)=(-1)^kp_k(-x)$, which has the same leading coefficient as $p_k$.

Changing variable $x\mapsto-x$ and using the even weight and inductive hypothesis gives $\langle q_k,p_j\rangle_w=(-1)^{k+j}\langle p_k,p_j\rangle_w=0$ for $j<k$. Hence $q_k-p_k$ has degree below $k$ and is orthogonal to every $p_0,\ldots,p_{k-1}$. Those [polynomials](../../../../polynomial-split.md) form a basis for the [polynomials](../../../../polynomial-split.md) of degree below $k$, so the difference is orthogonal to itself. Positivity of the weighted [inner product](../../../../inner-product-split.md) forces it to be zero.

Therefore

$$
\boxed{p_k(-x)=(-1)^kp_k(x),}
$$

completing the induction and proving [parity of orthogonal polynomials for an even weight](../../../../parity-of-orthogonal-polynomials-for-an-even-weight.md). Thus even indices give even [functions](../../../../function-split.md) and odd indices give odd [functions](../../../../function-split.md), regardless of the nonzero normalization chosen.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [P3](../../p3.md)
3. [2013](../../../2013-split.md)
4. [Past exam of the options II course of the University of Oxford](../../../split.md)
5. [Options II course of the University of Oxford](../../../../options-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
