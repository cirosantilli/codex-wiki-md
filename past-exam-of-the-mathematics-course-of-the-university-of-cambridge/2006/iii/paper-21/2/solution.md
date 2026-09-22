<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Regard $\operatorname{Mat}_n(\mathbb C)$ as a real vector space of dimension $2n^2$, and let $\operatorname{Herm}_n(\mathbb C)$ be the real vector space of Hermitian matrices, of dimension $n^2$. The smooth Gram map

$$
F(A)=A^*A
$$

has $F^{-1}(I)=U(n)$ and differential $DF_A(K)=A^*K+K^*A$. At a unitary $A$, any Hermitian matrix $H$ is obtained by taking $K=AH/2$. Indeed $A^*K=H/2$ and $K^*A=H/2$. Hence $I$ is a [regular value](../../../../../regular-value.md), and the [regular level set theorem](../../../../../regular-level-set-theorem.md) proves the [unitary group as a regular level set](../../../../../unitary-group-as-a-regular-level-set.md) result:

$$
\boxed{U(n)\text{ is a smooth manifold of real dimension }n^2.}
$$

Similarly let $G(A)=A^TA$ from $\operatorname{Mat}_n(\mathbb R)$ to the symmetric real matrices, whose dimension is $n(n+1)/2$. At an orthogonal $A$ its differential is $DG_A(K)=A^TK+K^TA$, again onto by choosing $K=AH/2$ for a symmetric $H$. Therefore the [orthogonal group as a regular level set](../../../../../orthogonal-group-as-a-regular-level-set.md) has

$$
\boxed{\dim_{\mathbb R}O(n)=n^2-\frac{n(n+1)}2=\frac{n(n-1)}2.}
$$

Matrix multiplication is smooth on both groups, and inversion is conjugate transpose or transpose, respectively, so these manifold structures also make them [Lie groups](../../../../../lie-group.md). Both groups are closed and bounded in their finite-dimensional ambient matrix spaces, hence compact.

Realification identifies a unitary complex matrix with an orthogonal transformation of $\mathbb R^{2n}$. This is a smooth injective group homomorphism, with closed image, so $U(n)$ is the stated Lie subgroup of $O(2n)$. The assumed maximal-rank quotient map has fibers diffeomorphic to $U(n)$. Consequently the compact [homogeneous space](../../../../../homogeneous-space.md), also known as the [space of orthogonal complex structures](../../../../../space-of-orthogonal-complex-structures.md), has dimension

$$
d=\dim O(2n)-\dim U(n)=n(2n-1)-n^2=n(n-1).
$$

The original PDF's sphere is $S^{n^2}$, with a square on the exponent; its dimension exceeds $d$ by $n$.

For completeness, [maps to a sphere above the dimension of a compact smooth manifold are null-homotopic](../../../../../maps-to-a-sphere-above-the-dimension-of-a-compact-smooth-manifold-are-null-homotopic.md). Let $X$ be a compact [smooth manifold](../../../../../smooth-manifold.md) of dimension $d<q$, with $q\geq1$, and let $f:X\to S^q\subset\mathbb R^{q+1}$ be continuous. Choose a finite open cover on which $f$ is uniformly close to its value at a chosen point of that open set, and take a smooth [partition of unity](../../../../../partition-of-unity.md) subordinate to the cover. The weighted sum of those chosen sphere values is a smooth map $g_0:X\to\mathbb R^{q+1}$ uniformly within $\epsilon<1$ of $f$. It never vanishes. Normalize it to $g=g_0/\|g_0\|$. Normalizing $(1-s)f+sg_0$ gives a [homotopy](../../../../../homotopy.md) from $f$ to $g$, since that vector remains within $\epsilon$ of the unit vector $f$.

Every value of $g$ is critical because its differential has rank at most $d<q$. The [Sard theorem](../../../../../sard-s-theorem.md) makes its image have measure zero in $S^q$, so it misses some point $p$. The punctured sphere $S^q\setminus\{p\}$ is homeomorphic to $\mathbb R^q$ and contractible. Thus $g$, and hence $f$, is null-homotopic. This reasoning does not require $X$ to be connected, and all constant maps are homotopic because $S^q$ is path connected.

Apply it with $X=O(2n)/U(n)$ and $q=n^2$, for positive integer $n$. We obtain

$$
\boxed{[O(2n)/U(n),\,S^{n^2}]=\{[\text{constant map}]\}.}
$$

The notation means [homotopy](../../../../../homotopy.md) classes of maps; no [homotopy](../../../../../homotopy.md) equivalence between the two spaces is asserted.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 21](../../paper-21-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
