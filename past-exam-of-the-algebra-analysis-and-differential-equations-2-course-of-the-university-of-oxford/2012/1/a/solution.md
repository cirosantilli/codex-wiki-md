<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [minimal polynomial](../../../../minimal-polynomial.md) $m_T(t)$ is the unique monic [polynomial](../../../../polynomial-split.md) of least positive [polynomial degree](../../../../degree-of-a-polynomial.md) satisfying $m_T(T)=0$. Such an annihilating [polynomial](../../../../polynomial-split.md) exists without using the [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md): the [vector space](../../../../vector-space-split.md) $\operatorname{End}(V)$ has [dimension of a vector space](../../../../dimension-vector-space.md) equal to $n^2$, so $I,T,\ldots,T^{n^2}$ are [linearly dependent](../../../../linear-dependence.md). Normalize a nonzero annihilating [polynomial](../../../../polynomial-split.md) to be monic and choose one of least degree. Two distinct monic choices of that degree would have an annihilating difference of lower degree, contradicting minimality. A nonzero constant cannot annihilate $T$ because $V\ne0$.

Choose a [basis](../../../../basis.md) $B$ and let $A=[T]_B$. The [characteristic polynomial](../../../../characteristic-polynomial.md) is

$$
\boxed{\chi_T(t)=\det(tI-A).}
$$

It is independent of the chosen [basis](../../../../basis.md). Indeed a change of basis replaces $A$ by a [similar matrix](../../../../matrix-similarity.md) $P^{-1}AP$, and

$$
\det(tI-P^{-1}AP)=\det\bigl(P^{-1}(tI-A)P\bigr)=\det(tI-A)
$$

by multiplicativity of the [determinant](../../../../determinant.md). Thus this monic degree-$n$ [polynomial](../../../../polynomial-split.md) is an invariant of the [linear transformation](../../../../linear-map.md) itself.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
