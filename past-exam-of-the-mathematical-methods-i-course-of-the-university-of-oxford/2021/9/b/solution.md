<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First check that the proposed space is closed under the stated operations: $|\alpha a_i+b_i|^2\le2\alpha^2a_i^2+2b_i^2$, and summing gives a finite result. For any finite $N$, the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_{i=1}^N|a_ib_i|
\le\left(\sum_{i=1}^Na_i^2\right)^{1/2}
\left(\sum_{i=1}^Nb_i^2\right)^{1/2}
\le\|A\|_2\|B\|_2.
$$

The left side is an increasing, bounded sequence of real numbers. Its [limit](../../../../limit-of-a-function.md) exists, proving [absolute convergence](../../../../absolute-convergence.md) of $\sum_i a_ib_i$. This justifies termwise addition and scalar multiplication in the defining sum. Symmetry and [bilinearity](../../../../bilinearity.md) follow, while $\langle A,A\rangle=\sum_i a_i^2\ge0$, with equality only when every $a_i=0$. Thus it is a real [inner product](../../../../inner-product-split.md) on the real [l2 sequence space](../../../../l2-sequence-space.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [9](../../9.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
