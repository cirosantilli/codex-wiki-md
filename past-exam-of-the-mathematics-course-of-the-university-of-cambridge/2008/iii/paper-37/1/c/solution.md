<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Work first with $M_0=0$. More generally, the assertion needs $M_0\in L^2$ and then applies to $M-M_0$. Without this assumption, an integrable but non-square-integrable initial random variable kept constant in time has zero [quadratic variation](../../../../../../quadratic-variation.md) but is not bounded in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md).

Choose increasing [stopping times](../../../../../../stopping-time.md)

$$
\tau_n=\inf\{t:|M_t|\geq n\text{ or }[M]_t\geq n\}.
$$

They tend to infinity almost surely, because the continuous path and its [quadratic variation](../../../../../../quadratic-variation.md) are finite on every compact time interval. The stopped process is a bounded [martingale](../../../../../../martingale-split.md), and $M_{t\wedge\tau_n}^2-[M]_{t\wedge\tau_n}$ is bounded and a [local martingale](../../../../../../local-martingale.md). Taking expectations gives

$$
\mathbb E M_{t\wedge\tau_n}^2=\mathbb E[M]_{t\wedge\tau_n}.
$$

Suppose $C=\mathbb E[M]_\infty<\infty$. These squared expectations are at most $C$. For each fixed $t$, the stopped values converge almost surely to $M_t$ and are uniformly integrable, since they are uniformly bounded in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). They therefore converge in $L^1$. Passing in the stopped conditional-expectation identity, using contraction of [conditional expectation](../../../../../../conditional-expectation.md) in $L^1$, gives $\mathbb E(M_t\mid\mathcal F_s)=M_s$ for $s\leq t$. Thus $M$ is a true [martingale](../../../../../../martingale-split.md). The [Fatou lemma](../../../../../../fatou-s-lemma.md) gives $\mathbb E M_t^2\leq C$, uniformly in $t$, so it is an [L2-bounded continuous martingale](../../../../../../l2-bounded-continuous-martingale.md).

Conversely, suppose $M$ is a true [martingale](../../../../../../martingale-split.md) with $\sup_t\mathbb E M_t^2\leq C$. For fixed $t$, bounded-time [optional sampling theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) gives $M_{t\wedge\tau_n}=\mathbb E(M_t\mid\mathcal F_{t\wedge\tau_n})$. Conditional [Jensen inequality](../../../../../../jensen-s-inequality.md) then yields

$$
\mathbb E[M]_{t\wedge\tau_n}=\mathbb E M_{t\wedge\tau_n}^2\leq\mathbb E M_t^2\leq C.
$$

The brackets increase to $[M]_t$. Applying the [monotone convergence theorem](../../../../../../monotone-convergence-theorem.md) first in $n$ and then in $t\uparrow\infty$ proves $\mathbb E[M]_\infty\leq C<\infty$.

The exact identities and terminal limits can also be justified. On each fixed horizon $t$, the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) gives

$$
\mathbb E\sup_{s\leq t}|M_s|^2\leq4\mathbb E|M_t|^2<\infty.
$$

This is an integrable dominating variable for $M_{t\wedge\tau_n}^2$, so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) and increasing convergence of the brackets remove the stopping:

$$
\mathbb E M_t^2=\mathbb E[M]_t.
$$

The [L2 martingale convergence theorem](../../../../../../l2-martingale-convergence-theorem.md) supplies $M_\infty$ with $M_t\to M_\infty$ almost surely and in [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). Consequently the squares converge in $L^1$, while $[M]_t\uparrow[M]_\infty$. We obtain the [integrable terminal bracket criterion](../../../../../../integrable-terminal-bracket-criterion.md) with the precise terminal identity

$$
\boxed{M\text{ is an }L^2\text{-bounded martingale}\iff\mathbb E[M]_\infty<\infty,\qquad\mathbb E M_\infty^2=\mathbb E[M]_\infty.}
$$

For $M_0\in L^2$ rather than zero, the final identity becomes $\mathbb E M_\infty^2=\mathbb E M_0^2+\mathbb E[M]_\infty$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
