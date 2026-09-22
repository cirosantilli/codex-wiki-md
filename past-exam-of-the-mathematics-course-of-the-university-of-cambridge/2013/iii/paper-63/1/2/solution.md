<h1 id="1/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The zero [Dirichlet boundary conditions](../../../../../../dirichlet-boundary-condition.md) permit an exact finite-interval calculation. Let $T=\operatorname{tridiag}(1,-2,1)$ on the $M$ interior grid points. The [Dirichlet discrete Laplacian](../../../../../../dirichlet-discrete-laplacian.md) has an orthogonal [eigenvector](../../../../../../eigenvector.md) basis

$$
v_m^{(j)}=\sin\frac{jm\pi}{M+1},\qquad
Tv^{(j)}=-4s_jv^{(j)},\qquad
s_j=\sin^2\frac{j\pi}{2(M+1)},\quad 1\leq j\leq M.
$$

Consequently the update matrix $G=(I-rT)^{-1}$ has modal amplification factors

$$
g_j=\frac1{1+4rs_j}.
$$

For every physical $r\geq0$, all denominators are at least one. [Orthogonal diagonalization](../../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md) therefore proves

$$
\|G^nU^0\|_d\leq\|U^0\|_d,\qquad
\|U\|_d^2=d\sum_{m=1}^M|U_m|^2,
$$

uniformly in $M$, $r$ and $n$. The same bound controls initial perturbations; a forcing increment is propagated by contraction, so successive increments accumulate at most by their sum. **The highest-order consistent method is unconditionally stable for all $r\geq0$.** This proof incorporates the boundary conditions, whereas a periodic [Fourier mode](../../../../../../fourier-mode.md) calculation alone would not do so.

For completeness, if “range” is interpreted algebraically to include negative $r$ on a fixed grid, the exact power-stable range is

$$
\boxed{r\in[0,\infty)\ \cup\ \left(-\infty,-\frac1{2\sin^2(\pi/[2(M+1)])}\right].}
$$

Indeed, for $r<0$ every denominator is less than one, so $|g_j|\leq1$ requires $1+4rs_j\leq-1$ for every $j$. The strongest restriction comes from $s_1$. Equality gives a simple amplification factor $-1$ and is allowed because the update is orthogonally diagonalizable. Other negative values either amplify a mode or make the update singular. This extra branch describes backward time stepping on a fixed spatial grid; it is not a positive-time diffusion discretization, and no fixed negative $r$ remains in that branch as $M\to\infty$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [1](../../1.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
