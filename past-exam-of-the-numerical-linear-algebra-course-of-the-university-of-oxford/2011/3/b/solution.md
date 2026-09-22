<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The exact minimization gives $r_{j+1}=r_j-\alpha_jAp_j$, with $\alpha_j=p_j^Tr_j/(p_j^TAp_j)$. For [steepest descent method](../../../../gradient-descent-split.md), the next [search direction](../../../../search-direction.md) is $p_{j+1}=r_{j+1}$. Hence

$$
\boxed{p_j^Tp_{j+1}=p_j^Tr_j-\alpha_jp_j^TAp_j=0.}
$$

Thus consecutive nonzero [search directions](../../../../search-direction.md) are [orthogonal](../../../../orthogonal-vectors.md). This calculation even covers an arbitrary initial direction $p_1$, as in the generic algorithm: it only needs the exact preceding line minimization and the choice $p_{j+1}=r_{j+1}$. If the new [linear-system residual](../../../../linear-system-residual.md) is zero, the [linear system](../../../../system-of-linear-equations.md) is already solved. No pairwise orthogonality of all nonconsecutive directions is asserted.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical linear algebra course of the University of Oxford](../../../split.md)
5. [Numerical linear algebra course of the University of Oxford](../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
