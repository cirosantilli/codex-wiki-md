<h1 id="18g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Give $V_n$ the action $(g\cdot P)(x,y)=P((x,y)g)$, where $(x,y)$ is a row vector. Substitution preserves homogeneous degree, and composition agrees with [matrix multiplication](../../../../../../matrix-multiplication.md), so this is a [complex representation](../../../../../../complex-representation.md) of [SU(2) group](../../../../../../su-2-group.md). The diagonal [torus](../../../../../../torus.md) $\operatorname{diag}(z,z^{-1})$ acts on $x^{n-j}y^j$ with weight $z^{n-2j}$; these weights are distinct.

A nonzero [invariant subspace](../../../../../../invariant-subspace.md) is invariant under the [torus](../../../../../../torus.md), so finite-dimensional Fourier projection onto its [weight spaces](../../../../../../weight-space.md) supplies a nonzero [monomial](../../../../../../monomial.md). Differentiating the [group action](../../../../../../group-action.md) and complexifying supplies the operators $E=x\partial_y$ and $F=y\partial_x$. Their repeated application moves between every successive [monomial](../../../../../../monomial.md), with nonzero coefficients until an endpoint is reached:

$$
E(x^{n-j}y^j)=j x^{n-j+1}y^{j-1},\qquad
F(x^{n-j}y^j)=(n-j)x^{n-j-1}y^{j+1}.
$$

The [invariant subspace](../../../../../../invariant-subspace.md) therefore contains the whole [monomial basis](../../../../../../monomial-basis.md). Thus

$$
\boxed{V_n\text{ is irreducible and }\dim V_n=n+1.}
$$

For $n=0$ this is the one-dimensional [trivial representation](../../../../../../trivial-representation.md). [Torus](../../../../../../torus.md) weight projections are legitimate because an invariant complex subspace is closed in finite dimension.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [18G](../../18g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
