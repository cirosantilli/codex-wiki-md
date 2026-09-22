<h1 id="4/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $d=\deg f$ and let $f_d$ be the nonzero highest homogeneous part. Choose one coordinate, after a permutation, such that

$$
f_d(X_1,\ldots,X_{n-1},1)
$$

is not the zero polynomial. A polynomial of degree at most $d$ in each variable cannot vanish on the entire grid $\{0,1,\ldots,d\}^{n-1}$, by induction on the number of variables. Hence there are $a_i\in\{0,1,\ldots,d\}$ such that

$$
f_d(a_1,\ldots,a_{n-1},1)\ne0.
$$

Set

$$
y_i=t_i-a_it_n\quad(1\leq i<n),
\qquad y_n=t_n.
$$

This is given, up to the initial coordinate permutation, by an integer matrix $M$ with determinant $\pm1$ and

$$
\max_{i,j}|M_{ij}|\leq d.
$$

In the inverse coordinates $t_i=y_i+a_iy_n$, the coefficient of $y_n^d$ in $f$ is the nonzero real number $f_d(a_1,\ldots,a_{n-1},1)$. Dividing by it makes the defining equation monic in $y_n$. Thus $A$ is integral over $\mathbb R[y_1,\ldots,y_{n-1}]$ by [linear Noether normalization for a hypersurface](../../../../../../../linear-noether-normalization-for-a-hypersurface.md). The [Lying-over theorem](../../../../../../../lying-over-theorem.md) now makes

$$
\operatorname{Spec}A\longrightarrow
\operatorname{Spec}\mathbb R[y_1,\ldots,y_{n-1}]
$$

surjective.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [4](../../../4.md)
4. [Paper 101](../../../../paper-101-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
