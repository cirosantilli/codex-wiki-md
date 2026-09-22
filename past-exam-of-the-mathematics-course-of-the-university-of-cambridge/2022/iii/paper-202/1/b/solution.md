<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [simple predictable process](../../../../../../simple-predictable-process.md)

$$
H_s=\sum_{i=0}^{n-1}H_i\mathbf1_{(t_i,t_{i+1}]}(s),
\qquad H_i\in L^\infty(\mathcal F_{t_i}),
$$

define

$$
(H\mathbin\cdot M)_t
=\sum_{i=0}^{n-1}H_i
\bigl(M_{t\wedge t_{i+1}}-M_{t\wedge t_i}\bigr).
$$

Each summand is a bounded predictable multiple of a martingale increment, so conditional expectation proves that $H\mathbin\cdot M$ is a martingale. Orthogonality of disjoint martingale increments gives

$$
\mathbb E|(H\mathbin\cdot M)_\infty|^2
=\sum_i\mathbb E\!\left[
H_i^2(M_{t_{i+1}}-M_{t_i})^2\right]<\infty.
$$

It is therefore an $L^2$-bounded continuous martingale.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
