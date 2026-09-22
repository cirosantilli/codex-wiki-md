<h1 id="31j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $Z=(X,Y)$ be an independent test example and write $Z_i=(X_i,Y_i)$. Exchangeability of $Z$ and $Z_i$ gives

$$
\mathbb E\,\ell(H_D,Z)
=\frac1n\sum_{i=1}^n
\mathbb E\,\ell(H_{D_i(Z)},Z_i).
$$

The datasets $D_i(Z)$ and $D$ differ in one coordinate, so stability gives

$$
\mathbb E\,\ell(H_{D_i(Z)},Z_i)
\leq\mathbb E\,\ell(H_D,Z_i)+\beta.
$$

Averaging over $i$ and subtracting the empirical loss proves

$$
\boxed{\mathbb EF(D)\leq\beta}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [31J](../../31j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
