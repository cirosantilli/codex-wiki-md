<h1 id="12k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [linear-feedback shift register](../../../../../../linear-feedback-shift-register.md) is a linear map

$$
M(x_1,\ldots,x_d)=(x_2,\ldots,x_d,\sum_ia_ix_i).
$$

For the stated matrix $H$, a word $c=(c_0,\ldots,c_{k-1})$ lies in $C$ exactly when $\sum_jc_jM^jx=0$. If $\sigma c$ is its cyclic shift, periodicity $M^kx=x$ gives

$$
H(\sigma c)=M(Hc)=0.
$$

**Thus $\ker H$ is shift-invariant and is a binary cyclic code.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12K](../../12k.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
