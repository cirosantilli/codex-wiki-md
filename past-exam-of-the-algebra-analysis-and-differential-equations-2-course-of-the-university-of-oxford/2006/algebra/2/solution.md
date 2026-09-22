<h1 id="algebra/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [dual space](../../../../dual-space-split.md) $V^*$ is the [vector space](../../../../vector-space-split.md) of [linear maps](../../../../linear-map.md) $V\to\mathbb F$, with pointwise operations. For the given [basis](../../../../basis.md) define coordinate forms $e^i$ by $e^i(\sum_ja_je_j)=a_i$. These are linear and satisfy $e^i(e_j)=\delta_{ij}$. If $\sum_ic_ie^i=0$, evaluation at $e_j$ gives $c_j=0$. For every [linear form](../../../../linear-functional.md) $\phi$,

$$
\phi(v)=\sum_i\phi(e_i)e^i(v),
$$

so the coordinate forms span the dual and form its [dual basis](../../../../dual-basis.md).

In the [polynomial](../../../../polynomial-split.md) example write $p(X)=a+bX+cX^2$. Then

$$
\phi_1(p)=a,\qquad\phi_2(p)=a+b+c,\qquad\phi_3(p)=a-b+c.
$$

These recover all three [coefficients](../../../../coefficient.md), so they span $V^*$ and, since the dual has [dimension](../../../../dimension-vector-space.md) three, form a [basis](../../../../basis.md). Explicitly the [basis](../../../../basis.md) dual to $1,X,X^2$ is

$$
\boxed{e^1=\phi_1,\qquad e^2=\frac{\phi_2-\phi_3}2,\qquad e^3=\frac{\phi_2+\phi_3}2-\phi_1.}
$$

Evaluation on the three monomials verifies the dual-[basis](../../../../basis.md) identities directly.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [Algebra](../../algebra.md)
3. [2006](../../../2006-split.md)
4. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
