<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take a [singular value decomposition](../../../../singular-value-decomposition.md) $F=Q_1DQ_2^T$, with $D=\operatorname{diag}(\lambda_1,\lambda_2,\lambda_3)$ positive and $Q_1,Q_2\in SO(3)$. Such a choice is possible because $\det F>0$. Left [material frame indifference](../../../../material-frame-indifference.md) removes $Q_1$, and right [material isotropy](../../../../material-isotropy.md) removes $Q_2$, giving $W(F)=W(D)$.

Moreover $W(D)$ is unchanged when the positive diagonal entries are permuted. Every [permutation](../../../../permutation.md) can be implemented by a signed [permutation matrix](../../../../permutation-matrix.md) of [determinant](../../../../determinant.md) one; the signs disappear in conjugating a [diagonal matrix](../../../../diagonal-matrix.md). Thus the energy depends only on the unordered [principal stretches](../../../../principal-stretch.md).

The three invariants determine precisely this unordered triple: the roots of $t^3-I_Bt^2+II_Bt-III_B$ are $\lambda_1^2,\lambda_2^2,\lambda_3^2$, and their positive [square roots](../../../../square-root.md) give the stretches. Consequently, on the set of admissible invariant triples, define $h(I_B,II_B,III_B)$ to be $W(D)$. The preceding argument proves that this is well defined and that

$$
\boxed{W(F)=h(I_B,II_B,III_B).}
$$

Not every positive triple is realizable by three positive roots. Since the requested statement only asserts existence of a [function](../../../../function-split.md) on $(0,\infty)^3$, extend $h$ arbitrarily on the nonrealizable triples; no choice there affects the formula for a [deformation in continuum mechanics](../../../../deformation-mechanics.md). Smooth invariant representations, where needed for differentiating the [constitutive equation](../../../../constitutive-equation.md), are understood locally on the realizable set.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the solid mechanics course of the University of Oxford](../../../split.md)
5. [Solid mechanics course of the University of Oxford](../../../../solid-mechanics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
