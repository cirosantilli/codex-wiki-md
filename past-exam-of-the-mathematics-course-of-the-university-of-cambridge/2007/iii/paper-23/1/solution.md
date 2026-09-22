<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Use the quotient convention for [projective space](../../../../../projective-space-split.md). To a [scheme](../../../../../scheme.md) $T$, associate the set of pairs

$$
(q,\mathcal L),\qquad q:\mathcal O_T^{\oplus(n+1)}\twoheadrightarrow\mathcal L,
$$

where $\mathcal L$ is a [line bundle](../../../../../line-bundle.md), modulo [isomorphisms](../../../../../isomorphism.md) $\mathcal L\to\mathcal L'$ carrying $q$ to $q'$. Pullback defines the contravariant [functor](../../../../../functor.md). On $T=\operatorname{Spec}A$, this means rank-one [projective module](../../../../../projective-module.md) quotients of $A^{n+1}$; the quotient need not be free. Thus merely listing generating tuples modulo multiplication by a unit would omit points over rings with nontrivial [Picard group](../../../../../picard-group.md).

This [functor](../../../../../functor.md) is represented by $\mathbb P^n_{\mathbb Z}$. For each $i$, the locus where $q(e_i)$ generates $\mathcal L$ is open. These loci cover $T$, since a surjection onto a rank-one free stalk must have some coefficient a unit in its [local ring](../../../../../local-ring.md). On this locus, trivialize by $q(e_i)$ and write

$$
t_j=\frac{q(e_j)}{q(e_i)},\qquad j\ne i.
$$

These functions specify a map to the standard chart $U_i=\operatorname{Spec}\mathbb Z[t_j:j\ne i]$. Their transition rules are exactly those of [projective space](../../../../../projective-space-split.md), so the chart maps glue. Conversely the universal quotient on [projective space](../../../../../projective-space-split.md) pulls back to the given pair, and the construction is natural and unique. This proves that [projective space represents invertible quotients](../../../../../projective-space-represents-invertible-quotients.md).

Write its universal exact sequence as

$$
0\longrightarrow\mathcal K\longrightarrow V\otimes\mathcal O\xrightarrow q\mathcal O(1)\longrightarrow0,\qquad V=\mathbb Z^{n+1}.
$$

A first-order change of the quotient, with target trivialized locally, is a map $\delta q:V\otimes\mathcal O\to\mathcal O(1)$. Changing the target trivialization by $1+\varepsilon h$ changes $\delta q$ by $hq$. Restriction to $\mathcal K$ removes this ambiguity, and every local map $\mathcal K\to\mathcal O(1)$ extends because the displayed sequence splits locally. Consequently the [tangent sheaf of a scheme](../../../../../tangent-sheaf-of-a-scheme.md) is

$$
\mathcal T_{\mathbb P^n/\mathbb Z}\cong\mathcal H om(\mathcal K,\mathcal O(1)).
$$

This identification can also be seen on $U_i$: the first-order change of $t_j$ is $\delta q(e_j)-t_j\delta q(e_i)$ after setting $q(e_i)=1$. Thus these maps are precisely the coordinate tangent directions.

Apply $\mathcal H om(-,\mathcal O(1))$ to the universal sequence. Since its terms are [locally free](../../../../../locally-free-sheaf.md) and it splits locally, this gives the [Euler sequence](../../../../../euler-sequence.md)

$$
\boxed{0\longrightarrow\mathcal O\xrightarrow{(X_0,\ldots,X_n)}\mathcal O(1)^{\oplus(n+1)}\longrightarrow\mathcal T_{\mathbb P^n/\mathbb Z}\longrightarrow0.}
$$

It remains exact after any base change. Taking its [dual of a sheaf](../../../../../dual-of-a-sheaf.md) over a [field](../../../../../field.md) $k$ gives

$$
0\longrightarrow\Omega^1_{\mathbb P^n_k/k}\longrightarrow\mathcal O(-1)^{\oplus(n+1)}\longrightarrow\mathcal O\longrightarrow0.
$$

For $n=1$, the first term has rank one; taking determinants yields

$$
\boxed{\Omega^1_{\mathbb P^1_k/k}\cong\mathcal O(-2).}
$$

Explicitly, for $u=t^{-1}$ on the overlap of the two affine charts, $du=-t^{-2}dt$, the same transition as $\mathcal O(-2)$ after changing one local frame's sign.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
