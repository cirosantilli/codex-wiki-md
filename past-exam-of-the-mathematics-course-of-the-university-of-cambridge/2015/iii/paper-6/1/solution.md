<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For $1\leq p<\infty$, the real [Lp space](../../../../../lp-space.md) is the [vector space](../../../../../vector-space-split.md) of real [measurable functions](../../../../../measurable-function.md) with $\int_\Omega|f|^p\,d\mu<\infty$, identifying functions equal [almost everywhere](../../../../../almost-everywhere.md). Its [Lp norm](../../../../../lp-norm.md) is $\|f\|_p=(\int|f|^p\,d\mu)^{1/p}$. For $p=\infty$, take the essentially bounded real [measurable functions](../../../../../measurable-function.md), with the same identification and [norm](../../../../../norm.md) $\|f\|_\infty=\operatorname{ess\,sup}|f|$. The identification makes each [norm](../../../../../norm.md) definite; absolute homogeneity follows from the [Lebesgue integral](../../../../../lebesgue-integral.md), and the [triangle inequality](../../../../../triangle-inequality.md) follows from [Minkowski inequality](../../../../../minkowski-inequality.md) for finite $p$, or directly from the [essential supremum](../../../../../essential-supremum.md) for $p=\infty$.

Here is a [completeness](../../../../../completeness.md) proof valid on any [measure space](../../../../../measure-space.md). For $p<\infty$, a [Cauchy sequence](../../../../../cauchy-sequence.md) $(f_n)$ has a [subsequence](../../../../../subsequence.md) $(f_{n_k})$ with $\|f_{n_{k+1}}-f_{n_k}\|_p\leq2^{-k}$. Choose [measurable function](../../../../../measurable-function.md) representatives and put $h_k=f_{n_{k+1}}-f_{n_k}$. By [Minkowski inequality](../../../../../minkowski-inequality.md) and the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md),

$$
\left\|\sum_{k=1}^N|h_k|\right\|_p\leq\sum_{k=1}^N2^{-k}\leq1,
\qquad
\int\left(\sum_{k=1}^\infty|h_k|\right)^p\,d\mu\leq1.
$$

Consequently the [series](../../../../../series-mathematics.md) $\sum h_k$ converges absolutely [almost everywhere](../../../../../almost-everywhere.md). Define $f=f_{n_1}+\sum h_k$ there, and define it to be zero on the measurable exceptional null set. Then $f\in L^p$, and [Fatou lemma](../../../../../fatou-s-lemma.md) applied to each tail gives $\|f-f_{n_k}\|_p\leq\sum_{j=k}^\infty2^{-j}\to0$. The original [Cauchy sequence](../../../../../cauchy-sequence.md) also converges in [Lp norm](../../../../../lp-norm.md), by the [triangle inequality](../../../../../triangle-inequality.md). For $p=\infty$, choose the same [subsequence](../../../../../subsequence.md) using the [essential supremum](../../../../../essential-supremum.md) [norm](../../../../../norm.md). Outside one measurable null set, all the bounds $|h_k|\leq2^{-k}$ hold and $f_{n_1}$ is bounded. The [series](../../../../../series-mathematics.md) then converges uniformly there, with an essentially bounded [measurable function](../../../../../measurable-function.md) limit and the same tail estimate in [essential supremum](../../../../../essential-supremum.md) [norm](../../../../../norm.md). Thus **all these spaces are [Banach spaces](../../../../../banach-space-split.md)**.

The [duality of Lp spaces](../../../../../duality-of-lp-spaces.md) says that, for $1<p<\infty$ and $q=p/(p-1)$, the map

$$
I_p:L^q\longrightarrow(L^p)^*,\qquad (I_pg)(f)=\int fg\,d\mu
$$

is an [isometric isomorphism of normed spaces](../../../../../isometric-isomorphism-of-normed-spaces.md). This form of [Lp duality on an arbitrary measure space](../../../../../lp-duality-on-an-arbitrary-measure-space.md) requires no finiteness hypothesis on $\mu$. At $p=1$, a standard version assumes a [sigma-finite measure](../../../../../sigma-finite-measure.md) and identifies $(L^1)^*$ with $L^\infty$ through the same [dual pairing](../../../../../dual-pairing.md). That endpoint assertion must not be made without a suitable measure-space hypothesis.

We first prove the required [duality of Lp spaces](../../../../../duality-of-lp-spaces.md) for a [finite measure](../../../../../finite-measure.md). Let $F\in(L^p)^*$ and set $\nu(E)=F(\mathbf1_E)$. For disjoint measurable $E_j$, the [indicator functions](../../../../../indicator-function.md) of their partial unions converge in [Lp norm](../../../../../lp-norm.md) to that of their union, so $\nu$ is countably additive. It has finite [variation measure](../../../../../variation-measure.md): for every finite measurable partition $(E_j)$, choosing real signs gives

$$
\sum_j|\nu(E_j)|=F\left(\sum_j\operatorname{sgn}(\nu(E_j))\mathbf1_{E_j}\right)
\leq\|F\|\mu(\Omega)^{1/p}.
$$

Also $\mu(E)=0$ implies $\nu(E)=0$. The [Radon-Nikodym theorem](../../../../../radon-nikodym-theorem.md) supplies a [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md) $g\in L^1$ with $\nu(E)=\int_Eg\,d\mu$. Linearity gives $F(f)=\int fg\,d\mu$ for [simple functions](../../../../../simple-function.md). Uniform approximation by [simple functions](../../../../../simple-function.md) extends this identity to bounded [measurable functions](../../../../../measurable-function.md): both their [Lp norm](../../../../../lp-norm.md) errors and the errors in integration against $g$ tend to zero.

To establish the correct [integrability](../../../../../integrability.md), test with the bounded [measurable function](../../../../../measurable-function.md) $f_N=\operatorname{sgn}(g)|g|^{q-1}\mathbf1_{\{|g|\leq N\}}$. Since $(q-1)p=q$, writing $A_N=\int_{\{|g|\leq N\}}|g|^q\,d\mu$ gives

$$
A_N=F(f_N)\leq\|F\|A_N^{1/p},\qquad A_N^{1/q}\leq\|F\|.
$$

The second inequality is also valid when $A_N=0$. The [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives $g\in L^q$ and $\|g\|_q\leq\|F\|$. Density of [simple functions](../../../../../simple-function.md) in the [Lp space](../../../../../lp-space.md), together with [Hölder's inequality](../../../../../holder-s-inequality.md), now gives $F=I_pg$ on all of $L^p$. Conversely [Hölder's inequality](../../../../../holder-s-inequality.md) gives $\|I_pg\|\leq\|g\|_q$. If $g\ne0$, testing against

$$
f=\frac{\operatorname{sgn}(g)|g|^{q-1}}{\|g\|_q^{q-1}}
$$

gives $\|f\|_p=1$ and $(I_pg)(f)=\|g\|_q$, so **$\boxed{\|I_pg\|=\|g\|_q}$**. This also proves uniqueness of the representing [Radon-Nikodym derivative](../../../../../radon-nikodym-derivative.md).

For completeness, the passage to an arbitrary [measure space](../../../../../measure-space.md) can be made without losing a hypothesis in the [reflexive Banach space](../../../../../reflexive-banach-space.md) argument below. On a [sigma-finite measure](../../../../../sigma-finite-measure.md) space, exhaust by nested finite-measure sets $E_n$. The representing [Radon-Nikodym derivatives](../../../../../radon-nikodym-derivative.md) on $E_n$ agree on overlaps by uniqueness. Their glued density has [Lp norm](../../../../../lp-norm.md) $\|g\|_q\leq\|F\|$ by the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), and represents $F$ because $f\mathbf1_{E_n}\to f$ in [Lp norm](../../../../../lp-norm.md). Every $f\in L^p$ on an arbitrary [measure space](../../../../../measure-space.md) is supported on a sigma-finite measurable set: the sets $\{|f|>1/n\}$ have finite measure and their union is $\{f\ne0\}$.

Use [support localization of an Lp functional](../../../../../support-localization-of-an-lp-functional.md) as follows. For a sigma-finite measurable $A$, let $m_A$ be the [operator norm](../../../../../operator-norm.md) of $F$ restricted to functions supported in $A$. The support observation gives $\sup_A m_A=\|F\|$. Choose $A_n$ approaching this supremum and set $A=\bigcup_nA_n$; then $m_A=\|F\|$. If a sigma-finite $B\subseteq\Omega\setminus A$ had $m_B=\beta>0$, functions supported on the disjoint sets $A,B$ have the direct-sum [Lp norm](../../../../../lp-norm.md). Optimizing their two scalar coefficients by [Hölder's inequality](../../../../../holder-s-inequality.md), and using functions approaching the two restriction [operator norms](../../../../../operator-norm.md), would give

$$
\|F\|\geq(m_A^q+\beta^q)^{1/q}>m_A,
$$

a contradiction. Thus $F$ vanishes on functions supported outside $A$. The density on $A$, extended by zero, represents $F$ globally. The case $F=0$ simply uses $g=0$. This proves the stated [Lp duality on an arbitrary measure space](../../../../../lp-duality-on-an-arbitrary-measure-space.md).

Finally let $X=L^p$ and let $\Phi\in X^{**}$, where stars denote [continuous dual spaces](../../../../../continuous-dual-space-split.md). Compose with $I_p$ to obtain the [bounded linear functional](../../../../../continuous-linear-functional.md) $g\mapsto\Phi(I_pg)$ on $L^q$. Applying [duality of Lp spaces](../../../../../duality-of-lp-spaces.md) with the exponents reversed gives $f\in L^p$ with $\Phi(I_pg)=\int fg\,d\mu$. For the [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md) $J_Xf$, its value on $I_pg$ is also $\int fg\,d\mu$. Since $I_p$ is onto, $\Phi=J_Xf$. Its [norm](../../../../../norm.md) is $\|f\|_p$ by the same [dual pairing](../../../../../dual-pairing.md) [norm](../../../../../norm.md) identity. Therefore **$\boxed{J_X(L^p)=(L^p)^{**}}$**, which proves that $L^p$ is a [reflexive Banach space](../../../../../reflexive-banach-space.md) through its actual [canonical embedding into the bidual](../../../../../canonical-embedding-into-the-bidual.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
