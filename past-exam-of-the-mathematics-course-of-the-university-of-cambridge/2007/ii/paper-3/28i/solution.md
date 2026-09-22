<h1 id="28i/solution">Solution</h1>

↑ **Parent:** [28I](../28i.md)

A [Markov control](../../../../../markov-policy.md) chooses its action from the current time and state, $a=u(k,x)$, rather than the full past. It gives transition probabilities $P_k^u(x,y)=P(y\mid k,x,u(k,x))$, hence a time-inhomogeneous [Markov chain](../../../../../markov-chain.md).

For any admissible control, the given inequality and conditional expectation imply

$$
V(k,X_k)\leq c(k,X_k,A_k)+\mathbb E[V(k+1,X_{k+1})\mid\mathcal F_k].
$$

Take expectations and sum from zero to $n-1$. The value terms telescope, and $V(n,X_n)=C(X_n)$ gives $V(0,x)\leq\mathbb E_x[\sum_{k<n}c(k,X_k,A_k)+C(X_n)]$. For $u^*$ every inequality is equality, so its cost is exactly $V(0,x)$ and it achieves the lower bound. Thus **$u^*$ is optimal**. Boundedness of $V$ and the usual integrability of the costs justify these expectations; the argument even compares it with history-dependent controls.

For the cards, let $r,b$ be the remaining red and black counts, $m=r+b\geq2$. Betting now succeeds with probability $q(r,b)=r(r-1)/[m(m-1)]$. For $m\geq3$, elementary simplification gives

$$
\frac r m q(r-1,b)+\frac b m q(r,b-1)=q(r,b),
$$

with zero-probability transitions omitted when a colour count vanishes. Thus continuing one reveal has exactly the same conditional winning probability as betting now. The backward value function for maximal success probability is $q$ at $m=2$, and induction makes it $q$ at every earlier state: the stop and continue values coincide. Equivalently the conditional success probabilities are a bounded [martingale](../../../../../martingale-split.md), and every permitted stopping time is bounded by the time at which two cards remain.

Therefore **any adapted betting rule that makes exactly one bet while at least two cards remain is optimal**; there is no strictly advantageous moment. Betting immediately is one simple optimal rule, with winning probability $26\cdot25/(52\cdot51)=25/102$. The stake size only rescales a fixed payoff, and does not alter this comparison. This is [unchanging betting probability under sampling without replacement](../../../../../unchanging-betting-probability-under-sampling-without-replacement.md); allowing the player never to bet would be a different problem.

## ↑ Ancestors (10)

1. [28I](../28i.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
