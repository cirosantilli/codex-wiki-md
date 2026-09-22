<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A rate-$R$ block code consists of an encoder $E_n:J^n\to\{1,\ldots,M_n\}$ and decoder $D_n$, with $M_n\leq2^{nR}$; it is reliable when $\Pr[D_n(E_n(U^n))\ne U^n]\to0$. Choose $\varepsilon>0$ with $H(U)+\varepsilon<R$. The [typical set](../../../../../../typical-set.md) has probability tending to one and cardinality at most $2^{n(H(U)+\varepsilon)}\leq2^{nR}$. Encode its words injectively and map every atypical word to a default codeword. The error probability is at most the atypical probability, so reliable compression exists.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 323](../../../paper-323-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
