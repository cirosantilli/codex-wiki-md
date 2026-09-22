<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [weak-star topology](../../../../../weak-star-topology.md) $\sigma(X^*,X)$ is the coarsest topology making $f\mapsto f(x)$ continuous for every $x\in X$. Its basic neighbourhoods of zero impose finitely many inequalities $|f(x_j)|<\epsilon$.

Suppose first that zero had a countable neighbourhood base $(U_n)$ in the entire dual. Choose a basic neighbourhood $V_n\subset U_n$ controlled by a finite set $F_n\subset X$, and let $E_n=\operatorname{span}(F_1\cup\cdots\cup F_n)$. Given $x\in X$, the neighbourhood $W_x=\{f:|f(x)|<1\}$ contains some $U_n$, hence $V_n$. If $x\notin\operatorname{span}F_n$, the [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) supplies a [bounded linear functional](../../../../../continuous-linear-functional.md) $h$ which vanishes on $F_n$ but has $h(x)\ne0$. Indeed, the finite-dimensional span is closed, and the functional taking $e+tx$ to $t$ on its sum with $\mathbb F x$ is bounded because $\operatorname{dist}(x,\operatorname{span}F_n)>0$. Every scalar multiple of $h$ lies in $V_n$, contradicting $V_n\subset W_x$. Thus $x\in E_n$, and $X=\bigcup_n E_n$ has countable Hamel dimension.

If $X$ is infinite-dimensional, every finite-dimensional $E_n$ is closed and has empty interior. Completeness rules out their union. For clarity, the [Baire category theorem](../../../../../baire-category-theorem.md) needed here has a direct nested-ball proof: inside a starting open ball choose a closed ball missing $E_1$, then inside its interior choose a closed ball missing $E_2$, and continue with positive radii tending to zero. The centres are Cauchy; their limit belongs to every ball and to none of the $E_n$, a contradiction. A metric topology would have a countable ball base at zero. Hence

$$
\boxed{\sigma(X^*,X)\text{ is not metrizable on }X^*.}
$$

This is the [weak-star topology on an entire infinite-dimensional Banach dual is not metrizable](../../../../../weak-star-topology-on-an-entire-infinite-dimensional-banach-dual-is-not-metrizable.md) result. It does not contradict [weak-star metrizability of the dual ball](../../../../../weak-star-metrizability-of-the-dual-ball.md) for a separable predual: that assertion concerns a bounded subset.

The [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md) states that $B_{X^*}$ is compact for $\sigma(X^*,X)$ for every [normed vector space](../../../../../normed-vector-space.md) $X$, whether complete or not. Embed it in the product $\prod_{x\in X}\{a\in\mathbb F:|a|\le\|x\|\}$ by its evaluations. Each factor is compact, so [Tychonoff theorem](../../../../../tychonoff-s-theorem.md) makes the product compact Hausdorff. The equations expressing additivity and scalar homogeneity define a closed subset of the product. Its elements are exactly the bounded linear functionals of [norm](../../../../../norm.md) at most one, since the coordinate bounds give $|f(x)|\le\|x\|$. The induced product topology is precisely weak-star, proving the theorem.

The theorem printed as “Goldstein” is the standard [Goldstine theorem](../../../../../goldstine-theorem.md): $J(B_X)$ is weak-star dense in $B_{X^{**}}$ for the [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md). To prove it, fix $\Phi\in B_{X^{**}}$ and $f_1,\ldots,f_m\in X^*$. The set $S=\{(f_1(x),\ldots,f_m(x)):x\in B_X\}$ is [convex](../../../../../convex-function.md). If $b=(\Phi(f_1),\ldots,\Phi(f_m))$ were outside its closure, finite-dimensional [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) would supply coefficients $a_j$ such that, for $f=\sum_j a_jf_j$,

$$
\operatorname{Re}\Phi(f)>\sup_{x\in B_X}\operatorname{Re}f(x)=\|f\|.
$$

The real case omits real parts; in the complex case every real-linear separating functional on $\mathbb C^m$ has the displayed form. The [supremum](../../../../../supremum.md) equals the dual [norm](../../../../../norm.md) by multiplying vectors by signs or unimodular scalars. The strict inequality contradicts $\|\Phi\|\le1$. Thus $b\in\overline S$, which is exactly approximation on every prescribed finite family of weak-star coordinates.

Now take $K=B_{X^*}$ with its compact Hausdorff weak-star topology. For each $x\in X$, the evaluation $\widehat x:f\mapsto f(x)$ is continuous on $K$, and [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md) gives $\|\widehat x\|_\infty=\|x\|$. Therefore

$$
\boxed{X\longrightarrow C(K),\qquad x\longmapsto\widehat x}
$$

is the [isometric evaluation embedding into continuous functions on a compact dual ball](../../../../../isometric-evaluation-embedding-into-continuous-functions-on-a-compact-dual-ball.md), over the same scalar field as $X$.

For the final sequential assertions, choose a norm-dense sequence $(f_j)$ in the separable dual $X^*$ and suppose $\|x_n\|\le M$. Each bounded scalar sequence $f_j(x_n)$ has a convergent subsequence: divide a bounding interval or square into finitely many smaller closed pieces, repeatedly retain one containing infinitely many terms, and let the diameters tend to zero. Successive extraction for $j=1,2,\ldots$, followed by a diagonal subsequence $(y_n)$, makes every $f_j(y_n)$ converge.

If $M=0$ the conclusion is immediate. Otherwise, for any $f\in X^*$ and $\epsilon>0$, choose $j$ with $\|f-f_j\|<\epsilon/(4M)$. For sufficiently large $n,m$,

$$
|f(y_n)-f(y_m)|\le2M\|f-f_j\|+|f_j(y_n)-f_j(y_m)|<\epsilon.
$$

Thus $\varphi(f)=\lim_n f(y_n)$ exists for every $f$. Taking limits proves linearity, and $|\varphi(f)|\le M\|f\|$ proves

$$
\boxed{\varphi\in X^{**},\qquad\|\varphi\|\le M.}
$$

This diagonal argument includes the continuity estimate rather than appealing to a sequential compactness theorem.

If $X$ is not reflexive, choose $\Phi\in B_{X^{**}}\setminus JX$, scaling a bidual element outside $JX$ if necessary. The Goldstine theorem proved above supplies $x_n\in B_X$ with $|f_j(x_n)-\Phi(f_j)|<1/n$ for $j\le n$. [Norm](../../../../../norm.md) density and the bound $\|Jx_n-\Phi\|\le2$ extend this convergence to every $f\in X^*$. Hence $Jx_n\to\Phi$ weak-star. Every subsequence has the same coordinate limits, so a weakly convergent subsequence with limit $x\in X$ would give $Jx=\Phi$, a contradiction. This [sequential Goldstine approximation for a separable dual](../../../../../sequential-goldstine-approximation-for-a-separable-dual.md) proves

$$
\boxed{\|x_n\|\le1,\quad(x_n)\text{ has no weakly convergent subsequence in }X.}
$$

The construction uses the Goldstine proof already given, not an unproved weak sequential compactness result.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 106](../../paper-106-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
