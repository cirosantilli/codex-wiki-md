<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The initial-value convention is essential. A [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md), so the conclusion is $M_t=M_0$ up to [indistinguishability of stochastic processes](../../../../../../indistinguishability-of-stochastic-processes.md). The stated zero conclusion uses the usual zero-start convention $M_0=0$; without it, $M_t\equiv1$ is a counterexample.

Put $N=M-M_0$. Let $V_t$ be its [total-variation process](../../../../../../total-variation-process.md), and stop when either $|N|$ or $V$ reaches $n$. The resulting process $N^{\tau_n}$ is a bounded [continuous local martingale](../../../../../../continuous-local-martingale.md), hence a true [martingale](../../../../../../martingale-split.md), and its total variation on every time interval is bounded by $n$. Fix $t$ and take deterministic partitions $0=t_0<\cdots<t_k=t$ whose mesh tends to zero. Orthogonality of [martingale](../../../../../../martingale-split.md) increments gives

$$
\mathbb E(N^{\tau_n}_t)^2=\sum_{j=1}^k\mathbb E\bigl(N^{\tau_n}_{t_j}-N^{\tau_n}_{t_{j-1}}\bigr)^2.
$$

Pathwise,

$$
\sum_j\bigl(N^{\tau_n}_{t_j}-N^{\tau_n}_{t_{j-1}}\bigr)^2
\leq\max_j|N^{\tau_n}_{t_j}-N^{\tau_n}_{t_{j-1}}|\,V_t(N^{\tau_n})\longrightarrow0
$$

by uniform continuity of a continuous path on $[0,t]$. The sums are bounded by $2n^2$, so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) makes their expectations tend to zero. Hence $N^{\tau_n}_t=0$ almost surely. Take the countable intersection over rational $t$ and integer $n$, use path continuity, and then let $n\to\infty$. The [stopping times](../../../../../../stopping-time.md) tend to infinity because the original path and its [finite variation](../../../../../../total-variation-of-a-function.md) are bounded on every compact time interval. Thus

$$
\boxed{M_t=M_0\text{ for all }t\geq0\text{ outside one null event};\quad M_0=0\Longrightarrow M\equiv0.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
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
