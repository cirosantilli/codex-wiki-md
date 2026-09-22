<h1 id="38c/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a linear system write $A=D+R$, where $D$ is the diagonal. The [Jacobi method](../../../../../../jacobi-method.md) iterates

$$
u^{(k+1)}=D^{-1}(b-Ru^{(k)}),\qquad e^{(k+1)}=Be^{(k)},\quad B=-D^{-1}R.
$$

Here $D=(10/3)I$, and $B$ has nonnegative off-diagonal entries with row sums at most one. Rows adjacent to the boundary have sum strictly less than one; those at purely interior stencil vertices have sum one. Thus $\|B\|_\infty\leq1$.

To prove strict [spectral radius](../../../../../../spectral-radius.md) below one, suppose $Bv=\zeta v$ with $|\zeta|=1$, and choose an index with $|v_i|=\|v\|_\infty>0$. In

$$
|v_i|=|\zeta v_i|\leq\sum_jB_{ij}|v_j|\leq\left(\sum_jB_{ij}\right)\|v\|_\infty\leq\|v\|_\infty,
$$

equality forces that row sum to equal one and every linked neighbor to attain the same maximum modulus. Propagate this along the connected axial grid to a boundary-adjacent row, whose row sum is strictly less than one, a contradiction. All [eigenvalues](../../../../../../eigenvalue.md) therefore have modulus strictly below one. Hence $B^k\to0$ and the Jacobi errors tend to zero from every initial vector. The unique solution exists by positive definiteness, so $\boxed{\text{Jacobi converges for this discretization in any ordering}.}$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [38C](../../38c.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
