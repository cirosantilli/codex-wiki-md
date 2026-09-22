<h1 id="p/p4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [degree](../../../../../degree-graph-theory.md)-ordered [orthogonal](../../../../../orthogonal-vectors.md) [polynomials](../../../../../polynomial-split.md) identified in (b); otherwise the printed nodes need not exist. Let $\ell_j$ be the [degree](../../../../../degree-graph-theory.md)-$n$ [Lagrange interpolation polynomial](../../../../../lagrange-polynomial.md) with $\ell_j(x_i)=\delta_{ij}$ and set $w_j=\int_a^b\ell_j(x)w(x)dx$.

For any $f\in\Pi_{2n+1}$, [polynomial division](../../../../../polynomial-division.md) gives $f=p_{n+1}s+r$ with $\deg s\le n$ and $\deg r\le n$. [Orthogonality](../../../../../orthogonal-vectors.md) gives $\int p_{n+1}sw=0$, while this product also vanishes at every node. The interpolation formula for $r$ then proves

$$
\boxed{\int_a^bf(x)w(x)dx=\sum_{j=0}^nw_jf(x_j).}
$$

Apply this exactness to $\ell_j^2$, of [degree](../../../../../degree-graph-theory.md) at most $2n$. It gives $w_j=\int_a^b\ell_j(x)^2w(x)dx>0$, because $\ell_j$ is not the zero [polynomial](../../../../../polynomial-split.md). Thus all [quadrature weights](../../../../../quadrature-weight.md) are actually strictly positive, stronger than the requested nonnegativity. Here exactness is for the weighted integral defined at the start of the question.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [P4](../../p4.md)
3. [P](../../../p.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
