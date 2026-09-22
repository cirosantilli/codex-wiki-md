<h1 id="19g/solution">Solution</h1>

↑ **Parent:** [19G](../19g.md)

For $\ell\in V^*$ define $(g\ell)(v)=\ell(g^{-1}v)$. The representing matrix is the transpose of the inverse matrix on $V$, so the dual [character](../../../../../character-of-a-representation.md) is

$$
\boxed{\beta(g)=\alpha(g^{-1})=\overline{\alpha(g)}.}
$$

The last equality follows by averaging a [Hermitian inner product](../../../../../hermitian-form.md) to make the finite-group [group representation](../../../../../group-representation.md) unitary. Complex finite-group representations are isomorphic exactly when their [characters](../../../../../character-of-a-representation.md) agree. Hence $V$ is self-dual exactly when its [character](../../../../../character-of-a-representation.md) is real-valued.

The invariant tensor identification $(V\otimes V)^G\simeq\operatorname{Hom}_G(V^*,V)$ and [Schur lemma](../../../../../schur-s-lemma.md) show that, for irreducible $V$, the trivial multiplicity is zero unless $V^*\simeq V$, and one in that case. Dually, a self-duality isomorphism gives a nonzero invariant [bilinear form](../../../../../bilinear-form.md) $B$ on $V$. Its radical is an invariant subspace, so irreducibility makes $B$ nondegenerate. The space of invariant [bilinear forms](../../../../../bilinear-form.md) is one dimensional. Since the transpose $B^T$ is another such form, $B^T=cB$; transposing again gives $c^2=1$. Therefore $B$ is symmetric or alternating: in the negative-transpose case, $B(v,v)=-B(v,v)$ forces $B(v,v)=0$. Both types cannot coexist, since proportional nonzero forms cannot have both transpose signs.

In odd dimension an alternating matrix has [determinant](../../../../../determinant.md) zero: $\det B=\det(-B^T)=(-1)^n\det B=-\det B$. Thus only the symmetric case is possible. Over $\mathbb C$ a nondegenerate [symmetric bilinear form](../../../../../symmetric-bilinear-form.md) has a [basis](../../../../../basis.md) with matrix $I$: diagonalize it by congruence and rescale each nonzero diagonal entry. In that [basis](../../../../../basis.md) invariance says $\rho(g)^T\rho(g)=I$. Consequently

$$
\boxed{\rho(G)\text{ is conjugate to a subgroup of }O(n,\mathbb C)\quad(n\text{ odd, irreducible self-dual}).}
$$

## ↑ Ancestors (10)

1. [19G](../19g.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
