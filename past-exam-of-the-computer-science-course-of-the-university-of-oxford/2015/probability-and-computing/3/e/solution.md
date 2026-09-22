<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Set $N=\binom n4$. Independently sample an [edge coloring](../../../../../edge-coloring.md) exactly as in part (d), count its [monochromatic](../../../../../monochromatic-set.md) copies of $K_4$ by examining all four-[vertex](../../../../../vertex-graph-theory.md) [subsets](../../../../../subset.md), and accept precisely when $32Z\leq N$. Otherwise start over with a fresh [edge coloring](../../../../../edge-coloring.md).

To prove an expected [polynomial time](../../../../../polynomial-time.md) bound, the existence argument alone is insufficient: we need a lower bound on the acceptance [probability](../../../../../probability.md) at this exact threshold. Since $32Z$ is a nonnegative [integer](../../../../../integer-split.md) with [expectation](../../../../../expected-value-split.md) $N$, rejection implies $32Z\geq N+1$. [Markov's inequality](../../../../../markov-s-inequality.md) therefore gives the [integer-valued expectation threshold restart bound](../../../../../integer-valued-expectation-threshold-restart-bound.md)

$$
\mathbb P(\text{reject})\leq\frac{N}{N+1},
\qquad
\boxed{\mathbb P(\text{accept})\geq\frac1{N+1}.}
$$

The number of attempts has a [geometric distribution](../../../../../geometric-distribution.md), with [expectation](../../../../../expected-value-split.md) at most $N+1$. Sampling the [edge coloring](../../../../../edge-coloring.md) costs $O(n^2)$ random [bits](../../../../../bit.md), and checking all $N$ four-[vertex](../../../../../vertex-graph-theory.md) [subsets](../../../../../subset.md) costs $O(n^4)$ operations, since only six [edges](../../../../../edge-of-a-graph.md) must be tested per [subset](../../../../../subset.md). Hence

$$
\boxed{\mathbb E[\text{running time}]=O((N+1)n^4)=O(n^8).}
$$

This is a [randomized algorithm](../../../../../randomized-algorithm.md) that always returns an [edge coloring](../../../../../edge-coloring.md) meeting the original threshold and terminates with [probability](../../../../../probability.md) one. The stated operation count uses $O(\log n)$-[bit](../../../../../bit.md) counters; counting their [bit complexity](../../../../../bit-complexity.md) explicitly introduces at most a further [logarithm](../../../../../logarithm.md) factor and still gives [polynomial time](../../../../../polynomial-time.md). For $n<4$, return any [edge coloring](../../../../../edge-coloring.md) immediately.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Probability and computing](../../../probability-and-computing-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
