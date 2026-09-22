<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret $\theta$ as a continuous finite-dimensional complex [group representation](../../../../../../group-representation.md), so its values lie in $\operatorname{GL}_{\mathbb C}(V)$, and interpret approximation in the [uniform norm](../../../../../../supremum-norm.md). Assume the usual Hausdorff convention for the compact topological [group](../../../../../../group-split.md). The following argument proves the required form of the [Peter-Weyl theorem](../../../../../../peter-weyl-theorem.md) without first assuming that $G$ is a [Lie group](../../../../../../lie-group.md).

Start with normalized [Haar measure](../../../../../../haar-measure.md). It is both left- and right-invariant on a compact [group](../../../../../../group-split.md). Average any [Hermitian inner product](../../../../../../hermitian-form.md) to make a finite-dimensional representation unitary. The left regular action $L_a h(x)=h(a^{-1}x)$ is already unitary on $L^2(G)$.

Choose a continuous nonnegative [function](../../../../../../function-split.md) $k$ supported in a small symmetric identity neighbourhood, with $k(z^{-1})=k(z)$ and $\int k=1$. Such [functions](../../../../../../function-split.md) are obtained from a nonzero continuous bump near the identity, symmetrizing and normalizing. Define

$$
T_kh(x)=\int_Gk(y^{-1}x)h(y)\,dy
=\int_Gk(z)h(xz^{-1})\,dz.
$$

The [convolution](../../../../../../convolution.md) operator $T_k$ commutes with [left translations](../../../../../../left-and-right-translation-on-a-lie-group.md). Its continuous kernel is Hermitian, hence it is self-adjoint. It is compact on $L^2(G)$: approximate the continuous kernel uniformly by finite sums of separated [functions](../../../../../../function-split.md) of $x$ and $y$, using the [Stone-Weierstrass theorem](../../../../../../stone-weierstrass-theorem.md) on the compact product. The corresponding operators have finite rank and converge in operator norm. It also maps into $C(G)$ and satisfies

$$
\|T_kh\|_\infty\leq\|k\|_2\|h\|_2,
$$

by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md); continuity follows from the [uniform continuity](../../../../../../uniform-continuity.md) of the translated kernel.

The [spectral theorem for compact self-adjoint operators](../../../../../../spectral-theorem-for-compact-hermitian-operators.md) decomposes the [orthogonal complement](../../../../../../orthogonal-complement.md) of its kernel into finite-dimensional [eigenspaces](../../../../../../eigenspace.md) with nonzero [eigenvalues](../../../../../../eigenvalue.md). Every such [eigenspace](../../../../../../eigenspace.md) is left-translation invariant, and all its elements are continuous, since $h=T_kh/\lambda$ there. If $W\subset C(G)$ is one of these invariant spaces, write $\rho(a)=L_a|_W$. Evaluation at the identity gives

$$
h(x)=\operatorname{ev}_e\bigl(\rho(x^{-1})h\bigr)
=\bigl(\rho^\vee(x)\operatorname{ev}_e\bigr)(h).
$$

Thus $h$ is a [matrix coefficient](../../../../../../matrix-coefficient.md) of the [dual representation](../../../../../../dual-representation.md). This identifies each finite spectral sum with finite-dimensional representation data.

To get uniform rather than just $L^2$ approximation, let $S_N$ project onto increasing finite sums of the nonzero [eigenspaces](../../../../../../eigenspace.md). For $f\in C(G)$, $T_kf$ is orthogonal to the kernel, so $S_NT_kf\to T_kf$ in $L^2$. Applying the displayed smoothing bound gives

$$
\|T_kS_NT_kf-T_k^2f\|_\infty\longrightarrow0.
$$

Meanwhile, choosing the support of $k$ sufficiently small makes $T_kf$ uniformly close to $f$, by [uniform continuity](../../../../../../uniform-continuity.md) under small translations. Since $\|T_k\|_{C\to C}\leq1$, it also makes $T_k^2f$ uniformly close to $f$. Every $T_kS_NT_kf$ belongs to a finite sum of invariant [eigenspaces](../../../../../../eigenspace.md), hence is a finite sum of [matrix coefficients](../../../../../../matrix-coefficient.md). This completes the [convolution proof of uniform Peter-Weyl approximation](../../../../../../convolution-proof-of-uniform-peter-weyl-approximation.md).

A coefficient $\ell(\theta(g)v)$ equals $\operatorname{tr}(\alpha\theta(g))$ for the rank-one [endomorphism](../../../../../../endomorphism.md) $\alpha=v\otimes\ell$. Finite sums of coefficients can be combined using a direct-sum representation and a block-diagonal $\alpha$. Therefore the conclusion has exactly the requested form:

$$
\boxed{\text{For every }\varepsilon>0\text{ there are }V,\theta,\alpha
\text{ with }\sup_{g\in G}|f(g)-\operatorname{tr}(\alpha\theta(g))|<\varepsilon.}
$$

For a [class function](../../../../../../class-function.md) $f$, apply [conjugation averaging on a compact group](../../../../../../conjugation-averaging-on-a-compact-group.md),

$$
\mathcal AF(g)=\int_G F(hgh^{-1})\,dh.
$$

It fixes $f$ and is a contraction in the [uniform norm](../../../../../../supremum-norm.md), so averaging an approximation preserves its error bound. A [trace](../../../../../../matrix-trace.md) coefficient averages to $\operatorname{tr}(\overline\alpha\theta(g))$, where

$$
\overline\alpha=\int_G\theta(h)^{-1}\alpha\theta(h)\,dh.
$$

This [endomorphism](../../../../../../endomorphism.md) commutes with the representation. A finite-dimensional [unitary representation](../../../../../../unitary-representation.md) splits into irreducibles by repeatedly taking invariant orthogonal complements. On each irreducible diagonal block, [Schur lemma](../../../../../../schur-s-lemma.md) makes its average a scalar multiple of the identity, namely its [trace](../../../../../../matrix-trace.md) divided by the block dimension. Off-diagonal blocks do not contribute to the total [trace](../../../../../../matrix-trace.md). Thus the averaged coefficient is a finite [linear combination](../../../../../../linear-combination.md) of [irreducible characters](../../../../../../irreducible-character.md). Consequently **irreducible complex characters span a uniformly dense subspace of the continuous [class functions](../../../../../../class-function.md)**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
