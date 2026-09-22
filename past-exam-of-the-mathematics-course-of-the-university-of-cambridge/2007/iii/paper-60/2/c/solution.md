<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Set $X_j=iH_j$. The symplectic Lie condition is $X_j^TJ+JX_j=0$, equivalently $H_j^TJ+JH_j=0$. For the supplied diagonal $H_0$, the nonzero entries of $J$ pair levels $1,4$ and $2,3$; the corresponding energy sums are $-\alpha+\alpha=0$ and $-\beta+\beta=0$. Thus $H_0J+JH_0=0$ for all real $\alpha,\beta$.

For the supplied real symmetric control [matrix](../../../../../../matrix.md), direct multiplication gives

$$
H_1J=\begin{pmatrix}0&0&1&0\\0&-1&0&1\\1&0&1&0\\0&1&0&0\end{pmatrix}=-JH_1.
$$

Both generators therefore satisfy the same alternating-form condition. That condition is closed under real linear combinations, and for two such generators

$$
[X,Y]^TJ=-J[X,Y],
$$

as follows by substituting $X^TJ=-JX$ and $Y^TJ=-JY$ into $(XY)^TJ-(YX)^TJ$. Hence the whole [Dynamical Lie algebra](../../../../../../dynamical-lie-algebra.md) obeys it.

If $\dot U=X(t)U$ and $U(0)=I$, differentiating gives

$$
\frac d{dt}(U^TJU)=U^T(X^TJ+JX)U=0.
$$

Thus **every reachable propagator satisfies $U^TJU=J$**. Also $J^T=-J$, $J^\dagger J=I$, so this is a [symplectic dynamical symmetry in quantum control](../../../../../../symplectic-dynamical-symmetry-in-quantum-control.md): the generated group lies in the corresponding [compact symplectic group](../../../../../../compact-symplectic-group.md), unitarily equivalent to $Sp(2)$. It is not necessary to claim equality with $Sp(2)$, and special choices of $\alpha,\beta$ can give a smaller group.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 60](../../../paper-60-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
