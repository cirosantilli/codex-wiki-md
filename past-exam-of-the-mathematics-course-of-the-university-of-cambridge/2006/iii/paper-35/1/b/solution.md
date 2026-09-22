<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $V_t$ be the [total variation](../../../../../../total-variation.md) of $X$ on $[0,t]$, and set $\tau_n=\inf\{t:V_t\ge n\}$. Adaptation and continuity of $V$ make these [stopping times](../../../../../../stopping-time.md); [finite variation](../../../../../../total-variation-of-a-function.md) on every compact interval gives $\tau_n\uparrow\infty$. The stopped process $U=X^{\tau_n}$ satisfies $|U_t|\le n$ and has [total variation](../../../../../../total-variation.md) at most $n$. It is a [martingale](../../../../../../martingale-split.md) by the [bounded local martingale criterion](../../../../../../bounded-local-martingale-criterion.md), and is [square-integrable](../../../../../../square-integrable-function.md).

Fix $t$ and take deterministic partitions $0=t_0<\cdots<t_m=t$ with mesh tending to zero. The [martingale-difference orthogonality](../../../../../../martingale-difference-orthogonality.md) of the increments gives

$$
\mathbb E[U_t^2]=\sum_j\mathbb E[(U_{t_{j+1}}-U_{t_j})^2].
$$

Pathwise, however,

$$
\sum_j(U_{t_{j+1}}-U_{t_j})^2
\le\max_j|U_{t_{j+1}}-U_{t_j}|\sum_j|U_{t_{j+1}}-U_{t_j}|
\le n\max_j|U_{t_{j+1}}-U_{t_j}|\longrightarrow0,
$$

by [uniform continuity](../../../../../../uniform-continuity.md) on $[0,t]$. These sums are bounded by $n^2$, so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives $\mathbb E U_t^2=0$. Hence $U_t=0$ almost surely. Take all rational $t$ on a common probability-one event and use continuity to obtain $U\equiv0$. Then let $n\to\infty$. This proves the [continuous finite-variation local martingale is constant](../../../../../../continuous-finite-variation-local-martingale-is-constant.md) result in its zero-starting form:

$$
\boxed{X_t=0\text{ for every }t\ge0\text{ almost surely}.}
$$

The proof does not assume the uniqueness of [quadratic variation](../../../../../../quadratic-variation.md) that is to be established next.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
