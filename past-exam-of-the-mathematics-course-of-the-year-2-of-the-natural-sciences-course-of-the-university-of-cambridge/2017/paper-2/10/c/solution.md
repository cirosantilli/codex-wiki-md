<h1 id="10/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $Y_p=D(Y)$. Direct [matrix multiplication](../../../../../matrix-multiplication.md) gives

$$
Y_p^2=\begin{pmatrix}1&p-p\\0&1\end{pmatrix}=I_2
$$

for every real $p$. Since $D(X)=-I_2$ commutes with all matrices and $D(Z)=-Y_p$, the remaining relations also hold:

$$
D(X)^2=D(Z)^2=I_2,\qquad D(X)D(Y)=D(Z),\qquad D(X)D(Y)D(Z)=I_2.
$$

All matrices are invertible, and the relations reproduce the [multiplication table](../../../../../multiplication-table.md) of the [Klein four-group](../../../../../klein-four-group.md). Therefore

$$
\boxed{p\in\mathbb R\text{ is arbitrary}.}
$$

A [representation](../../../../../group-representation.md) need not be an [orthogonal representation](../../../../../orthogonal-representation.md); imposing orthogonality on the displayed matrices would be an extra condition.

The [characters](../../../../../character-of-a-representation.md) are their traces, independent of $p$:

$$
\boxed{\big(\chi(I),\chi(X),\chi(Y),\chi(Z)\big)=(2,-2,0,0).}
$$

In terms of part (b), $\chi=\chi_{-+}+\chi_{--}$, so the representation is reducible. For an explicit [change of basis](../../../../../change-of-basis.md), take

$$
S=\begin{pmatrix}1&-p/2\\0&1\end{pmatrix}.
$$

Then $S^{-1}D(Y)S=\operatorname{diag}(-1,1)$ and $S^{-1}D(Z)S=\operatorname{diag}(1,-1)$, while $D(X)$ remains $-I_2$. These are the [equivalent sheared representations of the Klein four-group](../../../../../equivalent-sheared-representations-of-the-klein-four-group.md); the parameter changes the basis, not the two irreducible constituents.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [10](../../10.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
