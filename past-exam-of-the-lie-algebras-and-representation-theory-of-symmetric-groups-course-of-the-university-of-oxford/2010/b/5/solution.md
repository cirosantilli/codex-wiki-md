<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [tabloid](../../../../tabloid.md) is the row-equivalence class $\{t\}$ of a tableau filled bijectively with $1,\ldots,n$: order inside each row is forgotten, but the rows remain distinguished. The [permutation module](../../../../permutation-module.md) $M^\lambda$ has these tabloids as an $F$-[basis](../../../../basis.md), with $\Sigma_n$ permuting their entries. Let $C_t$ be the column stabilizer of $t$ and define

$$
\kappa_t=\sum_{\sigma\in C_t}\operatorname{sgn}(\sigma)\sigma,\qquad
e_t=\kappa_t\{t\}.
$$

The [Specht module](../../../../specht-module.md) $S^\lambda$ is the [submodule](../../../../submodule.md) spanned by all polytabloids $e_t$.

If a [module](../../../../module-mathematics.md) homomorphism $\phi:M^\lambda\to M^\mu$ is nonzero on $S^\lambda$, it is nonzero on some spanning $e_t$. Equivariance gives $0\ne\phi(e_t)=\kappa_t\phi(\{t\})$, so $\kappa_tM^\mu\ne0$. The allowed criterion yields $\lambda\ge\mu$.

In [characteristic zero](../../../../characteristic-zero.md), [Maschke's theorem](../../../../maschke-s-theorem.md) gives an equivariant projection $M^\lambda\to S^\lambda$. If $S^\lambda\cong S^\mu$, compose that projection with the isomorphism and the inclusion into $M^\mu$. The preceding argument gives $\lambda\ge\mu$. Reversing the roles gives $\mu\ge\lambda$, so antisymmetry of dominance gives

$$
\boxed{\lambda=\mu.}
$$

For a map defined only on a [Specht module](../../../../specht-module.md) in arbitrary characteristic, **dominance need not hold**. Take $F=\mathbb F_2$, $n=2$, $\lambda=(1,1)$ and $\mu=(2)$. The first [Specht module](../../../../specht-module.md) is the one-dimensional span of

$$
e=\{1\mid2\}-\{2\mid1\}=\{1\mid2\}+\{2\mid1\}.
$$

The transposition fixes $e$, so this is the trivial [module](../../../../module-mathematics.md). The one-row [permutation module](../../../../permutation-module.md) $M^{(2)}$ is also trivial and one-dimensional. Sending $e$ to its single [tabloid](../../../../tabloid.md) is a nonzero equivariant map, yet $(1,1)\not\ge(2)$. In this characteristic such a map need not extend to the surrounding [permutation module](../../../../permutation-module.md); that is exactly where the earlier proof ceases to apply.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../split.md)
5. [Lie algebras and representation theory of symmetric groups course of the University of Oxford](../../../../lie-algebras-and-representation-theory-of-symmetric-groups-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
