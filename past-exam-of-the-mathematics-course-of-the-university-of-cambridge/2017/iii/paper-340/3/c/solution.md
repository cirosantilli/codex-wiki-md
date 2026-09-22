<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [Lq null space property](../../../../../../lq-null-space-property.md) established above. Fix $0\ne v\in\ker A$ and order its magnitudes $a_1\ge\cdots\ge a_N\ge0$. For a fixed exponent, the sum over the largest $s$ entries is the greatest sum over any [support of a vector](../../../../../../support-of-a-vector.md) of size at most $s$, so it suffices to verify the property for this ordered support.

If $s\ge1$, put $t=a_s$. We have $t>0$: otherwise $v$ would have fewer than $s$ nonzero entries, and applying the [Lq null space property](../../../../../../lq-null-space-property.md) to its support would assert a positive number is less than zero. For $0<p<q$, the exponent $p-q$ is negative. Thus

$$
\sum_{i=1}^sa_i^p\le t^{p-q}\sum_{i=1}^sa_i^q<t^{p-q}\sum_{i>s}a_i^q\le\sum_{i>s}a_i^p.
$$

The first inequality uses $a_i\ge t$ on the top part; the last uses $0<a_i\le t$ in the tail. Zero tail entries contribute zero without invoking a negative power of zero. Every other set of size at most $s$ has no larger top sum and no smaller complementary sum, so it too satisfies the strict $p$ inequality. The preceding equivalence proves

$$
\boxed{\text{uniform }s\text{-sparse recovery at }q\ \Longrightarrow\ \text{uniform }s\text{-sparse recovery at every }0<p<q.}
$$

This is [monotonicity of uniform sparse recovery in the exponent](../../../../../../monotonicity-of-uniform-sparse-recovery-in-the-exponent.md). If $\ker A=\{0\}$ the feasible [vector](../../../../../../vector.md) is unique regardless of the objective; if $s=0$, only the zero [vector](../../../../../../vector.md) is relevant. These cases need no threshold argument.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
