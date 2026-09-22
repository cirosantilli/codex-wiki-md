<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $S=H\mathbin\cdot M$ and $A_t=\int_0^tH_s^2d[M]_s$. The candidate $A$ is continuous, adapted, nondecreasing, starts at zero and has integrable terminal value. We prove $S^2-A$ is a [martingale](../../../../../../martingale-split.md), rather than assuming the desired [quadratic variation of a stochastic integral](../../../../../../quadratic-variation-of-a-stochastic-integral.md).

The assumed boundedness of $M$ also makes $M^2-[M]$ a true [martingale](../../../../../../martingale-split.md) on every finite horizon. Indeed, apply its local [martingale](../../../../../../martingale-split.md) identity at a [localizing sequence](../../../../../../localizing-sequence.md); bounded stopped squares and the [Fatou lemma](../../../../../../fatou-s-lemma.md) show that $[M]_t$ is integrable. The stopped expressions are then dominated by $\sup_s|M_s|^2+[M]_t$, so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives the unrestricted conditional identity on that horizon.

First let $H$ be a bounded [simple predictable process](../../../../../../simple-predictable-process.md). On each interval with coefficient $h$, an increment of $S$ is $h(M_t-M_a)$. The defining [quadratic variation](../../../../../../quadratic-variation.md) identity for $M$, together with the [martingale](../../../../../../martingale-split.md) property of $M$, makes

$$
(M_t-M_a)^2-([M]_t-[M]_a)
$$

a [martingale](../../../../../../martingale-split.md) for $t\geq a$. Expanding $S_t^2-S_a^2$ gives a term $2S_ah(M_t-M_a)$ and the square term above; their [conditional expectations](../../../../../../conditional-expectation.md) yield the desired identity on that interval. Integrability follows because the variables are [square-integrable](../../../../../../square-integrable-function.md); concatenating the finitely many intervals gives $S^2-A$ a [martingale](../../../../../../martingale-split.md).

For general bounded [predictable](../../../../../../predictable-process.md) $H$, choose bounded [simple predictable processes](../../../../../../simple-predictable-process.md) $H^n\to H$ in $L^2(M)$, which is possible since they generate the [predictable sigma-algebra](../../../../../../predictable-sigma-algebra.md). Set $S^n=H^n\mathbin\cdot M$ and $A_t^n=\int_0^t(H_s^n)^2d[M]_s$. The [Itô isometry](../../../../../../ito-isometry.md) and [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) imply $S_t^n\to S_t$ in $L^2$; the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives $(S_t^n)^2\to S_t^2$ in $L^1$ and

$$
\mathbb E\sup_t|A_t^n-A_t|
\leq\|H^n-H\|_{L^2(M)}\bigl(\|H^n\|_{L^2(M)}+\|H\|_{L^2(M)}\bigr)\longrightarrow0.
$$

Pass the [conditional expectation](../../../../../../conditional-expectation.md) identity for $(S^n)^2-A^n$ to the $L^1$ limit. Thus $S^2-A$ is a [martingale](../../../../../../martingale-split.md). Uniqueness in the defining [quadratic variation](../../../../../../quadratic-variation.md) property now gives

$$
\boxed{[H\mathbin\cdot M]_t=\int_0^tH_s^2\,d[M]_s.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
