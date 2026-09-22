<h1 id="m/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The state-zero [stationary distribution](../../../../../stationary-distribution.md) equation is $\pi_0=q\pi_0+q\pi_1$, so $\pi_1=(p/q)\pi_0$. The state-one equation is $\pi_1=p\pi_0+q\pi_2$, giving $\pi_2=(p/q)\pi_1$. More generally, the stationary [probability](../../../../../probability.md) flow across the cut $\{0,\ldots,i\}$ is balanced, so $p\pi_i=q\pi_{i+1}$. This also follows inductively from $\pi_i=p\pi_{i-1}+q\pi_{i+1}$.

Hence $\pi_i=(p/q)^i\pi_0$. Since $p<q$, the [geometric series](../../../../../geometric-series.md) is summable, and normalization gives

$$
\boxed{\pi_i=\left(1-\frac pq\right)\left(\frac pq\right)^i,\qquad i\ge0.}
$$

These [probabilities](../../../../../probability.md) satisfy [detailed balance](../../../../../detailed-balance.md) and therefore all the stationarity equations. The [Markov chain](../../../../../markov-chain-split.md) is an [irreducible Markov chain](../../../../../irreducible-markov-chain.md), so this normalized [stationary distribution](../../../../../stationary-distribution.md) is unique.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [5](../../5.md)
3. [M](../../../m.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the Probability, statistics and options II course of the University of Oxford](../../../../split.md)
6. [Probability, statistics and options II course of the University of Oxford](../../../../../probability-statistics-and-options-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
