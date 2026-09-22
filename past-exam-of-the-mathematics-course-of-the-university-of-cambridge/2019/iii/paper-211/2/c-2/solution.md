<h1 id="2/c-2/solution">Solution</h1>

↑ **Parent:** [C](../c-2.md)

Condition on $S$ and use the characteristic function of a [standard normal distribution](../../../../../../standard-normal-distribution.md):

$$
\mathbb E_Z[S^{iZ}\mid S]
=\mathbb E_Z[e^{iZ\log S}]
=e^{-(\log S)^2/2}
=G(S).
$$

The integrand has modulus one, so [Fubini's theorem](../../../../../../fubini-s-theorem.md) is immediate. Taking expectation over $S$ yields

$$
\boxed{\mathbb E[G(S)]=\mathbb E[M(iZ)].}
$$

## ↑ Ancestors (11)

1. [C](../c-2.md)
2. [2](../../2.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
