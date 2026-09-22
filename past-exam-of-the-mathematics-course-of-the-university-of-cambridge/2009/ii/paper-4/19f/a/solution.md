<h1 id="19f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [restriction of a representation](../../../../../../restriction-of-a-representation.md) $\rho:G\to\operatorname{GL}(V)$ to $H$ is the same [vector space](../../../../../../vector-space-split.md) and operators with the domain limited to $H$; its [character](../../../../../../character-of-a-representation.md) is $\chi_H(h)=\chi(h)$. Averaging a positive Hermitian [inner product](../../../../../../inner-product.md) over $H$ makes it invariant, so invariant subspaces have invariant orthogonal complements. Repeating gives a direct sum of irreducible $H$-spaces and hence $\chi_H=\sum_i d_i\psi_i$ with nonnegative integer multiplicities.

By [character inner product](../../../../../../character-inner-product.md) [orthogonality](../../../../../../orthogonal-vectors.md),

$$
\sum_i d_i^2=\langle\chi_H,\chi_H\rangle_H
=\frac1{|H|}\sum_{h\in H}|\chi(h)|^2
\le\frac1{|H|}\sum_{g\in G}|\chi(g)|^2=\boxed{[G:H]},
$$

since $\chi$ is irreducible and has normalized squared [norm](../../../../../../norm.md) one on $G$. Equality holds precisely when the omitted nonnegative terms vanish, namely $\boxed{\chi(g)=0\text{ for every }g\notin H}$. This is the [restriction multiplicity bound](../../../../../../restriction-multiplicity-bound.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [19F](../../19f.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
