<h1 id="12j/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Suppose a zero-register machine decided $L=\{a^nb^n:n>0\}$, and choose $k\ne\ell$ as in part (d). Take $m\geq\max\{k,\ell\}$ and set

$$
x=a^mb^{m-k}.
$$

Then

$$
xb^k=a^mb^m\in L,
$$

whereas

$$
xb^\ell=a^mb^{m-k+\ell}\notin L.
$$

Part (d) puts both computations into the identical configuration $(q,x)$. Determinism forces their subsequent computations and outputs to agree, a contradiction. Therefore

$$
\boxed{L\text{ is not $0$-computable}}.
$$

This is the [one-register separation for equal block lengths](../../../../../../one-register-separation-for-equal-block-lengths.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [12J](../../12j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
