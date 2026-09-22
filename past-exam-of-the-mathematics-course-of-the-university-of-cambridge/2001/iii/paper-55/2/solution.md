<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

We prove uniqueness in the sense of **at most one** [Gibbs measure](../../../../../gibbs-measure.md) satisfying the printed [conditional distributions](../../../../../conditional-distribution.md). No shift-invariance assumption is needed in advance. Write a history as $\eta=(\epsilon_{s-1},\epsilon_{s-2},\ldots)$. The variation hypothesis makes $U$ continuous and bounded on the finite-alphabet sequence space; let $u_-\leq U\leq u_+$ and $V=u_+-u_-$. The [conditional distribution](../../../../../conditional-distribution.md) of the first spin, obtained by marginalizing the prescribed two-spin law, must be

$$
q(a\mid\eta)=\frac{\sum_{b\in K}\exp[U(a\eta)+U(ba\eta)]}{\sum_{c,b\in K}\exp[U(c\eta)+U(bc\eta)]}.
$$

In particular $q(a\mid\eta)\geq\delta:=e^{-2V}/k>0$ for every symbol and history. Any two candidate measures have this same time-homogeneous one-step kernel, by conditional marginalization and the tower property.

If $\eta,\eta'$ agree in their most recent $r$ symbols, each two-spin energy in this formula changes by at most

$$
D\lambda^{-r},\qquad D=C(\lambda^{-1}+\lambda^{-2}).
$$

Both numerator and denominator therefore change by factors between $e^{-D\lambda^{-r}}$ and $e^{D\lambda^{-r}}$. Consequently the [total variation distance](../../../../../total-variation-distance.md) of the two kernels is at most $e^{2D\lambda^{-r}}-1\leq B\lambda^{-r}$, where $B=e^{2D}-1$. Uniform positivity also bounds it by $1-k\delta$. Put

$$
b_r=\min(1-k\delta,B\lambda^{-r}).
$$

These bounds are decreasing, strictly below one, and summable. We now give the [summable-memory coupling](../../../../../summable-memory-coupling.md) argument rather than assuming a small one-step contraction coefficient.

Starting from any two histories at a remote time, use a [maximal coupling](../../../../../maximal-coupling.md) of the next-spin laws. If the actual histories have agreed for $r$ consecutive symbols, their probability of disagreement is at most $b_r$. Use shared independent uniform random numbers to construct a dominating match-length process $R$: it increases from $r$ to $r+1$ with probability $1-b_r$ and resets to zero with probability $b_r$. Since $b_r$ decreases, the actual consecutive-match length can be kept at least $R$ at every step. When the dominating process does not reset, the actual spins can be coupled to agree.

A new run from zero has probability

$$
p_*:=\prod_{r=0}^{\infty}(1-b_r)>0
$$

of never resetting. The product is positive because $b_r<1$ and $\sum b_r<\infty$: its tail logarithm converges absolutely, and its finite initial factors are positive. After each reset a fresh run has the same success probability, so the probability of $m$ failed runs is $(1-p_*)^m$. There are almost surely only finitely many resets. Every failed run has finite duration, and thus the time of the final reset is finite almost surely. Its distribution depends only on $(b_r)$, not on the two starting histories. It follows that the probability of any disagreement in a fixed future block tends uniformly to zero as the block's distance from the initial time tends to infinity.

Now take two candidate [Gibbs measures](../../../../../gibbs-measure.md), sample their respective histories before time $-N$, and couple their forward kernels as above. Their finite-block laws really are obtained by these kernels: successive conditional expectations use the common [conditional distribution](../../../../../conditional-distribution.md) $q$. For any fixed coordinate block $[s,t]$, the [coupling inequality for total variation](../../../../../coupling-inequality-for-total-variation.md) bounds the distance between the two candidate block laws by the dominating probability of a reset at or after step $N+s$. That bound tends to zero as $N\to\infty$. Hence all probabilities of finite [cylinder sets](../../../../../cylinder-set.md) agree; [cylinder sets](../../../../../cylinder-set.md) generate the product Borel sigma-algebra, so the measures agree.

Thus **there is at most one measure satisfying these conditional specifications**. There is a separate compatibility issue: for an arbitrary unnormalized [symbolic potential](../../../../../symbolic-potential.md) the finite-horizon [conditional distributions](../../../../../conditional-distribution.md) printed in the question need not be consistent as the right endpoint changes. The argument proves the requested uniqueness whenever such a law exists; it does not silently infer existence from the variation estimate. A normalized one-sided kernel or the usual compatible Gibbs specification supplies the standard existence formulation. For a concrete incompatibility, take two symbols and $U(a,\eta)=\log W_{\eta_1,a}$ with $W=\begin{pmatrix}1&1\\1&2\end{pmatrix}$. This has zero variation once two symbols agree. From a history ending in symbol one, the first-symbol probability obtained from a two-spin block is $2/5$, but from a three-spin block it is $5/13$. Thus the printed finite-horizon specification can indeed have no measure, even though its uniqueness implication remains valid.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 55](../../paper-55-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
