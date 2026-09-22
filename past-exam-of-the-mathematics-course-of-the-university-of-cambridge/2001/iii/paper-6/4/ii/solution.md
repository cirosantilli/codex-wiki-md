<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume instead that $T$ sends weakly compact sets to norm-compact sets. If $x_n\rightharpoonup0$, then $K=\{0,x_1,x_2,\ldots\}$ is weakly compact: an open cover has a member containing zero, which contains all but finitely many terms of the convergent sequence. Hence $T(K)$ is norm compact. A [bounded linear operator](../../../../../../continuous-linear-operator.md) is weak-to-weak continuous, because each $g\in F^*$ pulls back to $g\circ T\in E^*$. Thus $Tx_n\rightharpoonup0$. If $\|Tx_n\|$ did not tend to zero, a subsequence with norms bounded below by some $\varepsilon>0$ would have a norm-convergent further subsequence with limit $y$. That further subsequence also converges weakly to both $y$ and zero; uniqueness of limits in the Hausdorff [weak topology](../../../../../../weak-topology-split.md) forces $y=0$, contradicting the lower bound. Therefore **$\boxed{\|Tx_n\|\to0}$**, proving the equivalence and the characterization of [completely continuous operators](../../../../../../completely-continuous-operator.md).

Now consider the inclusion of the [space of continuous functions on a compact space](../../../../../../space-of-continuous-functions-on-a-compact-space.md) $C(\mathbb T)$ into [L2 space](../../../../../../l2-space-is-a-hilbert-space.md) for normalized [Lebesgue measure](../../../../../../lebesgue-measure.md). It is a [bounded linear operator](../../../../../../continuous-linear-operator.md), since $\|f\|_2\le\|f\|_\infty$. For a weakly null sequence $(f_n)$ in $C(\mathbb T)$, point evaluations are [continuous linear functionals](../../../../../../continuous-linear-functional.md), so $f_n(t)\to0$ for every $t$. The [Uniform boundedness principle](../../../../../../uniform-boundedness-principle.md), applied to the canonical embeddings $f_n\in C(\mathbb T)^{**}$, gives a uniform bound $\|f_n\|_\infty\le M$: each dual functional is bounded on the weakly convergent sequence. The [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) now yields

$$
\|j_2f_n\|_2^2=\int_{\mathbb T}|f_n|^2\,d\mu\longrightarrow0.
$$

Thus **$j_2$ satisfies both equivalent conditions**.

It is nevertheless **not a [compact operator](../../../../../../compact-operator-split.md)**. Over complex scalars the functions $f_n(t)=e^{int}$ lie in the unit ball of $C(\mathbb T)$ and form an [orthonormal sequence](../../../../../../orthonormal-sequence.md) in $L^2(\mu)$, so

$$
\boxed{\|j_2f_n-j_2f_m\|_2=\sqrt2\quad(n\ne m).}
$$

There is no norm-convergent subsequence. Over real scalars use $\cos(nt)$, whose distinct images have distance $1$. Complete continuity controls weakly compact sets, rather than all bounded sets.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
