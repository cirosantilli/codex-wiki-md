<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Writing the [Brauer character inner product](../../../../../../brauer-character-inner-product.md) as a sum over conjugacy-class representatives gives

$$
\langle\chi_{P_i},\chi_{S_j}\rangle
=\sum_r\frac{
\overline{\chi_{P_i}(x_r)}\chi_{S_j}(x_r)}
{|C_G(x_r)|}.
$$

Thus the duality from part (c) is exactly

$$
\boxed{\overline\Pi D X^T=I.}
$$

All three matrices are square. Reversing the two inverse factors gives $DX^T\overline\Pi=I$, hence

$$
X^T\overline\Pi=D^{-1}.
$$

Taking complex conjugates yields

$$
\boxed{\overline X^{,T}\Pi=D^{-1}
=\operatorname{diag}(|C_G(x_1)|,\ldots,|C_G(x_n)|).}
$$

The $(g,h)$ entry is $\sum_S\overline{\chi_S(g)}\chi_{P_S}(h)$, and $\overline{\chi_S(g)}=\chi_S(g^{-1})$. Therefore [Column orthogonality for Brauer characters](../../../../../../column-orthogonality-for-brauer-characters.md) gives

$$
\boxed{
\sum_S\chi_S(g^{-1})\chi_{P_S}(h)
=\begin{cases}
|C_G(g)|,&g\text{ and }h\text{ are conjugate},\\
0,&\text{otherwise}.
\end{cases}}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 138](../../../paper-138-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
