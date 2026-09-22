<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We use the [stationary weights of a reflected birth-death chain](../../../../../stationary-weights-of-a-reflected-birth-death-chain.md), also verifying why they decide the question. If a [stationary distribution](../../../../../stationary-distribution.md) $\pi$ exists, its equation at zero is $\pi_0=\pi_1d_1=\pi_0u_0$. At $k\geq1$, stationarity gives

$$
\pi_ku_k-\pi_{k+1}d_{k+1}=\pi_{k-1}u_{k-1}-\pi_kd_k.
$$

Thus the edge flow is constant, and its value at the boundary is zero. Every [stationary distribution](../../../../../stationary-distribution.md) must therefore satisfy [detailed balance](../../../../../detailed-balance.md) on each edge. Since irreducibility forces $\pi_0>0$, it must be proportional to

$$
w_0=1,\qquad w_k=\prod_{j=0}^{k-1}\frac{u_j}{d_{j+1}}.
$$

Conversely, if $\sum_kw_k<\infty$, normalizing these positive weights gives a [probability distribution](../../../../../probability-distribution-split.md) satisfying [detailed balance](../../../../../detailed-balance.md), hence a [stationary distribution](../../../../../stationary-distribution.md). Existence of a [stationary distribution](../../../../../stationary-distribution.md) for an [irreducible Markov chain](../../../../../irreducible-markov-chain.md) on a countable [state space](../../../../../state-space.md) is equivalent to [positive recurrence](../../../../../positive-recurrent-markov-chain.md).

The ratio is

$$
\frac{w_{k+1}}{w_k}=\frac{(kp+\theta)(k+1+\theta)}{(k+\theta)(k+1)q}\longrightarrow\frac pq.
$$

For $p<1/2$, the limit is less than one, so the [ratio test](../../../../../ratio-test.md) gives summability. For $p\geq1/2$, observe that $u_k=p+\theta q/(k+\theta)>p\geq1/2$, whereas $d_{k+1}<q\leq1/2$. Thus $w_{k+1}/w_k>1$ for every $k$, so the weights cannot be summable. This also resolves $p=1/2$ without making an inconclusive appeal to the limiting ratio. Therefore

$$
\boxed{\text{Positive recurrence holds exactly when }0<p<\tfrac12,\quad\theta>0.}
$$

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
