<h1 id="9f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $M(t_1,\ldots,t_n)=\operatorname{diag}(t_1,\ldots,t_n)-A$. Expanding the [determinant](../../../../../../determinant.md) along row $i$ shows that

$$
\frac{\partial p}{\partial t_i}=C_{ii}(M),
$$

where $C_{ii}$ is the corresponding cofactor. Since a diagonal entry of the [adjugate matrix](../../../../../../adjugate-matrix.md) is that same cofactor, the multivariable [chain rule](../../../../../../chain-rule.md) along the diagonal $t_1=\cdots=t_n=t$ yields

$$
\frac d{dt}\det(tI-A)
=\sum_{i=1}^n\left.\frac{\partial p}{\partial t_i}\right|_{(t,\ldots,t)}
=\sum_{i=1}^n[\operatorname{adj}(tI-A)]_{ii}.
$$

Therefore

$$
\boxed{\frac d{dt}\det(tI-A)=\operatorname{Tr}(\operatorname{adj}(tI-A))}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [9F](../../9f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
