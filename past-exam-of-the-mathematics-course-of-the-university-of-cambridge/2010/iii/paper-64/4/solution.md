<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The natural expectation is [orbital stability](../../../../../orbital-stability.md), since a spatial translation of a [travelling wave](../../../../../travelling-wave.md) is another [travelling wave](../../../../../travelling-wave.md). Thus convergence for ordinary perturbations, when it holds, is to a suitably translated front. It also matters which perturbations are allowed in the leading edge: the zero state ahead of this front is linearly unstable, and a sufficiently shallow positive tail can select a different speed. One should not assert [asymptotic stability](../../../../../asymptotic-stability.md) for arbitrary disturbances without a norm and a class of initial data. The requested [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md) calculation is a necessary part of such an analysis, not by itself a complete nonlinear stability proof.

In the moving coordinate $z=x-ct$, write $u(x,t)=w_c(z)+v(z,t)$. Expansion of the reaction term gives

$$
v_t=v_{zz}+cv_z+(k-2w_c)v-v^2.
$$

The first equation to study is its [linearization](../../../../../linearization.md),

$$
v_t=\mathcal Lv,\qquad \mathcal L=\partial_z^2+c\partial_z+k-2w_c(z),
$$

and the associated [eigenvalue](../../../../../eigenvalue.md) equation $\mathcal L\phi=\lambda\phi$. Differentiating the front equation gives $\mathcal Lw_c'=0$, the neutral translation mode whenever it belongs to the chosen function space. Ahead of the front the limiting coefficient is $k$, so in unweighted [L2 space](../../../../../l2-space-is-a-hilbert-space.md) the limiting dispersion relation is $\lambda=-\xi^2+ic\xi+k$: its rightmost real part is positive. An exponential weight penalizes precisely these disturbances ahead of the front.

There is a small functional-analytic correction to the printed definition. Use the complete [exponentially weighted L2 space](../../../../../exponentially-weighted-l2-space.md)

$$
X_\gamma=\{v:e^{\gamma z}v\in L^2(\mathbb R)\},\qquad
\|v\|_\gamma=\|e^{\gamma z}v\|_2.
$$

The additional requirement of unweighted [L2 space](../../../../../l2-space-is-a-hilbert-space.md) membership in the printed set makes that set incomplete under its stated weighted norm. Indeed $v_N=\mathbf1_{[-N,0]}$ belongs to the intersection and is a weighted [Cauchy sequence](../../../../../cauchy-sequence.md), but its weighted limit $\mathbf1_{(-\infty,0]}$ does not belong to unweighted [L2 space](../../../../../l2-space-is-a-hilbert-space.md). The usual [Hilbert space](../../../../../hilbert-space-split.md) for this spectral argument is the completion $X_\gamma$. We use that completion explicitly, rather than treating the intersection as a complete space.

Multiplication $T_\gamma v=e^{\gamma z}v$ is a unitary map from $X_\gamma$ onto [L2 space](../../../../../l2-space-is-a-hilbert-space.md). Take the domain $T_\gamma^{-1}H^2(\mathbb R)$ for $\mathcal L$. The transformed [closed operator](../../../../../closed-linear-operator.md) is

$$
\mathcal L_\gamma=T_\gamma\mathcal LT_\gamma^{-1}
=\partial_z^2+(c-2\gamma)\partial_z+\gamma^2-c\gamma+k-2w_c(z).
$$

This follows from $T_\gamma\partial_zT_\gamma^{-1}=\partial_z-\gamma$. The two limiting constant-coefficient dispersion relations, obtained by the [Fourier transform](../../../../../fourier-transform.md), are

$$
\lambda_{\mathrm{ahead}}(\xi)=-\xi^2+i(c-2\gamma)\xi+\gamma^2-c\gamma+k,
$$



$$
\lambda_{\mathrm{behind}}(\xi)=-\xi^2+i(c-2\gamma)\xi+\gamma^2-c\gamma-k.
$$

In particular the necessary strict leading-edge condition is $\gamma^2-c\gamma+k<0$. For $c>2\sqrt{k}$ this means

$$
\frac{c-\sqrt{c^2-4k}}2<\gamma<\frac{c+\sqrt{c^2-4k}}2.
$$

A particularly convenient choice is

$$
\boxed{\gamma=c/2,\qquad k-c^2/4<0\quad\text{if }c>2\sqrt{k}.}
$$

With this choice there is no first derivative, and $\mathcal L_\gamma=\partial_z^2+k-c^2/4-2w_c(z)$ is a [self-adjoint differential operator](../../../../../self-adjoint-differential-operator.md) on $H^2(\mathbb R)$. This also avoids possible ambiguities between definitions of [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md) for nonnormal operators.

The relevant perturbation theorem is [essential-spectrum invariance under relatively compact perturbations](../../../../../essential-spectrum-invariance-under-relatively-compact-perturbations.md): if $A_0$ is a [closed operator](../../../../../closed-linear-operator.md), $V:D(A_0)\to H$ is compact with respect to the [graph norm](../../../../../graph-norm.md), and $A_0+V$ is closed on the same domain, their Fredholm [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md) is the same. For [self-adjoint](../../../../../self-adjoint-operator.md) operators this is the usual [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md) after removing isolated finite-multiplicity [eigenvalues](../../../../../eigenvalue.md). To see why the theorem applies, regard $A_0-\lambda$ and $A_0+V-\lambda$ as bounded maps from the [graph norm](../../../../../graph-norm.md) domain to $H$, and use [compact perturbation invariance of Fredholm operators](../../../../../compact-perturbation-invariance-of-fredholm-operators.md) for each $\lambda$.

Define a step-potential comparison operator

$$
A_0=\partial_z^2+q_0(z),\qquad
q_0(z)=\begin{cases}-k-c^2/4,&z<0,\\k-c^2/4,&z\geq0.\end{cases}
$$

Both $A_0$ and $\mathcal L_\gamma$ are [self-adjoint](../../../../../self-adjoint-operator.md) on $H^2(\mathbb R)$. Their difference is multiplication by

$$
V(z)=k-c^2/4-2w_c(z)-q_0(z),\qquad V(z)\longrightarrow0\quad(z\to\pm\infty).
$$

It is relatively compact, not necessarily compact as a multiplication map on all of [L2 space](../../../../../l2-space-is-a-hilbert-space.md). To prove the needed compactness, take a sequence bounded in $H^2(\mathbb R)$. On each bounded interval the [Rellich-Kondrachov compactness theorem](../../../../../rellich-kondrachov-theorem.md) gives a subsequence converging in [L2 space](../../../../../l2-space-is-a-hilbert-space.md). A diagonal subsequence makes the products by $V$ converge locally. Outside a sufficiently large interval, $\|V\|_\infty$ is arbitrarily small and the sequence has a uniform [L2 norm](../../../../../l2-norm.md) bound, so those tails are uniformly small. Thus the products converge globally in [L2 space](../../../../../l2-space-is-a-hilbert-space.md), proving graph-domain compactness.

Finally,

$$
\sigma_{\mathrm{ess}}(A_0)=(-\infty,k-c^2/4].
$$

Here is a direct verification. Its quadratic form is at most $(k-c^2/4)\|h\|_2^2$, so no [spectrum](../../../../../spectrum-functional-analysis.md) lies above this endpoint. For every $\lambda\leq k-c^2/4$, choose $\xi$ with $\lambda=k-c^2/4-\xi^2$. Normalized, increasingly long cutoffs of $e^{i\xi z}$, translated far to the right, have disjoint supports and satisfy $\|(A_0-\lambda)h_N\|_2\to0$: differentiating the cutoff gives errors of orders $N^{-1}$ and $N^{-2}$. They converge weakly to zero. This is a singular sequence in the [Weyl criterion](../../../../../weyl-criterion.md), proving that every such $\lambda$ belongs to the [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md). The relatively compact perturbation theorem therefore gives

$$
\boxed{\sigma_{\mathrm{ess}}(\mathcal L\text{ on }X_{c/2})=(-\infty,k-c^2/4].}
$$

This proves the [weighted essential spectrum of a Fisher travelling front](../../../../../weighted-essential-spectrum-of-a-fisher-travelling-front.md) is strictly stable when $c>2\sqrt{k}$. In fact here the quadratic form gives more:

$$
\langle\mathcal L_{c/2}h,h\rangle
=-\|h'\|_2^2+\int(k-c^2/4-2w_c)|h|^2\,dz
\leq-(c^2/4-k)\|h\|_2^2.
$$

Since $w_c\geq0$, the full transformed [spectrum](../../../../../spectrum-functional-analysis.md) lies below $-(c^2/4-k)$, and the evolution given by its [linearization](../../../../../linearization.md) decays at least as $e^{-(c^2/4-k)t}$ in this weighted norm. This does not contradict translation invariance: the nonzero translation mode cannot lie in this weighted operator domain, since otherwise it would be a zero [eigenfunction](../../../../../eigenfunction.md), contradicting the strictly negative quadratic-form bound. The weight restricts the permitted perturbations and excludes these neutral translations. Nor does a weighted [L2 norm](../../../../../l2-norm.md) alone control the nonlinear remainder at $z\to-\infty$; a nonlinear theorem needs further boundedness or regularity assumptions.

At the minimal speed $c_*=2\sqrt{k}$, the best choice is $\gamma=\sqrt{k}$. Now $\gamma^2-c\gamma+k=(\gamma-\sqrt{k})^2$, and

$$
\boxed{\sigma_{\mathrm{ess}}(\mathcal L\text{ on }X_{\sqrt{k}})=(-\infty,0].}
$$

The [essential spectrum](../../../../../essential-spectrum-of-a-closed-operator.md) has no positive part but touches zero; no positive exponential weight makes it strictly negative. Thus the critical front has no spectral gap and this argument gives no exponential decay rate there. **Strict weighted spectral stability holds above the minimal speed; at the minimal speed it is marginal.**

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 64](../../paper-64-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
