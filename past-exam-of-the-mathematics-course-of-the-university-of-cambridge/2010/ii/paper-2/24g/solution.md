<h1 id="24g/solution">Solution</h1>

↑ **Parent:** [24G](../24g.md)

We use algebraic dimension and tangent spaces, equivalently after extending scalars to an algebraic closure; these are not dimensions of the finite set of rational points when $k$ is finite. The condition rank at most $r$ is equivalent to the vanishing of all $(r+1)\times(r+1)$ [matrix minors](../../../../../minor-linear-algebra.md). These are [polynomials](../../../../../polynomial-split.md) in the $nm$ entries, so define an affine [determinantal variety](../../../../../determinantal-variety.md) $X^{n,m,r}$. The same equations make it a [Zariski closed](../../../../../zariski-closed-set.md) subset of $X^{n,m,r+1}$.

For $1\leq r<\min(n,m)$, every line $tE_{ij}$ lies in $X$ because its matrices have rank at most one. Its tangent direction $E_{ij}$ therefore belongs to the [Zariski tangent space](../../../../../zariski-tangent-space.md) at zero. The matrix units span all $nm$ directions, so $T_0X=k^{nm}$. Meanwhile a rank-$r$ chart with an invertible $r\times r$ block has the form

$$
\begin{pmatrix}B&C\\D&DB^{-1}C\end{pmatrix}.
$$

The free blocks have $r^2+r(m-r)+(n-r)r=r(n+m-r)$ entries. Rank-$r$ matrices are dense in $X$: the factorization $UV$ parametrizes all rank-at-most-$r$ matrices, and the full-rank factor pairs form a dense open subset. This also proves irreducibility, so the local dimension at zero equals the dimension of $X$. Since $r(n+m-r)<nm$, **zero is singular when $1\leq r<\min(n,m)$.**

There is a necessary qualification to the printed claim: for $r=0$, $X=\{0\}$ is a smooth point, with zero-dimensional tangent space. Thus the claim is false if zero is allowed as a rank bound.

Finally, for $n=5,m=2,r=1$, the formula gives **$\boxed{\dim X^{5,2,1}=6}$.** Concretely, on a chart where an entry of the first column is nonzero, choose that column freely and make the second an arbitrary scalar multiple of it, giving five plus one parameters.

## ↑ Ancestors (10)

1. [24G](../24g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
