<h1 id="section-a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Apply the [implicit midpoint rule](../../../../../../../implicit-midpoint-rule.md), equivalently the [Crank-Nicolson method](../../../../../../../crank-nicolson-method.md), to the semidiscrete equation:

$$
i\frac{\mathbf u^{n+1}-\mathbf u^n}{\Delta t}
=H_h\frac{\mathbf u^{n+1}+\mathbf u^n}{2}.
$$

It has order two. Its amplification matrix is the [Cayley transform](../../../../../../../cayley-transform-of-a-hermitian-matrix.md)

$$
Q=\left(I+\frac{i\Delta t}{2}H_h\right)^{-1}
\left(I-\frac{i\Delta t}{2}H_h\right).
$$

Because $H_h$ is Hermitian, $Q$ is unitary. Hence $\|\mathbf u^{n+1}\|_2=\|\mathbf u^n\|_2$ exactly.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Section A](../../../section-a.md)
4. [Paper 341](../../../../paper-341-split.md)
5. [Iii](../../../../split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
