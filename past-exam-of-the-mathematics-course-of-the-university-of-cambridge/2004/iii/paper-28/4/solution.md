<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Here is the one-parameter [Kolmogorov continuity theorem](../../../../../kolmogorov-continuity-theorem.md). Suppose a real-valued [stochastic process](../../../../../stochastic-process-split.md) on $[0,1]$ satisfies, for some $p>0$, $q>0$ and finite $C$,

$$
\mathbb E|X_t-X_s|^p\leq C|t-s|^{1+q},\qquad s,t\in[0,1].
$$

Then it has a [continuous](../../../../../continuous-function.md) [modification of a stochastic process](../../../../../modification-of-a-stochastic-process.md) whose paths are [Hölder continuous](../../../../../holder-condition.md) of every positive exponent $\gamma<q/p$. A modification [means](../../../../../expected-value.md) equality [almost surely](../../../../../almost-sure-convergence.md) at each fixed time, not an a priori simultaneous equality at all times. Other compact time intervals follow by rescaling; the vector-valued version uses a [norm](../../../../../norm.md) in place of absolute value.

For the proof fix $0<\gamma<q/p$ and use the dyadic grids $D_n=\{j2^{-n}:0\leq j\leq2^n\}$. Let $D_n^*$ be the largest adjacent increment on this grid. The [union bound](../../../../../boole-s-inequality.md) and [Markov inequality](../../../../../markov-inequality.md) give

$$
\mathbb P(D_n^*>2^{-n\gamma})
\leq\sum_{j=0}^{2^n-1}2^{n\gamma p}
\mathbb E|X_{(j+1)2^{-n}}-X_{j2^{-n}}|^p
\leq C2^{-n(q-p\gamma)}.
$$

The right-hand side is summable. The [Borel-Cantelli first lemma](../../../../../borel-cantelli-first-lemma.md) shows that, outside a [null set](../../../../../null-set.md), an almost-surely finite random constant $K$ can absorb the finitely many early grids so that

$$
D_n^*\leq K2^{-n\gamma}\quad\text{for every }n.
$$

We now use [dyadic increment chaining](../../../../../dyadic-increment-chaining.md). For two distinct dyadic points $s,t$, choose $n$ with $2^{-(n+1)}<|t-s|\leq2^{-n}$. Approximate them from below by $s_j,t_j\in D_j$, for $j\geq n$. Each refinement moves by zero or one grid step, while $s_n,t_n$ are at most two grid steps apart. The sequences eventually equal the original dyadic points. Telescoping gives

$$
|X_t-X_s|
\leq 2K2^{-n\gamma}+2K\sum_{j=n+1}^{\infty}2^{-j\gamma}
\leq C_\gamma K|t-s|^\gamma,
$$

where a deterministic finite $C_\gamma$ absorbs the [geometric series](../../../../../geometric-series.md) and $2^{-n}<2|t-s|$. Thus the sample function on the [dense](../../../../../dense-set.md) union of dyadic grids has a unique Hölder-continuous extension to $[0,1]$. Define this extension to be $\widetilde X$ on the probability-one event, and set it to zero on the exceptional [null set](../../../../../null-set.md).

For a fixed $t$, take dyadic $t_j\to t$. The moment condition gives $X_{t_j}\to X_t$ in probability, while the constructed extension gives $X_{t_j}\to\widetilde X_t$ [almost surely](../../../../../almost-sure-convergence.md). Uniqueness of a probability limit yields $\widetilde X_t=X_t$ [almost surely](../../../../../almost-sure-convergence.md). This proves the required modification property. Performing the argument for a [countable](../../../../../countable-set.md) increasing sequence of exponents tending to $q/p$ gives one version with all smaller positive [Hölder exponents](../../../../../holder-exponent.md), since its extensions agree on the dyadic points.

For [Brownian motion](../../../../../brownian-motion-split.md), [Gaussian](../../../../../normal-distribution.md) increments give, for any integer $r\geq2$,

$$
\mathbb E|B_t-B_s|^{2r}=(2r-1)!!\,|t-s|^r.
$$

Use $p=2r$ and $q=r-1$. The theorem gives every exponent $\alpha<(r-1)/(2r)=1/2-1/(2r)$. For any $0<\alpha<1/2$, choose $r$ large enough. Intersect probability-one events over integer $r$ and compact intervals $[0,N]$ to obtain

$$
\boxed{\text{Brownian paths are locally Hölder continuous of every exponent }0<\alpha<\tfrac12\text{ almost surely}.}
$$

The usual [continuous](../../../../../continuous-function.md) Brownian version has the same property: its [continuous](../../../../../continuous-function.md) paths agree with the constructed version on a [countable](../../../../../countable-set.md) [dense](../../../../../dense-set.md) set and hence everywhere, outside one [null set](../../../../../null-set.md). The Hölder constant depends on the compact interval. This is the precise local meaning of [Brownian Hölder regularity](../../../../../brownian-holder-regularity.md); it is not a uniform Hölder bound on the entire unbounded time axis.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 28](../../paper-28-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
