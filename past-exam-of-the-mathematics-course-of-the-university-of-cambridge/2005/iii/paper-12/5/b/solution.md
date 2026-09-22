<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use row [vectors](../../../../../../vector.md) for population counts. Given $Z_t$, [independent](../../../../../../independent-random-variables.md) reproduction has conditional [mean](../../../../../../expected-value.md) $\mathbb E[Z_{t+1}\mid Z_t]=Z_t\Lambda$. Starting from $Z_0=e_i^T$, induction gives $\mathbb E Z_t=e_i^T\Lambda^t$. Summing all child types, the expected size of generation $t$ is

$$
\boxed{\mathbb E_i|Z_t|=e_i^T\Lambda^t\mathbf1=\sum_{j=1}^l(\Lambda^t)_{ij}.}
$$

This also covers $t=0$, using $\Lambda^0=I$. All these finite-generation [expectations](../../../../../../expected-value.md) are finite because the [matrix](../../../../../../matrix.md) is finite with finite entries.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 12](../../../paper-12-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
