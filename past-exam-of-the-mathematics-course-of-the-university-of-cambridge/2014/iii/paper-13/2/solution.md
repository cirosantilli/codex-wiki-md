<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For an [affine variety](../../../../../affine-algebraic-set.md) $V\subseteq\mathbb A_k^N$, one construction defines $\mathcal O_V(U)$ as the functions $U\to k$ which locally have the form $p/q$, where $p,q$ are elements of the [coordinate ring](../../../../../coordinate-ring.md) $k[V]$ and $q$ does not vanish on the neighbourhood in question. Restrictions are restrictions of functions, and locality gives the [sheaf](../../../../../sheaf-mathematics.md) axioms. In particular

$$
\boxed{\mathcal O_V(D(f))=k[V]_f,\qquad(\mathcal O_V)_x=k[V]_{\mathfrak m_x}.}
$$

The second formula identifies its [local rings](../../../../../local-ring.md).

In the classical convention, an [algebraic variety](../../../../../algebraic-variety.md) over $k$ is an irreducible [ringed space](../../../../../ringed-space-split.md) with a [sheaf](../../../../../sheaf-mathematics.md) of $k$-valued functions, admitting a finite [open cover](../../../../../open-cover.md) by spaces isomorphic to affine varieties, and satisfying the [separated variety](../../../../../separated-variety.md) condition that its diagonal is closed in $X\times X$. Its topology is Noetherian. One can instead allow reducible reduced varieties; the arguments below still work with the denominator-clearing version of the [localization](../../../../../localization-of-a-ring.md) argument. A [morphism of varieties](../../../../../morphism-of-algebraic-varieties.md) is a continuous map whose pullback takes local [regular functions](../../../../../regular-function.md) to [regular functions](../../../../../regular-function.md), equivalently a morphism of locally ringed $k$-spaces. The maps on [local rings](../../../../../local-ring.md) are local because a function nonzero at the image point stays nonzero at the source point.

An [affine variety](../../../../../affine-algebraic-set.md) supplies its own finite affine cover, is Noetherian, and is separated: its diagonal in $V\times V$ is cut out by the differences of corresponding coordinates. A [regular map](../../../../../morphism-of-algebraic-varieties.md) between affine varieties pulls coordinate functions back to [regular functions](../../../../../regular-function.md). It is continuous because the inverse image of any [polynomial](../../../../../polynomial-split.md) zero set is the zero set of the pulled-back [regular functions](../../../../../regular-function.md); on affine charts such zero sets are closed. Pulling back a locally represented fraction $p/q$ gives a regular fraction wherever its denominator is nonzero. Hence a regular map is a [morphism of varieties](../../../../../morphism-of-algebraic-varieties.md) in this definition.

For a morphism $\phi:X\to Y$ which is an [isomorphism](../../../../../isomorphism.md) over each member $U_i$ of an [open cover](../../../../../open-cover.md) of $Y$, every fibre contains exactly one point. Thus $\phi$ is bijective. Its inverse is continuous and regular on every $U_i$, since there it is the given inverse of the local [isomorphism](../../../../../isomorphism.md). These inverses agree on overlaps, being inverses of the same map. They glue to a global inverse [morphism of varieties](../../../../../morphism-of-algebraic-varieties.md). Therefore **being an [isomorphism](../../../../../isomorphism.md) is local on the target**.

Let $A=\Gamma(X,\mathcal O_X)$, and let $Y$ be affine with [coordinate ring](../../../../../coordinate-ring.md) $B$. Given a $k$-algebra homomorphism $\alpha:B\to A$, choose a presentation $B=k[y_1,\ldots,y_N]/I$. The map

$$
\boxed{x\longmapsto\bigl(\alpha(y_1)(x),\ldots,\alpha(y_N)(x)\bigr)}
$$

lands in $Y$ because all the equations in $I$ become zero functions. Its coordinates are [global regular functions](../../../../../global-regular-function.md), so it is a morphism on every affine chart of $X$, and therefore globally. On a target neighbourhood where a fraction $b/c$ is defined its pullback is $\alpha(b)/\alpha(c)$, proving that the induced map on [global sections](../../../../../global-section.md) is exactly $\alpha$. This also proves independence of the chosen generators and uniqueness. This is the [affine-target adjunction for varieties](../../../../../affine-target-adjunction-for-varieties.md).

For $f\in A$, the natural map $A_f\to\Gamma(X_f,\mathcal O_X)$ sends $a/f^N$ to that [regular function](../../../../../regular-function.md). In the irreducible convention, if $f\ne0$, $X_f$ is dense, so this map is injective: a global [regular function](../../../../../regular-function.md) vanishing there vanishes everywhere. Cover $X$ by finitely many affine charts $U_j$. A section $s$ on $X_f$ restricts on $U_j\cap X_f=D_{U_j}(f|_{U_j})$ to an element of $\Gamma(U_j,\mathcal O_X)_{f|_{U_j}}$. A common power $f^N$ clears all these finitely many denominators. The resulting regular sections on $U_j$ agree on the dense principal open in each overlap, hence agree there altogether and glue to a [global section](../../../../../global-section.md) $a$. Thus $s=a/f^N$. If $f=0$, both sides are the zero ring of sections on the empty open. Consequently

$$
\boxed{\Gamma(X_f,\mathcal O_X)\cong A_f.}
$$

This is [localization of global sections on a principal open](../../../../../localization-of-global-sections-on-a-principal-open.md). For reduced reducible varieties, equality on a principal open instead means that a sufficiently large power of $f$ annihilates the difference; finitely many charts and overlap refinements allow one common extra power. The same denominator-clearing proof then gives the stated [localization](../../../../../localization-of-a-ring.md) [isomorphism](../../../../../isomorphism.md) without a density assumption.

Now suppose $\sum_i g_if_i=1$ in $A$ and every $X_{f_i}$ is affine. Each $A_{f_i}=\Gamma(X_{f_i},\mathcal O_X)$ is a finitely generated $k$-algebra. Select finitely many generators, writing them as $a_{ij}/f_i^{N_{ij}}$. Let $B\subseteq A$ be the $k$-subalgebra generated by all $f_i$, all $g_i$, and all $a_{ij}$. It is finitely generated, and

$$
\boxed{B_{f_i}=A_{f_i}\quad\text{for every }i.}
$$

The inclusion from left to right is immediate, while the chosen generators give the reverse inclusion. This construction does not assume that $A$ was finitely generated in advance.

The reduced algebra $B$ is the [coordinate ring](../../../../../coordinate-ring.md) of an affine variety $Y$ (irreducible when $X$ is). The map $B\hookrightarrow A$ produces $X\to Y$ by the preceding construction. The sets $D_Y(f_i)$ cover $Y$, since their functions generate the [unit ideal](../../../../../unit-ideal.md) already in $B$. Their inverse images are $X_{f_i}$, and on them the map is the [isomorphism](../../../../../isomorphism.md) corresponding to $B_{f_i}=A_{f_i}$. The target-local argument above now proves

$$
\boxed{X\cong Y\quad\text{and in particular }X\text{ is affine}.}
$$

This is [affineness from a unit-ideal principal affine cover](../../../../../affineness-from-a-unit-ideal-principal-affine-cover.md). The printed sets are $X_{f_i}$; the missing index in the TeX aid is not a different hypothesis.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 13](../../paper-13-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
