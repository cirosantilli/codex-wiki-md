<h1 id="5/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The usual [quadratic variation](../../../../../../quadratic-variation.md) convention includes $\langle M\rangle_0=0$. If $A,C$ are two continuous [finite-variation processes](../../../../../../finite-variation-process.md) with $A_0=C_0=0$ such that $M^2-A$ and $M^2-C$ are [continuous local martingales](../../../../../../continuous-local-martingale.md), then $A-C$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md) of [finite variation](../../../../../../total-variation-of-a-function.md). It must be constant, and its initial value is zero, so $A=C$ up to [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md).

Here is a proof of the fact used. Subtract the initial value of a [continuous local martingale](../../../../../../continuous-local-martingale.md) $N$ of [finite variation](../../../../../../total-variation-of-a-function.md), and stop so that both $|N|$ and its [total-variation process](../../../../../../total-variation-process.md) are bounded by deterministic constants. The stopped [local martingale](../../../../../../local-martingale.md) is a bounded true [martingale](../../../../../../martingale-split.md), so orthogonality of its increments gives, on any deterministic [partition of an interval](../../../../../../partition-of-an-interval.md) of $[0,t]$,

$$
\mathbb E(N_t^2)=\mathbb E\sum_i(\Delta_iN)^2\leq\mathbb E\left[\max_i|\Delta_iN|\,V_t(N)\right]\longrightarrow0.
$$

Continuity and the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) justify the last limit. Remove stopping and use continuity on a countable dense set of times to conclude $N\equiv0$.

**As literally printed, uniqueness is false without normalization.** If $A$ works then $A+c$ also works for any deterministic constant $c$, since subtracting a constant preserves the [local martingale](../../../../../../local-martingale.md) property; this is a genuine omitted convention.

**With normalization, existence always holds for a [continuous local martingale](../../../../../../continuous-local-martingale.md).** Its [quadratic variation](../../../../../../quadratic-variation.md) $[M]$, obtained as the limit in [probability](../../../../../../probability.md) of squared increments, is continuous, increasing, starts at zero and satisfies $M^2-[M]$ is a [continuous local martingale](../../../../../../continuous-local-martingale.md), so taking $\langle M\rangle=[M]$ supplies the required [finite-variation process](../../../../../../finite-variation-process.md).

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [5](../../5.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
