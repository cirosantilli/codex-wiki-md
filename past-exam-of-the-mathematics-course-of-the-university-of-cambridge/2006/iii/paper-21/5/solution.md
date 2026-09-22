<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a real or [complex vector bundle](../../../../../complex-vector-bundle.md) $E$, choose a fiber metric. Its [Thom space](../../../../../thom-space.md) is the pointed quotient

$$
\operatorname{Th}(E)=D(E)/S(E),
$$

collapsing the [sphere bundle](../../../../../sphere-bundle.md) to one basepoint. When the base is compact, this is the [one-point compactification](../../../../../alexandroff-extension.md) of the total space: fiberwise radial compression identifies the total space with the interior of $D(E)$, and all directions approaching its boundary become the single point at infinity.

Decompose $\mathbb C^{n+m+2}=V\oplus W$ with $V=\mathbb C^{n+1}$, $W=\mathbb C^{m+1}$, so the subspace being collapsed is $\mathbb P(V)=\mathbb{CP}^n$. Every line outside it has a representative $(v,w)$ with $w\ne0$. Its projection to $W$ gives the line $\ell=\mathbb Cw\in\mathbb P(W)=\mathbb{CP}^m$, and there is a unique complex-linear map $A:\ell\to V$ such that $A(w)=v$. The line in $V\oplus W$ is precisely the graph of $A$. This construction is unaffected by replacing $(v,w)$ with $(\lambda v,\lambda w)$.

Let $\gamma=\eta_1$ be the tautological line over $\mathbb P(W)$. The graph construction and its inverse are continuous, indeed smooth in the usual affine charts, and identify

$$
\mathbb{CP}^{n+m+1}\setminus\mathbb{CP}^{n}
\cong\operatorname{Tot}\bigl(\operatorname{Hom}_{\mathbb C}(\gamma,V)\bigr)
=\operatorname{Tot}\bigl((\gamma^*)^{\oplus(n+1)}\bigr).
$$

A [Hermitian metric](../../../../../hermitian-metric-on-a-holomorphic-vector-bundle.md) gives a complex-linear bundle isomorphism $\bar\gamma\cong\gamma^*$. With the Hermitian form linear in its first argument, it sends $\bar v$ to the functional $w\mapsto\langle w,v\rangle$. Linearity in the conjugate vector is exactly what makes this a complex, rather than merely real, isomorphism. Thus the bundle is $(\bar\eta_1)^{\oplus(n+1)}$, with the conjugation bars present in the original PDF.

Collapsing the closed subspace $\mathbb{CP}^n$ in [compact Hausdorff space](../../../../../compact-hausdorff-space.md) $\mathbb{CP}^{n+m+1}$ gives the [one-point compactification](../../../../../alexandroff-extension.md) of its open complement: neighborhoods of the collapsed point have compact complements, and conversely every compact subset of the complement is closed in the ambient space. The graph [homeomorphism](../../../../../homeomorphism.md) therefore extends over the added point. This proves the [projective-space quotient as a Thom space of conjugate tautological lines](../../../../../projective-space-quotient-as-a-thom-space-of-conjugate-tautological-lines.md):

$$
\boxed{\mathbb{CP}^{n+m+1}/\mathbb{CP}^{n}
\cong\operatorname{Th}\bigl((\bar\eta_1)^{\oplus(n+1)}
\longrightarrow\mathbb{CP}^{m}\bigr).}
$$

The graph coordinates also determine the normal [complex structures](../../../../../complex-structure.md) requested in the second part. The copy $\mathbb P(W)$ corresponds to the [zero section](../../../../../zero-section-of-a-vector-bundle.md) of the graph bundle, whose [normal bundle](../../../../../normal-bundle.md) is that bundle itself. For a coordinate embedding $\mathbb{CP}^k\subset\mathbb{CP}^n$, use $W=\mathbb C^{k+1}$ and its complementary coordinate space $V=\mathbb C^{n-k}$. Then the [normal bundle of a linear complex-projective embedding](../../../../../normal-bundle-of-a-linear-complex-projective-embedding.md) is

$$
\boxed{\nu_k=\operatorname{Hom}_{\mathbb C}(\gamma_k,\mathbb C^{n-k})
\cong(\gamma_k^*)^{\oplus(n-k)}
\cong\bar\gamma_k^{\oplus(n-k)}.}
$$

The [complex structure](../../../../../complex-structure.md) is the linear structure in these graph coordinates. Equivalently, applying the preceding [homeomorphism](../../../../../homeomorphism.md) with its parameters $n-k-1$ and $k$ identifies the [Thom space](../../../../../thom-space.md) of this [normal bundle](../../../../../normal-bundle.md) with $\mathbb{CP}^n/\mathbb{CP}^{n-k-1}$, after reordering coordinates. Define $\nu_m$ in the identical way. The Hermitian-metric identification with the conjugate line does not change the complex normal orientation.

The original coordinate embeddings may be nested, so first move one into transverse position. Keep $\mathbb{CP}^k=\mathbb P(A)$ for the first $k+1$ coordinates, and move $\mathbb{CP}^m$ to $\mathbb P(B)$ for the last $m+1$ coordinates. A unitary coordinate permutation accomplishes this. Every unitary matrix can be joined to the identity by diagonalizing it and varying its eigenvalue phases continuously, so this move is an [ambient isotopy](../../../../../ambient-isotopy.md). Its trace gives a cobordism carrying the transported normal [complex structure](../../../../../complex-structure.md), and hence leaves the input cobordism class unchanged.

If $k+m\geq n$, then

$$
A+B=\mathbb C^{n+1},\qquad
\dim_{\mathbb C}(A\cap B)=k+m-n+1.
$$

Their projectivizations are transverse and meet in $\mathbb{CP}^{r}$, where $r=k+m-n$. The direct-sum normal structure from question 1 restricts to

$$
\nu_k|_{\mathbb{CP}^{r}}\oplus\nu_m|_{\mathbb{CP}^{r}}
\cong\bar\gamma_r^{\oplus((n-k)+(n-m))}
=\bar\gamma_r^{\oplus(n-r)}
\cong\nu_r.
$$

The quotient map defining the transverse normal-bundle isomorphism is complex-linear here, so it agrees with the standard normal [complex structure](../../../../../complex-structure.md) and contributes no orientation sign. If $k+m<n$, the first and last coordinate subspaces have no nonzero vector in common, so their projectivizations are disjoint.

Consequently the [product of linear projective subspaces in complex cobordism](../../../../../product-of-linear-projective-subspaces-in-complex-cobordism.md) is

$$
\boxed{
[\mathbb{CP}^{k},\nu_k]*[\mathbb{CP}^{m},\nu_m]
=\begin{cases}
[\mathbb{CP}^{k+m-n},\nu_{k+m-n}],&k+m\geq n,\\
0,&k+m<n.
\end{cases}}
$$

The product degree is $2(2n-k-m)$, equal to the real codimension of the stated intersection when it exists. In the equality case $k+m=n$, the representative is one point with its complex-oriented normal space.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
