<h1 id="27j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The chain is not an [irreducible Markov chain](../../../../../../irreducible-markov-chain.md), since zero is absorbing and cannot reach a positive state. Write $q_i=-q_{ii}=\sum_{j\ne i}q_{ij}$. These are finite positive holding rates for the usual [continuous-time Markov chain](../../../../../../continuous-time-markov-chain.md). Its first holding time in state $i\geq1$ is exponential with rate $q_i$, and its jump destination has probabilities $q_{ij}/q_i$. Therefore

$$
\boxed{\delta=\min_{1\leq i\leq M}\frac{q_{i0}}{q_i}>0,\qquad
\mathbb P_i(X_{J_1}=0)\geq\delta.}
$$

The recursively defined $T_m$ are [stopping times](../../../../../../stopping-time.md): after $T_m$, wait until the path first reaches a different state in the finite set. Set all later times to infinity if a previous time is infinite. On $A_m$, the [Strong Markov property](../../../../../../strong-markov-property.md) applies at $T_m$. Its next jump goes to zero with probability at least $\delta$; if it does, $T_{m+1}=\infty$. Other jumps may also prevent another qualifying visit. Thus

$$
\mathbb P_i(A_{m+1}\mid\mathcal F_{T_m})\leq1-\delta\quad\text{on }A_m,
\qquad\mathbb P_i(A_{m+1})\leq(1-\delta)\mathbb P_i(A_m).
$$

Starting with $A_0$ certain gives **$\boxed{\mathbb P_i(A_m)\leq(1-\delta)^m}$**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [27J](../../27j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
