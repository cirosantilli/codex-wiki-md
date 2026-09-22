<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

A [holomorphic line bundle](../../../../../holomorphic-line-bundle.md) $L\to X$ is a rank-one [holomorphic vector bundle](../../../../../holomorphic-vector-bundle.md): it has local trivializations $L|_{U_i}\cong U_i\times\mathbb C$ whose fiberwise linear [transition functions of a vector bundle](../../../../../transition-function-of-a-vector-bundle.md) are nowhere-zero [holomorphic functions](../../../../../holomorphic-function.md). Equivalently, choose local holomorphic frames $e_i$ and write $e_j=g_{ij}e_i$ on overlaps, with $g_{ij}\in\mathcal O^*(U_i\cap U_j)$ and the cocycle relation on triple overlaps. A [holomorphic section](../../../../../holomorphic-section.md) over $U$ has coefficients $s_i$ holomorphic on $U\cap U_i$ in $s=s_i e_i$; consistency means $s_i=g_{ij}s_j$.

The [dual bundle](../../../../../dual-bundle.md) has fiber $L_x^*=\operatorname{Hom}_{\mathbb C}(L_x,\mathbb C)$. Its dual frames $e_i^*$ are characterized by $e_i^*(e_i)=1$, and the frame relation becomes $e_j^*=g_{ij}^{-1}e_i^*$. Reciprocals of nowhere-zero [holomorphic functions](../../../../../holomorphic-function.md) are holomorphic, and their cocycle relations persist. This defines the [holomorphic dual vector bundle](../../../../../holomorphic-dual-vector-bundle.md) structure on $L^*$, with holomorphic evaluation pairing $L^*\otimes L\to\mathcal O_X$.

Assume now that $X$ is compact and connected, and let $s$ and $t$ be nonzero global [holomorphic sections](../../../../../holomorphic-section.md) of $L$ and $L^*$, respectively. The function $t(s)$ is a global [holomorphic function](../../../../../holomorphic-function.md). The [maximum modulus principle](../../../../../maximum-modulus-principle.md), applied in local complex coordinate lines near a maximum and then propagated on the connected manifold, makes it constant. Moreover it is not identically zero: the zero locus of a nonzero [holomorphic section](../../../../../holomorphic-section.md) has empty interior by the [identity theorem](../../../../../identity-theorem.md), so the two nonvanishing loci are dense open sets and intersect. Thus $t(s)=c\ne0$ everywhere.

In particular, $s$ never vanishes. The map $(x,a)\mapsto a s(x)$ is a holomorphic bundle isomorphism $X\times\mathbb C\to L$; in a local frame its inverse divides by the nowhere-zero holomorphic coefficient of $s$. Conversely, a holomorphic trivialization supplies the constant unit sections of both $L$ and $L^*$. We have proved the [two-section criterion for holomorphic triviality](../../../../../two-section-criterion-for-holomorphic-triviality.md):

$$
\boxed{L\text{ is holomorphically trivial}\quad\Longleftrightarrow\quad
H^0(X,L)\ne0\text{ and }H^0(X,L^*)\ne0.}
$$

Write points of [Complex projective space](../../../../../complex-projective-space.md) as lines $[Z]\subset\mathbb C^{n+1}$. The [complex tautological line bundle](../../../../../complex-tautological-line-bundle.md) is

$$
\mathcal O(-1)=\{([Z],v):v\in\mathbb C Z\}\subset\mathbb P^n\times\mathbb C^{n+1},
$$

with fiber that very line. Its dual is the [hyperplane line bundle](../../../../../hyperplane-line-bundle.md) $\mathcal O(1)$. On the affine chart $U_i=\{Z_i\ne0\}$, the vector $e_i([Z])=Z/Z_i$ is a nowhere-zero holomorphic frame of $\mathcal O(-1)$. On $U_i\cap U_j$,

$$
e_j=\frac{Z_i}{Z_j}e_i,\qquad
e_j^*=\frac{Z_j}{Z_i}e_i^*.
$$

Both ratios are nowhere-zero [holomorphic functions](../../../../../holomorphic-function.md) of the affine coordinates. They exhibit the holomorphic [transition functions of a vector bundle](../../../../../transition-function-of-a-vector-bundle.md) for the two bundles explicitly.

Choose a nonzero linear functional $\ell:\mathbb C^{n+1}\to\mathbb C$ whose zero hyperplane is $H$. At $[Z]$, its restriction to $\mathbb C Z$ is an element of that line's dual and therefore defines a [holomorphic section](../../../../../holomorphic-section.md) $s_\ell$ of $\mathcal O(1)$. In the dual frame above its coefficient is

$$
s_\ell=\frac{\ell(Z)}{Z_i}e_i^*\quad\text{on }U_i.
$$

This expression is holomorphic even along $H$, and its zero locus is exactly $H$. Consequently **$s_\ell|_{\mathbb P^n\setminus H}$ is the requested nowhere-zero section; its global holomorphic extension vanishes precisely on $H$**. The extension need not, and does not, stay nowhere zero on the hyperplane.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 22](../../paper-22-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
