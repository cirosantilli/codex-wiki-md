<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B$ be the matrix whose $i$th column consists of the coordinates of $\beta_i$ in the basis $(e_j)$. Define the upper-triangular matrix $U$ and lower-triangular matrix $L$ by

$$
U_{ij}=
\begin{cases}
1,&i=j,\\
-a_{ij},&i<j,\\
0,&i>j,
\end{cases}
\qquad
L_{ij}=
\begin{cases}
1+a_{ii}=-1,&i=j,\\
a_{ij},&i>j,\\
0,&i<j.
\end{cases}
$$

The first identity in part b says $I=BU$, so $B=U^{-1}$. The second says that the matrix $C$ of $\sigma(c)$ is $C=BL=U^{-1}L$. Since $U$ has diagonal entries one, $\det U=1$, and therefore

$$
\det(tI-C)
=\det\bigl(U^{-1}(tU-L)\bigr)
=\det(tU-L).
$$

**Thus $\det(tU-L)$ is the [characteristic polynomial](../../../../../../characteristic-polynomial.md) of the [Coxeter element](../../../../../../coxeter-element.md) in its geometric representation.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 111](../../../paper-111-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
