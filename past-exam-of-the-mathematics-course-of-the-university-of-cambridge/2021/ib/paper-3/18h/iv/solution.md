<h1 id="18h/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Under $H_0$, write the [singular value decomposition](../../../../../../singular-value-decomposition.md)

$$
X=UDV^T,\qquad D_{jj}=\sqrt{\lambda_j}.
$$

Then

$$
\widehat\beta
=VD^{-1}U^T\varepsilon.
$$

The coordinates of $U^T\varepsilon/\sigma$ are independent standard normal variables. Hence

$$
\frac{\|\widehat\beta\|^2}{\sigma^2}
\mathrel{\overset d=}
\sum_{j=1}^p\lambda_j^{-1}W_j,
\qquad
W_j\sim\chi^2_1
$$

independently. By parts (ii) and (iii),

$$
Z=\frac{n\widehat\sigma^2}{\sigma^2}\sim\chi^2_{n-p}
$$

is independent of all the $W_j$. Consequently

$$
\boxed{
T\mathrel{\overset d=}
\frac{\sum_{j=1}^p\lambda_j^{-1}W_j}{Z}
}.
$$

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
