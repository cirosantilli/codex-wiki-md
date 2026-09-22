<h1 id="26k/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

A finite linear combination of independent [Gaussian random variables](../../../../../../../gaussian-random-variable.md) is Gaussian, so

$$
\sum_{k=1}^na_kY_k\sim N(0,v_n),
\qquad
v_n=\sum_{k=1}^na_k^2.
$$

Since $v_n\to v:=\sum_{k\geq1}a_k^2<\infty$, the [characteristic functions](../../../../../../../characteristic-function.md) converge pointwise:

$$
\exp\left(-\frac12v_nt^2\right)\longrightarrow\exp\left(-\frac12vt^2\right).
$$

The [Lévy continuity theorem](../../../../../../../levy-continuity-theorem.md) yields convergence in distribution to

$$
\boxed{N\left(0,\sum_{k\geq1}a_k^2\right)}.
$$

On the given common probability space, the same variance calculation actually proves convergence in $L^2$ as well.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [26K](../../../26k.md)
4. [Paper 4](../../../../paper-4-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
