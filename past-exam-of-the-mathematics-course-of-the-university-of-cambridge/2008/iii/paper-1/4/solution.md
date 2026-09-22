<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For a discrete [group](../../../../../group-split.md), one standard definition of amenability is the fixed-point property: every continuous affine action on a nonempty compact [convex set](../../../../../convex-set.md) in a locally convex space has a fixed point. The equivalent state formulation, which may be stated without proof here, is that there is a left-invariant [invariant mean](../../../../../invariant-mean.md) on $\ell^\infty(\Gamma)$. Equivalently, every [unital](../../../../../unital-algebra.md) left-translation-invariant [star-subalgebra](../../../../../star-subalgebra.md) of $\ell^\infty(\Gamma)$ admits a left-invariant state, with [continuity](../../../../../continuous-function.md) for the supremum [norm](../../../../../norm.md); one may equally pass to its [norm](../../../../../norm.md) [closure](../../../../../closure-topology.md). A state means a positive [linear functional](../../../../../linear-functional.md) of [norm](../../../../../norm.md) one with value one on the constant function one. Restriction proves the [subalgebra](../../../../../subalgebra.md) formulation from the full-algebra version, and taking the full algebra proves the converse. Such a mean is finitely additive on [indicator functions](../../../../../indicator-function.md), not necessarily countably additive.

Write $(\lambda(g)\mu)(h)=\mu(g^{-1}h)$ on $\ell^1(\Gamma)$ and $(L_gf)(h)=f(g^{-1}h)$ on bounded functions. We prove equivalence of this mean condition, the [Reiter condition](../../../../../reiter-condition.md), and existence of a [Følner sequence](../../../../../folner-sequence.md).

Assume first that an [invariant mean](../../../../../invariant-mean.md) $m$ exists. Fix a finite set $K\subseteq\Gamma$. In the real [Banach space](../../../../../banach-space-split.md) $\bigoplus_{g\in K}\ell^1(\Gamma)$ with sum [norm](../../../../../norm.md), consider the [convex set](../../../../../convex-set.md)

$$
\mathcal C=\{(\lambda(g)\mu-\mu)_{g\in K}:\mu\text{ a finitely supported probability measure}\}.
$$

If zero were outside its [norm](../../../../../norm.md) [closure](../../../../../closure-topology.md), the [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) would give bounded real functions $f_g$ and $\delta>0$ such that

$$
\sum_{g\in K}\sum_h f_g(h)[(\lambda(g)\mu)(h)-\mu(h)]\geq\delta
$$

for every such $\mu$. Testing point masses at $h$ shows

$$
\sum_{g\in K}[f_g(gh)-f_g(h)]\geq\delta\quad\text{for every }h.
$$

Applying the positive [invariant mean](../../../../../invariant-mean.md) makes the left side zero and the right side at least $\delta$, a contradiction. Therefore zero is in the [closure](../../../../../closure-topology.md): for any $\varepsilon>0$ a finitely supported [probability measure](../../../../../probability-measure.md) makes the sum of the translation defects over $K$ less than $\varepsilon$. Enumerate the countable [group](../../../../../group-split.md), take the first $n$ elements for $K$ and $\varepsilon=1/n$, and obtain a sequence satisfying the [Reiter condition](../../../../../reiter-condition.md). This proves (1) implies (2).

Next assume (2). An $\ell^1$ [probability measure](../../../../../probability-measure.md) can be approximated in [norm](../../../../../norm.md) by finitely supported [probability measures](../../../../../probability-measure.md), by restricting to a large finite set and renormalizing. Replacing $\mu$ by $\nu$ changes each defect by at most $2\|\mu-\nu\|_1$. Thus simultaneous small defects for finitely many translations can be achieved with finite support.

For such $\nu$, set $F_t=\{h:\nu(h)>t\}$. The elementary identity $|r-s|=\int_0^\infty|1_{r>t}-1_{s>t}|\,dt$ for $r,s\geq0$ gives

$$
\int_0^\infty|F_t|\,dt=1,\qquad
\int_0^\infty|F_t\mathbin\triangle gF_t|\,dt
=\|\lambda(g)\nu-\nu\|_1.
$$

If the sum of defects over $K$ is less than $\varepsilon$, some $t$ with $F_t\ne\varnothing$ must satisfy $\sum_{g\in K}|F_t\triangle gF_t|<\varepsilon|F_t|$; otherwise integration would contradict that strict inequality. Applying this [layer-cake extraction of Følner sets](../../../../../layer-cake-extraction-of-folner-sets.md) to successive finite sets of translations gives nonempty finite $F_n$ with each relative boundary tending to zero. Hence (2) implies (3).

Conversely, normalized counting measures $\mu_n=1_{F_n}/|F_n|$ satisfy

$$
\|\lambda(g)\mu_n-\mu_n\|_1=\frac{|gF_n\triangle F_n|}{|F_n|},
$$

so (3) implies (2). Finally, from (2) define states $m_n(f)=\sum_h\mu_n(h)f(h)$. The dual [unit ball](../../../../../unit-ball.md) of $\ell^\infty(\Gamma)$ is weak-star compact by the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md); take a convergent subnet, since this [compactness](../../../../../compact-space.md) need not be metrizable. Its limit $m$ is positive with $m(1)=1$, and

$$
|m_n(L_gf)-m_n(f)|\leq\|f\|_\infty\|\lambda(g^{-1})\mu_n-\mu_n\|_1\longrightarrow0.
$$

Thus $m$ is invariant, proving (2) implies (1). Together these implications establish all three equivalences. Countability is used to obtain sequences from finite tests; it is not a justification for replacing the [compactness](../../../../../compact-space.md) subnet by a subsequence.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
