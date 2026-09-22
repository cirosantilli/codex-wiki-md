<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

[Expectiminimax](../../../../../expectiminimax.md) adds [chance nodes](../../../../../chance-node.md) to the MAX and MIN decisions. A [chance node](../../../../../chance-node.md) uses

$$
V(s)=\sum_j p_jV(s_j),
$$

so exact evaluation generally needs all outcomes with positive [probability](../../../../../probability.md). An unfavorable child does not determine the [expected value](../../../../../expected-value-split.md): a later, sufficiently favorable child can offset it. Ordinary [alpha-beta pruning](../../../../../alpha-beta-pruning.md) therefore does not directly discard the remaining outcomes.

Random outcomes also enlarge the effective [branching factor](../../../../../branching-factor.md). If each player decision has $b$ choices and each action has $c$ chance outcomes, exploring $d$ player decisions can require order $(bc)^d$ leaves rather than $b^d$. Under the same budget, this gives roughly

$$
d_{\mathrm{stochastic}}\approx\frac{\log n}{\log b+\log c}
$$

before additional pruning benefits available in the deterministic game are considered. Exact [probability](../../../../../probability.md) calculations add overhead as well. These effects explain the typically shallower horizon; randomness alone is not a theorem of inevitable slowdown. Known [utility](../../../../../utility.md) bounds permit some [expected value](../../../../../expected-value-split.md) bounds and specialized pruning, and chance sampling can trade exactness for speed.[§3.3, chance-node expected-value backup; §3.3.1, mixed layer types](../../../../../cs-188-stochastic-and-general-game-notes.md)

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
