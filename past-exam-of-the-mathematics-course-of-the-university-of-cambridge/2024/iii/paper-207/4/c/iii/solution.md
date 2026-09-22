<h1 id="4/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $r_j=r_j^{(0)}+r_j^{(1)}$. The difference between the two [Nelson–Aalen estimator](../../../../../../../nelson-aalen-estimator.md) increments is

$$
\frac{u_j}{r_j^{(1)}}-\frac{1-u_j}{r_j^{(0)}}
=\frac{r_j}{r_j^{(0)}r_j^{(1)}}
\left(u_j-\frac{r_j^{(1)}}{r_j}\right).
$$

Therefore the [log-rank weights](../../../../../../../log-rank-weight.md)

$$
w_j=\frac{r_j^{(0)}r_j^{(1)}}{r_j^{(0)}+r_j^{(1)}}
$$

make each summand of $T_W$ equal the corresponding summand of $T_0$, and hence $T_W=T_0$.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
