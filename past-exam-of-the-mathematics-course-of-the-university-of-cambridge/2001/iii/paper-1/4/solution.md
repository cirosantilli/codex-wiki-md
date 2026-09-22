<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We prove uniform approximation, not just approximation in $L^2$. The analytic facts used are: a [continuous](../../../../../continuous-function.md) square-integrable kernel gives a compact integral operator on $L^2$; the [spectral theorem for compact self-adjoint operators](../../../../../spectral-theorem-for-compact-hermitian-operators.md) decomposes the closure of its range into its finite-dimensional nonzero [eigenspaces](../../../../../eigenspace.md); and [continuous](../../../../../continuous-function.md) functions are dense in $L^2$ for normalized [Haar measure](../../../../../haar-measure.md) on a [compact Lie group](../../../../../compact-lie-group.md). Normalized [Haar measure](../../../../../haar-measure.md) on a compact [group](../../../../../group-split.md) is both left- and right-invariant and is preserved by inversion.

Choose a [continuous](../../../../../continuous-function.md) nonnegative function $k$ of integral one, supported in a sufficiently small symmetric neighborhood of the identity, with $k(g^{-1})=k(g)$. Such functions are obtained from a local bump and its inverted bump followed by normalization. Define the [convolution](../../../../../convolution.md) operator

$$
(Th)(x)=\int_Gh(y)k(y^{-1}x)\,dy.
$$

Its kernel is [continuous](../../../../../continuous-function.md) on $G\times G$, so $T$ is compact. The symmetry of $k$ makes it self-adjoint. It commutes with the [left translations](../../../../../left-and-right-translation-on-a-lie-group.md) $(L_gh)(x)=h(g^{-1}x)$ by a change of variable $y=gz$.

By [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) and invariance of [Haar measure](../../../../../haar-measure.md),

$$
\|Th\|_\infty\leq\|k\|_2\|h\|_2.
$$

The same integral formula and continuity of the kernel show $Th$ is [continuous](../../../../../continuous-function.md) for every $h\in L^2(G)$. Moreover, rewriting $y=xz^{-1}$ gives $(Tf)(x)=\int f(xz^{-1})k(z)\,dz$. Uniform continuity on the compact [group](../../../../../group-split.md) therefore makes $\|Tf-f\|_\infty$ arbitrarily small when the support of $k$ is small. Also $\|T\|_{\infty\to\infty}\leq1$ because $k\geq0$ and has integral one.

Fix $\varepsilon>0$ and take $k$ so $\|Tf-f\|_\infty<\varepsilon/3$. Then

$$
\|T^2f-f\|_\infty
\leq\|T(Tf-f)\|_\infty+\|Tf-f\|_\infty
<2\varepsilon/3.
$$

Let $P_N$ be the [orthogonal projection](../../../../../orthogonal-projection.md) onto increasing finite sums of the nonzero [eigenspaces](../../../../../eigenspace.md) of $T$. Since $Tf$ lies in the closure of the range, the [spectral theorem](../../../../../spectral-theorem.md) gives $P_NTf\to Tf$ in $L^2$. Applying the smoothing estimate gives

$$
\|TP_NTf-T^2f\|_\infty
\leq\|k\|_2\|P_NTf-Tf\|_2\longrightarrow0.
$$

Thus some $h=TP_NTf$ satisfies $\|h-f\|_\infty<\varepsilon$.

Each nonzero [eigenspace](../../../../../eigenspace.md) is finite dimensional, invariant under $L_g$, and consists of [continuous](../../../../../continuous-function.md) functions: if $Tv=\lambda v$ with $\lambda\ne0$, then $v=Tv/\lambda$. The finite sum $M$ containing $h$ therefore carries the finite-dimensional [unitary representation](../../../../../unitary-representation.md) $\rho(g)=L_g|_M$. It is [continuous](../../../../../continuous-function.md), since translating each of its finitely many [continuous](../../../../../continuous-function.md) basis functions depends continuously on $g$ in the uniform and hence the $L^2$ norm.

Let $\ell$ be evaluation at the identity on $M$, and let the [dual representation](../../../../../dual-representation.md) on $M^*$ be $\theta(g)\ell=\ell\circ\rho(g^{-1})$. For the linear functional $L_h$ on $M^*$ defined by $L_h(u)=u(h)$,

$$
L_h(\theta(g)\ell)=\ell(\rho(g^{-1})h)=h(g).
$$

The rank-one endomorphism $\alpha=\ell\otimes L_h$ of $M^*$ satisfies $\operatorname{tr}(\alpha\theta(g))=L_h(\theta(g)\ell)$. Therefore

$$
\boxed{\|f-\operatorname{tr}(\alpha\theta(\,\cdot\,))\|_\infty<\varepsilon.}
$$

This is the requested [Peter-Weyl theorem](../../../../../peter-weyl-theorem.md), proved via the [convolution proof of uniform Peter-Weyl approximation](../../../../../convolution-proof-of-uniform-peter-weyl-approximation.md). The extra convolution after the spectral truncation is what upgrades the $L^2$ estimate to a uniform one.

To deduce a faithful finite-dimensional [representation](../../../../../group-representation.md), first note that these [representations](../../../../../group-representation.md) separate points. For $g\ne e$, choose a [continuous](../../../../../continuous-function.md) function taking different values at $g$ and $e$, and approximate it closely enough by a [trace](../../../../../matrix-trace.md) coefficient to retain that difference. The [representation](../../../../../group-representation.md) appearing in that [trace](../../../../../matrix-trace.md) must satisfy $\theta(g)\ne I$.

There is an identity neighborhood $U$ containing no nontrivial subgroup. Here is the [Lie groups have no small subgroups](../../../../../lie-groups-have-no-small-subgroups.md) argument: choose an injective exponential chart on a Lie-algebra ball of radius $r$, and take $U=\exp(B_\delta)$ with $0<\delta<r/2$. If a subgroup contained a nonidentity $\exp X$ in $U$, choose the first integer $m$ with $m\|X\|\geq\delta$. Then $\delta\leq m\|X\|<2\delta<r$, so its power $\exp(mX)$ lies outside $U$, a contradiction. For a zero-dimensional [group](../../../../../group-split.md), take $U=\{e\}$.

For every $g\notin U$, choose a [representation](../../../../../group-representation.md) nontrivial at $g$. The sets on which these [representations](../../../../../group-representation.md) are not the identity are open and cover the compact set $G\setminus U$. A finite subcover gives finitely many [representations](../../../../../group-representation.md), whose [direct sum](../../../../../direct-sum.md) has kernel contained in $U$. A subgroup contained in $U$ is trivial, so this [direct sum](../../../../../direct-sum.md) is faithful. Averaging its Hermitian form makes it unitary. Thus the [finite faithful representation from point-separating representations](../../../../../finite-faithful-representation-from-point-separating-representations.md) yields

$$
\boxed{G\hookrightarrow U_n\text{ for some finite }n.}
$$

Using the no-small-subgroups neighborhood is essential; $G\setminus\{e\}$ alone need not be compact, so a finite-subcover argument on that punctured set would not be valid.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
