<h1 id="p/p4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**An arbitrary [orthonormal basis](../../../../../orthonormal-basis.md) does not have the printed property.** For example on $[-1,1]$ with $w=1$, take the usual normalized constant and linear [Legendre polynomials](../../../../../legendre-polynomial.md) and swap their labels $p_0,p_1$. The resulting family is still an [orthonormal basis](../../../../../orthonormal-basis.md) but $p_0$ has one zero, rather than zero. The necessary intended hypothesis is that $p_k$ has [degree](../../../../../degree-graph-theory.md) $k$, or equivalently that the [basis](../../../../../basis.md) is obtained by orthogonalizing $1,x,x^2,\ldots$ in that order.

Under this hypothesis, $p_k$ is [orthogonal](../../../../../orthogonal-vectors.md) to every [polynomial](../../../../../polynomial-split.md) of [degree](../../../../../degree-graph-theory.md) less than $k$. Let $t_1,\ldots,t_s$ be its sign-changing zeros in $(a,b)$ and put $q(x)=\prod_{j=1}^s(x-t_j)$. If $s<k$, then $p_kq$ has a constant nonzero sign except at finitely many points: each interior sign change has been canceled, and all remaining zeros have even multiplicity or occur at endpoints. Since $w>0$, its integral cannot vanish. But [orthogonality](../../../../../orthogonal-vectors.md) to $q$, of [degree](../../../../../degree-graph-theory.md) $s<k$, says that integral is zero, a contradiction. Thus $s\ge k$. Since the [polynomial](../../../../../polynomial-split.md) has [degree](../../../../../degree-graph-theory.md) $k$, it follows that

$$
\boxed{p_k\text{ has exactly }k\text{ distinct simple zeros, all in }(a,b).}
$$

This proves the requested conclusion in its standard intended setting and explains why it does not follow from the literal [basis](../../../../../basis.md) statement alone.

## ↑ Ancestors (13)

1. [B](../b.md)
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
