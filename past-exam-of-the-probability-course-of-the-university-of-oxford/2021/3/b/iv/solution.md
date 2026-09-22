<h1 id="3/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

First identify the recurrence type, rather than infer an occupation limit from a one-time [probability](../../../../../probability.md). At time $k(a+b)$, return to zero requires exactly $kb$ upward steps. The [binomial distribution](../../../../../binomial-distribution.md) gives

$$
\mathbb P_0(S_{k(a+b)}=0)=\binom{k(a+b)}{kb}\left(\frac b{a+b}\right)^{kb}\left(\frac a{a+b}\right)^{ka}
\sim\sqrt{\frac{a+b}{2\pi abk}},
$$

where the last step is [Stirling's approximation](../../../../../stirling-formula.md). At all other positive times the return [probability](../../../../../probability.md) is zero. Hence $\sum_{n\geq0}\mathbb P_0(S_n=0)=\infty$. The [recurrence criterion by return probabilities](../../../../../recurrence-criterion-by-return-probabilities.md) proves the [recurrent](../../../../../recurrent-markov-chain.md) property; by the [irreducible Markov chain](../../../../../irreducible-markov-chain.md) property established in (i), every state is [recurrent](../../../../../recurrent-markov-chain.md). The equivalence of [positive recurrence](../../../../../positive-recurrent-markov-chain.md) and existence of a [stationary distribution](../../../../../stationary-distribution.md) for an [irreducible Markov chain](../../../../../irreducible-markov-chain.md) on a [countable](../../../../../countable-set.md) [state space](../../../../../state-space.md), together with (iii), makes this chain [null recurrent](../../../../../null-recurrent-state.md).

For completeness, the zero occupation proportion follows directly by treating returns as a [renewal process](../../../../../renewal-process.md). Let $L_1,L_2,\ldots$ be successive strictly positive return-cycle lengths to zero. The [Strong Markov property](../../../../../strong-markov-property.md) makes them [independent and identically distributed](../../../../../independent-and-identically-distributed-random-variables.md), the [recurrent](../../../../../recurrent-markov-chain.md) property makes them finite [almost surely](../../../../../almost-sure-convergence.md), and the [null recurrent](../../../../../null-recurrent-state.md) property gives $\mathbb EL_1=\infty$. For each positive [integer](../../../../../integer-split.md) $K$, the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) applied to $\min(L_j,K)$ gives

$$
\liminf_{r\to\infty}\frac{L_1+\cdots+L_r}{r}\geq\mathbb E\min(L_1,K)\quad\text{almost surely}.
$$

Take a common event of [probability](../../../../../probability.md) one for these countably many $K$. By the [monotone convergence theorem](../../../../../monotone-convergence-theorem.md), the right side increases to infinity. Thus the number of completed return cycles by time $n$, divided by $n$, tends to zero. Counting the initial visit changes this ratio by at most $1/n$. Consequently,

$$
\boxed{\frac1n\sum_{r=0}^{n-1}\mathbf1_{\{S_r=0\}}\longrightarrow0\quad\text{almost surely}.}
$$

The walk visits zero infinitely often, but the asymptotic fraction of time spent there is zero.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
