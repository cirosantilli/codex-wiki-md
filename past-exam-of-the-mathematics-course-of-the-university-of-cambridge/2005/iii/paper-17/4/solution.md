<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $n=\operatorname{rank}_{\mathbb Z}M$. Work with [commutative rings](../../../../../commutative-ring.md) and take a quotient to mean a surjection $p:M\otimes_{\mathbb Z}R\twoheadrightarrow Q$, considered up to an [isomorphism](../../../../../isomorphism.md) of $Q$ commuting with $p$. Equivalently, retain its [kernel](../../../../../kernel-of-a-linear-map.md) as a submodule of $M\otimes R$. Here a rank-$r$ [locally free module](../../../../../locally-free-module.md) is finite locally free, or equivalently a [finite projective module](../../../../../finite-projective-module.md) of constant rank $r$. A [ring homomorphism](../../../../../ring-homomorphism.md) $R\to R'$ sends the quotient to

$$
M\otimes R'\twoheadrightarrow Q\otimes_RR'.
$$

The [tensor product of modules](../../../../../tensor-product-of-modules.md) is right exact and preserves finite projectivity, so this defines the functorial action. We prove [scheme](../../../../../scheme.md) representability in the usual [functor of points](../../../../../functor-represented-by-a-scheme.md) sense:

$$
\boxed{F(R)\cong\operatorname{Hom}_{\mathbb Z}
\bigl(\operatorname{Spec}R,\operatorname{Gr}_r(M)\bigr),}
$$

naturally in $R$. The [Grassmannian of locally free quotients](../../../../../grassmannian-of-locally-free-quotients.md) will be constructed explicitly.

Assume first $0<r<n$, and choose a [basis](../../../../../basis.md) $e_1,\ldots,e_n$ of $M$. For every ordered subset $I=\{i_1<\cdots<i_r\}\subseteq\{1,\ldots,n\}$, consider those quotients for which $p(e_{i_1}),\ldots,p(e_{i_r})$ are a [basis](../../../../../basis.md) of $Q$. This choice gives a unique identification $Q\cong R^r$, in which the quotient is represented by an $r\times n$ [matrix](../../../../../matrix.md) $A_I$ whose columns indexed by $I$ are the identity [matrix](../../../../../matrix.md). Its remaining $r(n-r)$ entries are arbitrary elements of $R$. Thus this subfunctor is represented by the [affine scheme](../../../../../affine-scheme.md)

$$
U_I=\operatorname{Spec}\mathbb Z[a_{kj}:1\leq k\leq r,\ j\notin I]
\cong\mathbb A^{r(n-r)}_{\mathbb Z}.
$$

There is no further change-of-basis ambiguity: the selected quotient images already specify its [basis](../../../../../basis.md) uniquely.

For another subset $J$, write $A_I^{(J)}$ for the square submatrix consisting of the $J$ columns. The same quotient lies in the $J$ chart exactly when its [determinant](../../../../../determinant.md) is a unit. Consequently the chart overlap is the [principal open subset](../../../../../principal-open-subscheme.md)

$$
U_{IJ}=D(\delta_{IJ})\subseteq U_I,\qquad
\delta_{IJ}=\det A_I^{(J)}.
$$

On that overlap the [matrix](../../../../../matrix.md) normalized in the $J$ [basis](../../../../../basis.md) is

$$
\boxed{A_J=(A_I^{(J)})^{-1}A_I.}
$$

The entries are regular on $D(\delta_{IJ})$ by the [adjugate matrix](../../../../../adjugate-matrix.md). Conversely, the $I$ columns of $A_J$ form $(A_I^{(J)})^{-1}$, so normalization back to $I$ recovers $A_I$. The transition is therefore an [isomorphism](../../../../../isomorphism.md) $U_{IJ}\cong U_{JI}$.

The cocycle identity follows from the same [matrix](../../../../../matrix.md) computation, not just an assertion about [bases](../../../../../basis.md). On a triple overlap, normalization first to $J$ and then to $K$ gives

$$
\begin{aligned}
(A_J^{(K)})^{-1}A_J
&=\left((A_I^{(J)})^{-1}A_I^{(K)}\right)^{-1}
(A_I^{(J)})^{-1}A_I\\
&=(A_I^{(K)})^{-1}A_I.
\end{aligned}
$$

This is direct normalization from $I$ to $K$. By [gluing of schemes along open subschemes](../../../../../gluing-of-schemes-along-open-subschemes.md), the [standard affine charts of the quotient Grassmannian](../../../../../standard-affine-charts-of-the-quotient-grassmannian.md) therefore glue to a [scheme](../../../../../scheme.md) $G$ over $\mathbb Z$.

The universal [matrices](../../../../../matrix.md) also glue a universal quotient. On $U_I$, use the surjection

$$
M\otimes_{\mathbb Z}\mathcal O_{U_I}\xrightarrow{\ A_I\ }
\mathcal O_{U_I}^{\oplus r}.
$$

On overlaps, identify its targets by $(A_I^{(J)})^{-1}$, precisely the transition [matrix](../../../../../matrix.md) above. The cocycle identity glues these free sheaves into a rank-$r$ [locally free sheaf](../../../../../locally-free-sheaf.md) $\mathcal Q$ and glues the maps into $M\otimes\mathcal O_G\twoheadrightarrow\mathcal Q$. Its [kernel](../../../../../kernel-of-a-linear-map.md) $\mathcal S$ is locally free of rank $n-r$: on $U_I$ an explicit [basis](../../../../../basis.md) is

$$
e_j-\sum_{k=1}^ra_{kj}e_{i_k},\qquad j\notin I.
$$

Hence we have the universal [exact sequence](../../../../../exact-sequence.md)

$$
\boxed{0\longrightarrow\mathcal S\longrightarrow
M\otimes_{\mathbb Z}\mathcal O_G\longrightarrow\mathcal Q
\longrightarrow0,\qquad \operatorname{rank}\mathcal S=n-r,
\quad\operatorname{rank}\mathcal Q=r.}
$$

It remains to verify that these charts capture every quotient, including a nonfree projective target. Given $p:R^n\twoheadrightarrow Q$, define $V_I\subseteq\operatorname{Spec}R$ as the locus where the selected images $p(e_i)$, $i\in I$, form a [basis](../../../../../basis.md). This is open: locally trivialize the [locally free sheaf](../../../../../locally-free-sheaf.md) associated with $Q$, and it is the nonvanishing locus of the corresponding maximal minor. The sets $V_I$ cover $\operatorname{Spec}R$. Indeed, at every prime $\mathfrak p$, the images of all $n$ vectors span the $r$-dimensional residue-field quotient, so some $r$ of them form a [basis](../../../../../basis.md) there. Their [determinant](../../../../../determinant.md) is a unit in $R_{\mathfrak p}$, hence they form a [basis](../../../../../basis.md) over that [local ring](../../../../../local-ring.md) and on an open neighbourhood of $\mathfrak p$.

On $V_I$, trivialize $Q$ using exactly those selected images. The remaining columns give regular functions and hence a morphism $V_I\to U_I$. On $V_I\cap V_J$, the normalized [matrices](../../../../../matrix.md) satisfy the displayed transition formula, so the local morphisms glue to a morphism

$$
f_p:\operatorname{Spec}R\longrightarrow G.
$$

Its pullback of the universal quotient is the original quotient, because this is true in each of the specified [bases](../../../../../basis.md). Conversely, any morphism $f:\operatorname{Spec}R\to G$ pulls back the universal sequence to a rank-$r$ locally free quotient. On each inverse-image chart its [matrix](../../../../../matrix.md) is exactly the normalized [matrix](../../../../../matrix.md) used to reconstruct $f$, so the two constructions are inverse. They are unchanged by an [isomorphism](../../../../../isomorphism.md) commuting with the quotient map, and they commute with every [base change](../../../../../base-change-of-a-morphism-of-schemes.md) $R\to R'$. This proves the natural bijection and therefore

$$
\boxed{G=\operatorname{Gr}_r(M)\text{ represents }F.}
$$

Taking kernels over a field identifies this with the usual [Grassmannian](../../../../../grassmannian.md) of $(n-r)$-dimensional subspaces of $M\otimes k$. The construction itself does not assume the target [module](../../../../../module-mathematics.md) is globally free.

For $r=0$, the only quotient is zero; for $r=n$, a surjection to a [locally free module](../../../../../locally-free-module.md) of the same rank is an [isomorphism](../../../../../isomorphism.md), as can be checked locally by its [determinant](../../../../../determinant.md). Both endpoint functors are represented by $\operatorname{Spec}\mathbb Z$. If $r>n$, no such quotient exists over a nonempty test [scheme](../../../../../scheme.md), and the representing [scheme](../../../../../scheme.md) is empty. Finally, [scheme](../../../../../scheme.md) representability does not mean representation by a single [ring](../../../../../ring.md): already $r=1,n=2$ gives $\mathbb P^1_{\mathbb Z}$, which is not affine. This is the standard algebraic-geometric meaning of representability for the functor on [rings](../../../../../ring.md) here.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 17](../../paper-17-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
