<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The proof of the [linearity of a uniform pro-p group](../../../../../linearity-of-a-uniform-pro-p-group.md) has three distinct steps: pass to a finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md), integrate a faithful representation on a sufficiently small open subgroup, and extend it to the entire group. Working first on a small subgroup is essential because a faithful [Lie algebra representation](../../../../../lie-algebra-representation.md) need not send the original integral lattice into the convergence domain of the [matrix exponential](../../../../../matrix-exponential.md).

Let $G$ be a [uniform pro-p group](../../../../../uniform-pro-p-group.md) and let $L_G$ be its intrinsic [powerful Lie lattice](../../../../../powerful-lie-algebra-over-p-adic-integers.md). Then

$$
\mathfrak g=\mathbb Q_p\otimes_{\mathbb Z_p}L_G
$$

is a finite-dimensional [Lie algebra](../../../../../lie-algebra-split.md) over a [field](../../../../../field.md) of [characteristic zero](../../../../../characteristic-zero.md). The [Ado theorem](../../../../../ado-s-theorem.md), the classical Lie-theoretic ingredient in this proof, supplies a faithful finite-dimensional [Lie algebra representation](../../../../../lie-algebra-representation.md)

$$
\rho:\mathfrak g\hookrightarrow\mathfrak{gl}(V),\qquad \dim_{\mathbb Q_p}V=m<\infty.
$$

One must use a faithful representation rather than just the [Adjoint representation](../../../../../adjoint-representation-of-a-lie-algebra.md), which annihilates the [center of a Lie algebra](../../../../../center-of-a-lie-algebra.md).

Choose a [p-adic lattice](../../../../../integral-lattice-in-a-p-adic-vector-space.md) $\Lambda\subset V$. Since $L_G$ is finitely generated as a module, the entries of the representing [matrices](../../../../../matrix.md) of a module basis have bounded denominators. Hence for sufficiently large $k$,

$$
\rho(p^kL_G)\subseteq p\operatorname{End}_{\mathbb Z_p}(\Lambda).
$$

For odd $p$, the [matrix exponential](../../../../../matrix-exponential.md) and [p-adic logarithm](../../../../../p-adic-logarithm.md) converge and are inverse between $p\operatorname{End}(\Lambda)$ and $1+p\operatorname{End}(\Lambda)$. Put $H=G^{p^k}$; under the [uniform pro-p group and powerful Lie lattice correspondence](../../../../../uniform-pro-p-group-and-powerful-lie-lattice-correspondence.md) it is the BCH group on $p^kL_G$. Define

$$
\tau:H\longrightarrow\operatorname{GL}(\Lambda),\qquad
\tau(\exp_G X)=\exp(\rho(X)).
$$

Here $\exp_G$ denotes the inverse of the intrinsic logarithm identification, not an assumed matrix representation of $G$. The [Lie algebra homomorphism](../../../../../lie-algebra-homomorphism.md) $\rho$ respects the convergent [Baker--Campbell--Hausdorff formula](../../../../../baker-campbell-hausdorff-formula.md), so

$$
\exp(\rho(X*Y))=\exp(\rho(X))\exp(\rho(Y)).
$$

Thus $\tau$ is a continuous [group homomorphism](../../../../../group-homomorphism.md). If $\tau(\exp_G X)=1$, taking the [matrix logarithm](../../../../../matrix-logarithm.md) gives $\rho(X)=0$, whence $X=0$. Therefore $\tau$ is faithful and all its matrices preserve $\Lambda$. This proves linearity of the [open normal subgroup](../../../../../open-normal-subgroup.md) $H$.

To finish, use the [extension of a faithful representation from an open normal subgroup](../../../../../extension-of-a-faithful-representation-from-an-open-normal-subgroup.md). Choose representatives $t_1=1,t_2,\ldots,t_r$ of the finite left [cosets](../../../../../coset.md) $G/H$, where $r=[G:H]$. On the finite free module $W=\bigoplus_{j=1}^r\Lambda$, define the action of $g\in G$ by writing uniquely

$$
gt_j=t_i h_{ij},\qquad h_{ij}\in H,
$$

and mapping the $j$-th block to the $i$-th block by $\tau(h_{ij})$. If $g't_j=t_\ell h'$ and $gt_\ell=t_i h$, then $gg't_j=t_i hh'$; this proves the representation identity because $\tau(hh')=\tau(h)\tau(h')$. Each block matrix is invertible over $\mathbb Z_p$, and the map is continuous because the finite coset permutation is locally constant and the remaining matrix entries are obtained continuously from $\tau$.

If $g\notin H$, its permutation of $G/H$ moves the identity coset, so its block representation is not the identity. If $g\in H$ and its block representation is the identity, the block corresponding to $t_1=1$ is $\tau(g)=1$, and faithfulness of $\tau$ gives $g=1$. Thus this [induced representation](../../../../../induced-representation.md) is faithful. Choosing a basis of $W$ proves

$$
\boxed{G\hookrightarrow\operatorname{GL}_{mr}(\mathbb Z_p)}.
$$

The continuous injection is a topological embedding, since $G$ is compact and the target is Hausdorff. The trivial group is immediate. For uniform groups at $p=2$, the same proof uses the usual stronger powerfulness condition and the convergence ball $4\operatorname{End}(\Lambda)$ instead; the preceding questions concern odd $p$.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
