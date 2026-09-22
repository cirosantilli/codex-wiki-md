<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Using the paper's full-$\ell^1$ convention, the [total variation distance](../../../../../../total-variation-distance.md) is

$$
\lVert P-Q\rVert_{\rm TV}
=\sum_{a\in A}|P(a)-Q(a)|.
$$

Let $A_+=\{a:P(a)\geq Q(a)\}$. Since the signed differences sum to zero,

$$
\lVert P-Q\rVert_{\rm TV}
=2\sum_{a\in A_+}\{P(a)-Q(a)\}
=2\{P(A_+)-Q(A_+)\}.
$$

For every $B\subseteq A$, its positive difference is at most the sum over $A_+$, and its negative difference has the same bound by taking the complement. Therefore

$$
\boxed{\lVert P-Q\rVert_{\rm TV}
=2\sup_{B\subseteq A}|P(B)-Q(B)|.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 224](../../../paper-224-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
