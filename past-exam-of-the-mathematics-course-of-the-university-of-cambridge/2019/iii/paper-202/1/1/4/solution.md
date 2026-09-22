<h1 id="1/1/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

[Itô formula](../../../../../../../ito-s-lemma.md) gives

$$
dM_t=M_t\nabla f(B_t)\cdot dB_t,
$$

so $M$ is a positive [local martingale](../../../../../../../local-martingale.md). On every finite interval $[0,T]$, the hypotheses imply

$$
\int_0^T|\nabla f(B_s)|^2ds
\leq C_T\left(1+\sup_{s\leq T}|B_s|^{2-\epsilon}\right).
$$

The [Gaussian tail bound](../../../../../../../gaussian-tail-bound.md) of the Brownian maximum has finite exponential moments of every subquadratic power. Therefore [Novikov condition](../../../../../../../novikov-s-condition.md) holds on $[0,T]$, and the [stochastic exponential](../../../../../../../doleans-dade-exponential.md) $M$ is a true martingale there. Since $T$ was arbitrary, **$M$ is a true martingale**.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [1](../../1.md)
3. [1](../../../1.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
