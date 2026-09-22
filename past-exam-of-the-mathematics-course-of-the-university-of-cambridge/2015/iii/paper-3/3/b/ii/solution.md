<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We first record why [rigid quiver representations have open orbits](../../../../../../../rigid-quiver-representations-have-open-orbits.md). Let $\mathbf n=\dim X$, $G=\prod_i\operatorname{GL}(X_i)$ and $R=\operatorname{Rep}_Q(\mathbf n)$. The stabilizer is $\operatorname{Aut}_Q(X)$, the nonempty open set of units in $\operatorname{End}_Q(X)$, so it has dimension $\dim\operatorname{End}_Q(X)$. The [dimension formula for an algebraic group homomorphism](../../../../../../../dimension-formula-for-an-algebraic-group-homomorphism.md), or the same constant-fiber argument for the orbit map, gives

$$
\dim\mathcal O_X=\sum_i n_i^2-\dim\operatorname{End}_Q(X).
$$

By the [Ringel form](../../../../../../../ringel-form.md) identity and $\operatorname{Ext}^1_Q(X,X)=0$, this equals $\sum_\sigma n_{s(\sigma)}n_{t(\sigma)}=\dim R$. An algebraic-group orbit is locally closed; since $R$ is an irreducible [affine space](../../../../../../../affine-space.md), this full-dimensional orbit is open and dense.

Write $q=\rho\pi$ for the composed path. Each matrix entry of $q$ is a polynomial function on $R$. Since $qX=0$, change of basis makes it zero on all of $\mathcal O_X$, hence on all of $R$ by density. Suppose instead that $X_{t(\rho)}\ne0$. The condition $\pi X\ne0$ ensures that every vertex space visited by $\pi$ is nonzero. Choose a vector $v_a\ne0$ and a functional $\ell_a$ with $\ell_a(v_a)=1$ at every vertex visited by $q$. Assign to every arrow $\sigma$ occurring in $q$ the map $v_{t(\sigma)}\ell_{s(\sigma)}$, and assign arbitrary maps, say zero, to the other arrows. At this representation, the path $q$ carries its initial chosen vector to its final chosen vector, so $q$ is nonzero, a contradiction.

The construction uses a single assigned map per arrow, so it still works if an arrow or vertex occurs repeatedly in the path. Therefore

$$
\boxed{X_{t(\rho)}=0.}
$$

This proves the [path identities in a rigid quiver representation](../../../../../../../path-identities-in-a-rigid-quiver-representation.md) claim for an arbitrary [quiver](../../../../../../../quiver.md). Maximal rank of the individual arrows alone would not justify the conclusion about their composition.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Iii](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
