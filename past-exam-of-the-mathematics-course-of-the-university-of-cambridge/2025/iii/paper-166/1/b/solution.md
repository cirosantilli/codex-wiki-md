<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\Lambda=n\log2-m\log3$. It is nonzero by [unique prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md). If $3^m\leq2^{n-1}$ or $3^m\geq2^{n+1}$, the claimed inequality follows immediately after increasing the effective constant. We may therefore assume

$$
2^{n-1}<3^m<2^{n+1},
$$

which implies $m\asymp n$.

The [Baker lower bound for a homogeneous linear form in logarithms](../../../../../../baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms.md), with the fixed algebraic numbers $2$ and $3$, gives

$$
|\Lambda|\geq n^{-C_0}
$$

for an effective absolute constant $C_0$. If $|\Lambda|>1$, the desired conclusion is again immediate. Otherwise, the [mean value theorem](../../../../../../mean-value-theorem.md) applied to the [exponential function](../../../../../../exponential-function.md) on $[-1,1]$ gives $|e^u-1|\geq c|u|$. Hence

$$
|2^n-3^m|
=3^m|e^\Lambda-1|
\geq c3^m|\Lambda|
\geq c2^{n-1}n^{-C_0}.
$$

Absorbing the fixed factor into a larger exponent proves $|2^n-3^m|\geq2^n/n^C$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
