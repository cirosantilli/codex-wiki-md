<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Assume first that $\|P_n\|\leq M$ for all $n$. Given $x\in X$ and $\epsilon>0$, choose a finite linear combination $y$ of the $x_i$ with $\|x-y\|<\epsilon/(M+1)$. For all sufficiently large $n$, $P_ny=y$. Therefore

$$
\|P_nx-x\|\leq\|P_n(x-y)\|+\|y-x\|\leq(M+1)\|x-y\|<\epsilon.
$$

Thus $P_nx\to x$, and the formula in part (iii) yields the norm-convergent expansion

$$
\boxed{x=\sum_{i=1}^\infty x_i^*(x)x_i.}
$$

This proves the stated existence of coefficients.

Conversely, suppose every $x$ has some norm-convergent expansion $x=\sum_i\alpha_ix_i$. Applying the continuous functional $x_j^*$ to its partial sums and passing to the limit gives $\alpha_j=x_j^*(x)$. Hence those partial sums are precisely $P_nx$, so $P_nx\to x$ for every $x$. In particular $\sup_n\|P_nx\|<\infty$ for each fixed $x$. The [Uniform boundedness principle](../../../../uniform-boundedness-principle.md), using completeness of $X$, now gives

$$
\boxed{\sup_n\|P_n\|<\infty.}
$$

This proves the reverse implication. The coefficients are automatically unique, so the equivalence is the [uniform partial-sum criterion for a Schauder basis](../../../../uniform-partial-sum-criterion-for-a-schauder-basis.md) for the given minimal total [sequence](../../../../sequence.md). Its projection bound is the [basis constant](../../../../basis-constant.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the functional analysis course of the University of Oxford](../../../split.md)
5. [Functional analysis course of the University of Oxford](../../../../functional-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
