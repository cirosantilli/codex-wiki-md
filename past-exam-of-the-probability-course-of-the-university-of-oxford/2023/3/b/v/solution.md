<h1 id="3/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Let $I_n$ count immigration events during the first $n$ transitions, and let $A_n$ count upward steps during those transitions. Write $h(k)=\theta/(k+\theta)$ for the conditional immigration probability. If $J_m$ is the indicator that transition $m$ to $m+1$ is immigration, then $J_m-h(X_m)$ is a bounded [martingale difference](../../../../../martingale-difference.md) with respect to the history that records event types as well as population sizes. The [strong law for martingales with bounded increments](../../../../../strong-law-for-martingales-with-bounded-increments.md) implies

$$
\frac{I_n}{n}-\frac1n\sum_{m=0}^{n-1}h(X_m)\longrightarrow0\quad\text{almost surely}.
$$

Since $h$ is bounded, the [countable-state Markov chain ergodic theorem](../../../../../countable-state-markov-chain-ergodic-theorem.md) gives

$$
\frac{I_n}{n}\longrightarrow\sum_{k=0}^\infty\pi_k\frac{\theta}{k+\theta}\quad\text{almost surely}.
$$

Applying the same argument to upward-step indicators gives $A_n/n\to\sum_k\pi_ku_k$ [almost surely](../../../../../almost-sure-convergence.md). To evaluate this denominator, sum [detailed balance](../../../../../detailed-balance.md) over all neighboring edges:

$$
\sum_{k=0}^\infty\pi_ku_k=\sum_{k=0}^\infty\pi_{k+1}d_{k+1}=\sum_{k=0}^\infty\pi_kd_k.
$$

Since $u_k+d_k=1$ and $\sum_k\pi_k=1$, both sums equal $1/2$. The denominator limit is positive, so division is valid and the [immigration fraction among upward steps](../../../../../immigration-fraction-among-upward-steps.md) is

$$
\boxed{\frac{I_n}{A_n}\longrightarrow2\sum_{k=0}^\infty\pi_k\frac{\theta}{k+\theta}\quad\text{almost surely}.}
$$

This is the requested answer in terms of $\pi$. Substituting part (iii) additionally gives $\sum_k\pi_k\theta/(k+\theta)=(1-r)/2$, so the fraction simplifies to $1-r=(1-2p)/(1-p)$.

## ↑ Ancestors (13)

1. [V](../v.md)
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
