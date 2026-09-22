<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A continuous adapted process $M$ is a [local martingale](../../../../../../local-martingale.md) if there are [stopping times](../../../../../../stopping-time.md) $\tau_n\uparrow\infty$ almost surely such that each stopped process $M^{\tau_n}_t=M_{t\wedge\tau_n}$ is a [martingale](../../../../../../martingale-split.md). In this definition $M_0$ is integrable. A continuous adapted process $A$ has [finite variation](../../../../../../total-variation-of-a-function.md) if, almost surely, its paths have finite [total variation of a function](../../../../../../total-variation-of-a-function.md) on each compact time interval:

$$
V_t(A)=\sup_{0=t_0<\cdots<t_r=t}\sum_{j=1}^r|A_{t_j}-A_{t_{j-1}}|<\infty.
$$

The permitted fact that this [total-variation process](../../../../../../total-variation-process.md) is continuous and adapted makes its level-hitting times stopping times.

Suppose $M=A$, and put $N=M-M_0$. Define

$$
\sigma_n=\tau_n\wedge n\wedge\inf\{t:V_t(N)\geq n\}.
$$

These times increase to infinity almost surely. The [optional stopping theorem](../../../../../../optional-sampling-theorem-for-a-supermartingale.md) applied to the localized martingale shows that $N^{\sigma_n}$ is a martingale; it is also bounded in absolute value by $n$, with total variation at most $n$. Fix $n,t$ and write $L=N^{\sigma_n}$. For a deterministic [partition of an interval](../../../../../../partition-of-an-interval.md) $0=t_0<\cdots<t_r=t$, orthogonality of square-integrable martingale increments gives

$$
\mathbb E L_t^2=\sum_j\mathbb E(L_{t_j}-L_{t_{j-1}})^2.
$$

Pathwise the sum on the right is bounded by $n\max_j|L_{t_j}-L_{t_{j-1}}|$. For partitions with mesh tending to zero, continuity makes this converge to zero. It is bounded by $2n^2$, so [dominated convergence](../../../../../../dominated-convergence-theorem.md) gives $\mathbb E L_t^2=0$. First use rational $t$, then continuity, to obtain $L\equiv0$ almost surely. Letting $n\to\infty$ proves

$$
\boxed{M_t=M_0\quad\text{for all }t\geq0\text{ simultaneously, almost surely}.}
$$

This proves [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md) without assuming integrability of the unstopped total variation. Continuity matters: compensated jump martingales can have finite variation without being constant.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
