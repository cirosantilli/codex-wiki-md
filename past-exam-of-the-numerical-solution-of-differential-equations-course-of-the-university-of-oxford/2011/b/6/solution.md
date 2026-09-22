<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Let $x_*=A^{-1}b$, $e_k=x_k-x_*$ and $G=M^{-1}N$. Subtract the exact fixed-point equation to obtain $e_k=G^ke_0$. Hence convergence for every initial vector is equivalent to $G^k\to0$. If this holds, it holds after complexification; applying it to a complex [eigenvector](../../../../eigenvector.md) gives $\lambda^kv\to0$, so $|\lambda|<1$. Conversely, the complex [Jordan normal form](../../../../jordan-normal-form.md) expresses each power as a finite sum of terms $\binom{k}{r}\lambda^{k-r}$ from its blocks. Every term tends to zero when all [eigenvalues](../../../../eigenvalue.md) have modulus below one. Thus

$$
\boxed{\text{Convergence for every starting vector}\iff\rho(G)<1.}
$$

The [convergence criterion for a stationary iteration](../../../../convergence-criterion-for-a-stationary-iteration.md) needs complex triangularization or [Jordan normal form](../../../../jordan-normal-form.md). The paper's assertion that every real matrix is similar to a real upper-triangular matrix is false when nonreal [eigenvalues](../../../../eigenvalue.md) occur; complex triangularization supplies the intended argument. In the [Gauss-Seidel method](../../../../gauss-seidel-method.md), with $A=D+L+U$ split into diagonal, strictly lower and strictly upper parts, $\boxed{M=D+L,\ N=-U}$.

For $n\geq4$, eliminating the ghost values gives the symmetric pentadiagonal [matrix](../../../../matrix.md)

$$
\boxed{A=\begin{pmatrix}
7&-4&1&0&\cdots\\
-4&6&-4&1&\cdots\\
1&-4&6&-4&\ddots\\
0&1&-4&6&\ddots\\
\vdots&\vdots&\ddots&\ddots&\ddots
\end{pmatrix},\quad A_{nn}=7,\ A_{jj}=6\ (2\leq j\leq n-1),\quad A_{j,j+1}=-4,\quad A_{j,j+2}=1.}
$$

All other off-diagonal entries vanish. The first two equations are

$$
7U_1-4U_2+U_3=h^4f_1,\qquad
-4U_1+6U_2-4U_3+U_4=h^4f_2,
$$

and the last two are

$$
U_{n-3}-4U_{n-2}+6U_{n-1}-4U_n=h^4f_{n-1},\qquad
U_{n-2}-4U_{n-1}+7U_n=h^4f_n.
$$

For $n=3$ the matrix is $\begin{pmatrix}7&-4&1\\-4&6&-4\\1&-4&7\end{pmatrix}$, for $n=2$ it is $\begin{pmatrix}7&-4\\-4&7\end{pmatrix}$, and for $n=1$ it is $(8)$ because both ghost contributions meet the same unknown. The diagonal entries are positive in every case, so the lower triangular [matrix](../../../../matrix.md) $D+L$ is invertible and the [Gauss-Seidel iteration](../../../../gauss-seidel-method.md) is well defined.

An [eigenvalue](../../../../eigenvalue.md) $\lambda$ of $G=-(D+L)^{-1}U$ makes $H(\lambda)=\lambda(D+L)+U$ singular. Let $\ell_i$ and $r_i$ be the sums of absolute lower and upper entries in row $i$. The row's diagonal-dominance margin is

$$
|\lambda|d_i-|\lambda|\ell_i-r_i.
$$

Interior full rows have $d_i=6$, $\ell_i=r_i=5$, giving margin $|\lambda|-5$. Boundary rows have larger margins; for instance the first gives $7|\lambda|-5$, and the second gives at least $2|\lambda|-5$. Therefore $|\lambda|>5$ would make $H(\lambda)$ a [strictly diagonally dominant matrix](../../../../strictly-diagonally-dominant-matrix.md), hence nonsingular, a contradiction.

At $|\lambda|=5$ it is weakly diagonally dominant with strict boundary rows. Its nonzero nearest-neighbour entries make it an [irreducibly diagonally dominant matrix](../../../../irreducibly-diagonally-dominant-matrix.md). The nonsingularity theorem for that class again contradicts singularity. For the small matrices above all rows are already strict at this value. Hence

$$
\boxed{\text{Every iteration eigenvalue has }|\lambda|<5;\text{ equality is impossible}.}
$$

There is also a stronger conclusion. For $T=\operatorname{tridiag}(-1,2,-1)$,

$$
A=T^2+2e_1e_1^T+2e_ne_n^T,
$$

including the $n=1$ overlap. Since $T$ is positive definite, $A$ is a [symmetric positive-definite matrix](../../../../symmetric-positive-definite-matrix.md). The [Gauss-Seidel convergence from diagonal dominance and positive definiteness](../../../../gauss-seidel-convergence-from-diagonal-dominance-and-positive-definiteness.md) theorem consequently gives the stronger bound $\rho(G)<1$.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the numerical solution of differential equations course of the University of Oxford](../../../split.md)
5. [Numerical solution of differential equations course of the University of Oxford](../../../../numerical-solution-of-differential-equations-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
