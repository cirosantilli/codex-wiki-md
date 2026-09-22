<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write

$$
P(z)=\prod_{\substack{p\in\mathbb P\\p\leq z}}p.
$$

The [sifting function](../../../../../../sifting-function.md) is

$$
S(A,\mathbb P,z)=|\{a\in A:\gcd(a,P(z))=1\}|.
$$

For each integer $a$, [Möbius inversion](../../../../../../mobius-inversion-formula.md) in its divisor-indicator form gives

$$
\mathbf1_{\gcd(a,P(z))=1}
=\sum_{d\mid\gcd(a,P(z))}\mu(d)
=\sum_{\substack{d\mid P(z)\\d\mid a}}\mu(d).
$$

Summing over the finite set $A$ and interchanging the finite sums yields

$$
S(A,\mathbb P,z)
=\sum_{d\mid P(z)}\mu(d)|\{a\in A:a\equiv0\pmod d\}|.
$$

This is the inclusion-exclusion formula encoded by the [Möbius function](../../../../../../mobius-function.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 150](../../../paper-150-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
