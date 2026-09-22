<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [Leibniz formula for determinants](../../../leibniz-formula-for-determinants.md):

$$
\det M=\sum_{\sigma\in S_n}\operatorname{sgn}(\sigma)\prod_{j=1}^n m_{j,\sigma(j)}.
$$

For a nonzero product in an [upper triangular matrix](../../../upper-triangular-matrix.md), every selected column must satisfy $\sigma(j)\geq j$. But a [permutation](../../../permutation.md) has $\sum_j\sigma(j)=\sum_jj$, so every one of these inequalities is an equality. Only the identity [permutation](../../../permutation.md) can contribute. Its sign is positive and its product is $\prod_jm_{jj}$, which proves the result even if some diagonal entries vanish.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2019 resit](../../2019-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
