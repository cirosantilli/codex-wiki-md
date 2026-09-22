<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $A_i$ be the [event](../../../../../event.md) that candidate $i$ succeeds. The [countable additivity](../../../../../countable-additivity.md) axiom adds [probabilities](../../../../../probability.md) only for mutually disjoint [events](../../../../../event.md). Successes of different candidates are not mutually exclusive, so replacing the [probability](../../../../../probability.md) of their [union](../../../../../set-union.md) by $\sum_i\mathbb P(A_i)=1$ misuses that axiom. Without disjointness one obtains only the [union bound](../../../../../boole-s-inequality.md), not certainty. The same sum is the [expected value](../../../../../expected-value-split.md) of the number of successes, which also need not imply at least one.

If the ten outcomes are mutually [independent events](../../../../../independent-events.md), with each success [probability](../../../../../probability.md) $0.1$, all fail with [probability](../../../../../probability.md) $0.9^{10}$. Hence

$$
\boxed{\mathbb P(\text{at least one success})=1-0.9^{10}
=0.6513215599\ldots.}
$$

The [independence](../../../../../independent-random-variables.md) assumption is essential. The marginal [probabilities](../../../../../probability.md) alone allow any [union](../../../../../set-union.md) [probability](../../../../../probability.md) from $0.1$ up to $1$; perfectly overlapping success [events](../../../../../event.md) give the lower endpoint and disjoint successes give the upper endpoint.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
