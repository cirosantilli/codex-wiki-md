<h1 id="4h/solution">Solution</h1>

↑ **Parent:** [4H](../4h.md)

A binary [uniquely decodable code](../../../../../decipherable-code.md) assigns a finite binary word to each source symbol, so that no two distinct finite sequences of source symbols have the same concatenated encoding. This does not require the stronger prefix property. All codeword lengths are positive.

Put $S=\sum_j2^{-l_j}$ and let $A_{k,L}$ count sequences of $k$ source symbols whose encoded total length is $L$. Expanding the product gives

$$
S^k=\sum_{L=kl_{\min}}^{kl_{\max}}A_{k,L}2^{-L}.
$$

Unique decodability makes these encodings distinct, so $A_{k,L}\leq2^L$, the number of binary strings of that length. There are at most $k(l_{\max}-l_{\min})+1$ possible lengths. Therefore

$$
S^k\leq k(l_{\max}-l_{\min})+1.
$$

Taking $k$th roots and letting $k\to\infty$ proves the [McMillan inequality](../../../../../mcmillan-inequality.md):

$$
\boxed{\sum_j2^{-l_j}\leq1.}
$$

## ↑ Ancestors (10)

1. [4H](../4h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
