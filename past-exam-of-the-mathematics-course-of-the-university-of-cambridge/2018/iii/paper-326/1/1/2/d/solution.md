<h1 id="1/1/2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [direct method in the calculus of variations](../../../../../../../../direct-method-in-the-calculus-of-variations.md) gives the following existence theorem. Suppose bounded sequences in the [Banach space](../../../../../../../../banach-space-split.md) $\mathcal U$ have $\tau$-[convergent subsequences](../../../../../../../../convergent-subsequence.md), and $E$ is a [proper extended-real function](../../../../../../../../proper-extended-real-function.md) with [coercivity](../../../../../../../../coercive-function.md) and is $\tau$-[sequentially lower semicontinuous](../../../../../../../../sequential-lower-semicontinuity.md). Then **$E$ has a finite-valued [global minimizer](../../../../../../../../global-minimizer.md)**.

To prove this, properness makes $m=\inf E<+\infty$. First rule out $m=-\infty$: a sequence with $E(u_n)\to-\infty$ eventually lies in a fixed [sublevel set](../../../../../../../../sublevel-set.md), which is bounded by [coercivity](../../../../../../../../coercive-function.md). A $\tau$-[convergent subsequence](../../../../../../../../convergent-subsequence.md) would then have a limit $u$ with $E(u)\leq-\infty$, contradicting the codomain. Hence $m$ is finite.

Choose a [minimizing sequence](../../../../../../../../minimizing-sequence.md) with $E(u_n)\to m$. It eventually belongs to the bounded [sublevel set](../../../../../../../../sublevel-set.md) $\{E\leq m+1\}$. Extract $u_{n_j}\xrightarrow{\tau}\bar u$. By [sequential lower semicontinuity](../../../../../../../../sequential-lower-semicontinuity.md),

$$
m\leq E(\bar u)\leq\liminf_jE(u_{n_j})=m.
$$

Thus $E(\bar u)=m$. In particular, a [reflexive Banach space](../../../../../../../../reflexive-banach-space.md) with the [weak topology](../../../../../../../../weak-topology-split.md) supplies the required subsequence property by [weak sequential compactness of bounded sequences in a reflexive Banach space](../../../../../../../../weak-sequential-compactness-of-bounded-sequences-in-a-reflexive-banach-space.md). A [strictly convex function](../../../../../../../../strictly-convex-function.md) has at most one minimizer; this is an additional property, not part of the existence theorem.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [1](../../../../1.md)
5. [Paper 326](../../../../../paper-326-split.md)
6. [Iii](../../../../../split.md)
7. [2018](../../../../../../split.md)
8. [Past exam of the mathematics course of the University of Cambridge](../../../../../../../split.md)
9. [Mathematics course of the University of Cambridge](../../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../../split.md)
