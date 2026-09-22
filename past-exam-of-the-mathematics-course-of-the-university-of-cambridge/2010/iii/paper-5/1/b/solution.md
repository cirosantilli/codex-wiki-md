<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The relevant [Banach-Alaoglu theorem](../../../../../../banach-alaoglu-theorem.md) says that for $1<p<\infty$ the closed bounded balls of $L^p(\mathbb R^n)$ are compact in the [weak topology](../../../../../../weak-topology-split.md). In particular, every bounded sequence has a weakly convergent subsequence whose limit has [norm](../../../../../../norm.md) no larger than the common bound. Applying the preceding [duality of Lp spaces](../../../../../../duality-of-lp-spaces.md) also identifies this as weak-star compactness of $L^p=(L^q)^*$; its weak and weak-star test spaces are both $L^q$.

Here is a direct proof of both compactness and the subsequence assertion. Let $\|f_j\|_p\leq M$ and choose a countable dense set $\{g_m\}$ in the separable [Lp space](../../../../../../lp-space.md) $L^q$. Each scalar sequence $\int f_jg_m$ is bounded. Successive subsequence selection followed by the [diagonal subsequence argument](../../../../../../diagonal-subsequence-argument.md) gives $f_{j_k}$ for which these pairings converge for every $m$. For arbitrary $g\in L^q$,

$$
\left|\int(f_{j_k}-f_{j_l})g\right|\leq2M\|g-g_m\|_q+\left|\int(f_{j_k}-f_{j_l})g_m\right|.
$$

First approximate $g$ by $g_m$ and then take $k,l$ large. This proves convergence of every pairing, and the limit $\Lambda(g)=\lim_k\int f_{j_k}g$ is linear with $|\Lambda(g)|\leq M\|g\|_q$. Apply the already proved [duality of Lp spaces](../../../../../../duality-of-lp-spaces.md) with $q$ in place of $p$: $\Lambda(g)=\int fg$ for an $f\in L^p$ with $\|f\|_p\leq M$. Thus

$$
\boxed{f_{j_k}\rightharpoonup f\text{ in }L^p,\qquad \|f\|_p\leq M.}
$$

To obtain compactness rather than only a sequential statement, on the radius-$M$ ball define

$$
d(f,h)=\sum_{m=1}^{\infty}2^{-m}\frac{|\int(f-h)g_m|}{1+|\int(f-h)g_m|}.
$$

Density and [Hölder's inequality](../../../../../../holder-s-inequality.md) show that this is a [metric space](../../../../../../metric-space.md) distance and that its topology is exactly the [weak topology](../../../../../../weak-topology-split.md) on this ball: every remaining test pairing is uniformly approximated there by a dense-set pairing. The subsequence argument proves sequential compactness for this metric. A sequentially compact [metric space](../../../../../../metric-space.md) is compact: otherwise either an infinite separated sequence contradicts [total boundedness](../../../../../../totally-bounded-space.md) or a Cauchy sequence without a limit contradicts sequential compactness; completeness and [total boundedness](../../../../../../totally-bounded-space.md) give compactness by successive finite coverings. This completes the proof. The same argument is the [Sequential Banach-Alaoglu theorem for a separable predual](../../../../../../sequential-banach-alaoglu-theorem-for-a-separable-predual.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
