<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The number is

$$
\boxed{\binom{16}{6}=8008.}
$$

A direct search over every $q$-element [subset](../../../../../subset.md) must inspect $\binom nq$ candidates. Testing one candidate by generating its [subset sums](../../../../../subset-sum-problem.md) creates $2^q$ values; storing previously seen sums detects a collision. Generating them incrementally needs $O(2^q)$ arithmetic operations, or $O(q2^q)$ for the straightforward independent calculation of each sum. Thus the simple overall search has cost on the scale of $\binom nq2^q$, apart from [integer](../../../../../integer-split.md)-arithmetic and data-structure costs.

The important [time complexity](../../../../../time-complexity.md) distinction is that **fixed $q$ gives polynomial growth in $n$, of degree $q$**, but this can still become impractically large. If $q$ increases with $n$, both the candidate count and the internal [power set](../../../../../power-set.md) can grow exponentially. For example, near $q=n/2$ the [binomial coefficient](../../../../../binomial-coefficient-split.md) is already exponentially large. An exhaustive implementation can therefore encounter a [combinatorial explosion](../../../../../combinatorial-explosion.md); the fixed-$q$ estimate $\Theta(n^q)$ must not be described as exponential in $n$.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
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
