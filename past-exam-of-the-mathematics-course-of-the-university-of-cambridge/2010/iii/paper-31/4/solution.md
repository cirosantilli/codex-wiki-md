<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A real functional $\Phi$ is [Hadamard differentiable](../../../../../hadamard-differentiability.md) at $s_0$ if there exists a continuous linear functional $L=\dot\Phi_{s_0}:S\to\mathbb R$ such that, whenever $t_j\ne0$, $t_j\to0$ and $h_j\to h$ in the [normed vector space](../../../../../normed-vector-space.md),

$$
\boxed{\frac{\Phi(s_0+t_jh_j)-\Phi(s_0)}{t_j}\longrightarrow L(h).}
$$

If $\Phi$ is defined only on a subset, require $s_0+t_jh_j$ to lie in its domain. The variation of the directions $h_j$ is essential: convergence along each fixed direction alone is a weaker differentiability condition. Tangential [Hadamard differentiability](../../../../../hadamard-differentiability.md) restricts the limit directions to a specified subspace; here the derivative is defined on all of $S$.

We prove the [functional delta method](../../../../../functional-delta-method.md) using compact sets, so do not need an unjustified application of the [Skorokhod representation theorem](../../../../../skorokhod-representation-theorem.md) on an arbitrary nonseparable [normed vector space](../../../../../normed-vector-space.md). As usual for function-space [convergence in distribution](../../../../../convergence-in-distribution.md), the limiting random element is tight, and the real statistics are measurable, or convergence is understood through outer expectations. These are automatic under the usual separable complete random-element formulation; the empirical-process formulation used below has a tight separably supported limit.

For $t\ne0$ put

$$
R_t(h)=\frac{\Phi(s_0+th)-\Phi(s_0)}t-L(h).
$$

[Hadamard differentiability](../../../../../hadamard-differentiability.md) says $R_{t_j}(h_j)\to0$ for every convergent sequence of directions, since continuity gives $L(h_j)\to L(h)$. It implies a [Hadamard remainder near a compact set](../../../../../hadamard-remainder-near-a-compact-set.md): for every compact $K\subset S$ and $\epsilon>0$ there are $a>0$ and $\delta>0$ such that

$$
0<|t|<a,\quad\operatorname{dist}(h,K)<\delta\quad\Longrightarrow\quad |R_t(h)|<\epsilon.
$$

To prove it, suppose it failed. Choose $t_j\to0$ and $h_j$ at distance less than $1/j$ from $K$ with $|R_{t_j}(h_j)|\geq\epsilon$. Choose $k_j\in K$ with $\|h_j-k_j\|<2/j$. A subsequence of $k_j$ converges by compactness, so the corresponding $h_j$ converge too. The defining derivative limit contradicts the lower bound on $R_{t_j}(h_j)$.

Now let $Z_n=r_n(X_n-s_0)\xrightarrow d X$ and $t_n=1/r_n$. Given $\eta>0$, [tightness of a probability measure](../../../../../tightness-of-a-probability-measure.md) provides a compact $K$ with $\mathbb P(X\in K)>1-\eta$. For the open $\delta$-neighbourhood $K^\delta$, the [Portmanteau theorem](../../../../../portmanteau-theorem.md) gives

$$
\liminf_n\mathbb P(Z_n\in K^\delta)\geq\mathbb P(X\in K^\delta)>1-\eta.
$$

On $K^\delta$ the preceding uniform remainder is less than $\epsilon$ for all sufficiently large $n$. Consequently $\limsup_n\mathbb P(|R_{t_n}(Z_n)|\geq\epsilon)\leq\eta$. Since $\eta$ is arbitrary, this remainder tends to zero in [probability](../../../../../probability.md). We have proved the actual expansion

$$
r_n\bigl(\Phi(X_n)-\Phi(s_0)\bigr)=L(Z_n)+o_{\mathbb P}(1).
$$

Continuity of $L$ and the [continuous mapping theorem](../../../../../continuous-mapping-theorem.md) give $L(Z_n)\xrightarrow d L(X)$. The vanishing remainder and [Slutsky theorem](../../../../../slutsky-theorem.md) therefore yield

$$
\boxed{r_n\bigl(\Phi(X_n)-\Phi(s_0)\bigr)\xrightarrow d\dot\Phi_{s_0}(X).}
$$

This derivation uses the derivative definition, rather than assuming a uniform Fréchet remainder over every bounded set. If outer expectations are needed, the same compact-neighbourhood argument uses outer probabilities and gives the corresponding empirical-process [functional delta method](../../../../../functional-delta-method.md).

For the statistical application, use the sample's [empirical distribution function](../../../../../empirical-distribution-function.md) and the plug-in estimator

$$
\boxed{T_n=\Phi(F_n).}
$$

Here the printed $L^\infty$ denotes bounded pointwise functions with the [supremum norm](../../../../../supremum-norm.md), namely $\ell^\infty(\mathbb R)$, rather than equivalence classes modulo Lebesgue null sets. Assume [Hadamard differentiability](../../../../../hadamard-differentiability.md) at the true $F$ and the usual measurability of the scalar estimator. The [Donsker theorem for empirical distribution functions](../../../../../donsker-theorem-for-empirical-distribution-functions.md) and the proved [functional delta method](../../../../../functional-delta-method.md) give

$$
\boxed{\sqrt n\bigl(T_n-\Phi(F)\bigr)\xrightarrow d Z_F:=\dot\Phi_F(\mathbb G_F).}
$$

No continuity of $F$ is needed for this application. Since the derivative is continuous and linear and the bridge is a centred [Gaussian process](../../../../../gaussian-process.md), $Z_F$ is a centred Gaussian real random variable, possibly identically zero.

Finally, a finite real weak limit ensures the required [boundedness in probability](../../../../../boundedness-in-probability.md). Choose $M$ so large that $\mathbb P(|Z_F|\geq M)<\epsilon/2$. Applying the closed-set part of the [Portmanteau theorem](../../../../../portmanteau-theorem.md) to $\{z:|z|\geq M\}$ gives

$$
\limsup_n\mathbb P\!\left(\left|\sqrt n(T_n-\Phi(F))\right|\geq M\right)\leq\mathbb P(|Z_F|\geq M)<\epsilon/2.
$$

Hence there is $n_0$ such that, for every $n\geq n_0$,

$$
\boxed{\mathbb P\!\left(\left|\sqrt n(T_n-\Phi(F))\right|<M\right)>1-\epsilon.}
$$

In particular the upper-tail condition in the question holds. The plug-in estimator has estimation error $O_{\mathbb P}(n^{-1/2})$, even when its limiting variance is zero.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
