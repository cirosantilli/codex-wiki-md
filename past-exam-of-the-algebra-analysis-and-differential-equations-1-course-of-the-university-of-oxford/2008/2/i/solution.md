<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [projection](../../../../projection-linear-algebra.md) is a linear operator $E$ satisfying $E^2=E$; it need not be an orthogonal projection without an inner product. Pairwise annihilation gives

$$
P^2=\left(\sum_iE_i\right)^2=\sum_iE_i^2+\sum_{i\ne j}E_iE_j=\sum_iE_i=P.
$$

Thus their sum is a projection.

The identities $E_iP=E_i$ imply $T(I-P)=0$. Since $T$ is nonsingular, $P=I$. Also

$$
TE_i=\sum_j\lambda_jE_jE_i=\lambda_iE_i,
$$

so $\operatorname{im}E_i\subseteq V_i$. Conversely, if $Tx=\lambda_ix$, applying $E_j$ gives $(\lambda_j-\lambda_i)E_jx=0$. For $j\ne i$ the eigenvalues are distinct, hence $E_jx=0$. Since $P=I$, $x=E_ix$, proving $\operatorname{im}E_i=V_i$.

Every vector is $\sum_iE_ix$. If $\sum_iv_i=0$ with $v_i\in V_i$, applying $E_j$ gives $v_j=0$. Thus

$$
\boxed{V=V_1\oplus\cdots\oplus V_r.}
$$

These operators are the [spectral projections of a diagonalizable matrix](../../../../spectral-projection-of-a-diagonalizable-matrix.md), expressed without choosing an eigenbasis.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [2](../../2.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
