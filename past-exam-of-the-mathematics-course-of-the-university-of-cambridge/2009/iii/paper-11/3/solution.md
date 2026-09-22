<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The prescribed-pole form of [Runge theorem](../../../../../runge-s-theorem.md) is as follows. Let $K\subset\mathbb C$ be [compact](../../../../../compact-space.md), let $f$ be [holomorphic](../../../../../complex-differentiability-at-a-point.md) on a [neighborhood](../../../../../neighbourhood-mathematics.md) of $K$, and let $S\subset\widehat{\mathbb C}\setminus K$ meet every [connected component](../../../../../connected-component.md) of that complement. Then, for every $\epsilon>0$, there is a [rational function](../../../../../rational-function.md) $R$, all of whose [poles](../../../../../pole.md) belong to $S$, with $\sup_K|f-R|<\epsilon$. A [pole](../../../../../pole.md) at infinity means a [polynomial](../../../../../polynomial-split.md) part is allowed. In particular, if the complement is [connected](../../../../../connected-space.md), choose $S=\{\infty\}$ and obtain the [polynomial Runge theorem](../../../../../polynomial-runge-theorem.md).

First approximate using [poles](../../../../../pole.md) anywhere off $K$. Choose a bounded polygonal [neighborhood](../../../../../neighbourhood-mathematics.md) $V$ of $K$ whose closure lies in the [neighborhood](../../../../../neighbourhood-mathematics.md) on which $f$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md), and whose boundary is disjoint from $K$. Such a $V$ comes from a sufficiently fine finite grid covering a small closed [neighborhood](../../../../../neighbourhood-mathematics.md) of $K$. Orient the outer boundary positively and boundaries of holes negatively. The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) gives

$$
f(z)=\frac1{2\pi i}\int_{\partial V}\frac{f(\zeta)}{\zeta-z}\,d\zeta,\qquad z\in K.
$$

Because $\partial V$ and $K$ have positive distance, the integrand is [uniformly continuous](../../../../../uniform-continuity.md) on their product, separately along each boundary edge. Its [Riemann sums](../../../../../riemann-sum.md) converge uniformly for $z\in K$. Those sums are [rational functions](../../../../../rational-function.md) $\sum_jc_j/(\zeta_j-z)$ with [poles](../../../../../pole.md) $\zeta_j\notin K$. Thus arbitrary exterior [poles](../../../../../pole.md) suffice.

To move them to the prescribed set, let $A$ be the uniform closure on $K$ of [rational functions](../../../../../rational-function.md) with [poles](../../../../../pole.md) only in $S$. It is a closed unital algebra; it contains the coordinate function when $\infty\in S$. Define

$$
E=\{a\in\mathbb C\setminus K:(z-a)^{-1}\in A\}.
$$

This set is open relative to $\mathbb C\setminus K$. Indeed, if $a\in E$ and $|b-a|<\operatorname{dist}(a,K)$, the uniformly convergent expansion

$$
\frac1{z-b}=\sum_{j=0}^{\infty}\frac{(b-a)^j}{(z-a)^{j+1}}
$$

places the new reciprocal in $A$, using its algebra and closedness properties. It is also relatively closed: if $a_m\in E$ tends to $a\notin K$, then $(z-a_m)^{-1}$ tends uniformly on $K$ to $(z-a)^{-1}$. Each bounded component contains a finite selected [pole](../../../../../pole.md) and hence meets $E$. The unbounded component also meets $E$ if it contains a finite selected [pole](../../../../../pole.md); if its selected [pole](../../../../../pole.md) is infinity, take $|a|>\sup_K|z|$ and use

$$
\frac1{z-a}=-\frac1a\sum_{j=0}^{\infty}\left(\frac za\right)^j,
$$

a uniform [polynomial](../../../../../polynomial-split.md) expansion. Being both open and closed and meeting every component, $E$ is all of $\mathbb C\setminus K$. Every initial Cauchy-sum reciprocal therefore belongs to $A$, and so does $f$. This proves [Runge theorem](../../../../../runge-s-theorem.md), including its prescribed-pole assertion, rather than merely [polynomial](../../../../../polynomial-split.md) approximation on a special [compact set](../../../../../compact-space.md).

For the requested [pointwise polynomial approximation of a half-plane sign](../../../../../pointwise-polynomial-approximation-of-a-half-plane-sign.md), take $n\ge2$ and

$$
K_n^+=\{x+iy:|x|\le n,\ 1/n\le y\le n\},\qquad
K_n^0=[-n,n],\qquad K_n^-=\{x+iy:|x|\le n,\ -n\le y\le-1/n\},
$$

These three [compact sets](../../../../../compact-space.md) are disjoint, and their union $K_n$ has [connected](../../../../../connected-space.md) complement: there are horizontal gaps above and below the segment, and every complementary point can be joined through these gaps or around a rectangle to the exterior of $[-n,n]^2$. Define $h_n$ to be $1,0,-1$ on disjoint open [neighborhoods](../../../../../neighbourhood-mathematics.md) of these three sets. It is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on their union. By the [polynomial Runge theorem](../../../../../polynomial-runge-theorem.md), choose $P_n$ with $\sup_{K_n}|P_n-h_n|<1/n$.

For every fixed point with positive imaginary part, both coordinate bounds and $1/n\le\operatorname{Im}z$ eventually hold, so it lies in $K_n^+$ for all large $n$; the reflected assertion holds for negative imaginary part. Every real point eventually lies in $K_n^0$. Consequently

$$
\boxed{\lim_{n\to\infty}P_n(z)=\operatorname{sgn}(\operatorname{Im}z),\quad\operatorname{sgn}(0)=0.}
$$

The discontinuity of the limit does not contradict holomorphicity of the approximating functions: this convergence is pointwise, and is not locally uniform near the real axis.

Finally, identify $K^*$ as the [holomorphic convex hull](../../../../../holomorphic-convex-hull.md) relative to $\Omega$. If $U$ is a component of $\widehat{\mathbb C}\setminus K$ lying entirely in $\Omega$, it cannot contain infinity and is bounded. Its boundary lies in $K$, and its closure is [compact](../../../../../compact-space.md) in $\Omega$. For any [holomorphic](../../../../../complex-differentiability-at-a-point.md) $f$ on $\Omega$, the [maximum modulus principle](../../../../../maximum-modulus-principle.md) on $U$ gives $|f(w)|\le\sup_{\partial U}|f|\le\sup_K|f|$. Thus $U\subseteq K^*$, as is $K$ itself.

Conversely let $w\in\Omega\setminus K$ lie in a complementary component $U$ that is not entirely in $\Omega$. If it contains a finite point $a\notin\Omega$, form the [uniform algebra](../../../../../uniform-algebra.md) on $K$ generated by constants and $(z-a)^{-1}$. The same open-and-closed reciprocal argument above, now only on the [connected component](../../../../../connected-component.md) $U$, shows that $(z-w)^{-1}$ is in its uniform closure. Its approximants have [poles](../../../../../pole.md) only at $a$ and are [holomorphic](../../../../../complex-differentiability-at-a-point.md) on $\Omega$. If the available point outside $\Omega$ is infinity, use the [polynomial](../../../../../polynomial-split.md) algebra and its large-pole expansion instead. Hence in either case choose $h\in\mathcal O(\Omega)$ with

$$
\sup_{z\in K}\left|\frac1{z-w}-h(z)\right|<\frac1{2\max_{z\in K}|z-w|}.
$$

The function $F(z)=1-(z-w)h(z)$ is [holomorphic](../../../../../complex-differentiability-at-a-point.md) on $\Omega$, has $F(w)=1$, and satisfies $\sup_K|F|<1/2$. It separates $w$ from the hull, so $w\notin K^*$. Combining the two inclusions proves

$$
\boxed{K^*=K\ \cup\!\!\bigcup_{\substack{U\text{ component of }\widehat{\mathbb C}\setminus K\\U\subset\Omega}}U.}
$$

Here $\mathbb P$ denotes the [Riemann sphere](../../../../../riemann-sphere.md); using it ensures that the unbounded component, which contains infinity, is not accidentally filled. The empty [compact set](../../../../../compact-space.md) has empty hull by the usual convention; the separation argument above concerns nonempty $K$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
