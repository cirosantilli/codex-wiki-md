<h1 id="19f/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $m=[G:H]$, extend $\psi$ to $\psi_0$ by zero outside $H$, and choose [coset](../../../../../../coset.md) representatives $x_1,\ldots,x_m$. Then $\operatorname{Ind}\psi(g)=\sum_{j=1}^m f_j(g)$ with $f_j(g)=\psi_0(x_j^{-1}gx_j)$. Each summand has squared $G$-norm

$$
\|f_j\|_G^2=\frac1{|G|}\sum_{h\in H}|\psi(h)|^2=\frac1m,
$$

since $\psi$ is irreducible. Pointwise [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $|\sum f_j|^2\le m\sum|f_j|^2$. After summing and dividing by $|G|$,

$$
\boxed{\sum_i e_i^2=\|\operatorname{Ind}\psi\|_G^2\le m\sum_j\|f_j\|_G^2=m.}
$$

The $e_i$ are nonnegative integers by part (b). This proves the [character induction norm bound](../../../../../../character-induction-norm-bound.md) without an assumption that $H$ is normal.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [19F](../../19f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
