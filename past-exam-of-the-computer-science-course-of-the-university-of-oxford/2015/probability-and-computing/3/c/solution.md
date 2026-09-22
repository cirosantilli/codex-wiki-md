<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use [uniform balanced binary sequence sampling](../../../../../uniform-balanced-binary-sequence-sampling.md) by choosing the positions of the heads. Number the $2n=2^m$ positions from zero to $2n-1$. Start with no selected positions. Repeatedly toss the fair coin $m$ times, interpret the resulting [bits](../../../../../bit.md) as a position, and select that position if it has not already been selected; otherwise discard this block of tosses and retry. Stop when $n$ distinct positions have been selected. Put heads at those positions and tails everywhere else.

After $s$ positions have been selected, every one of the remaining positions has the same [probability](../../../../../probability.md) of being the next new position. This follows either by summing a [geometric series](../../../../../geometric-series.md) over rejected blocks or by conditioning a [uniform distribution on a finite set](../../../../../discrete-uniform-distribution.md) on avoiding the selected positions. Every ordered list of $n$ distinct selected positions consequently has [probability](../../../../../probability.md)

$$
\frac1{(2n)(2n-1)\cdots(n+1)}.
$$

Each fixed $n$-element [subset](../../../../../subset.md) has $n!$ such orders, so its [probability](../../../../../probability.md) is

$$
\boxed{\frac{n!}{(2n)(2n-1)\cdots(n+1)}=\frac1{\binom{2n}{n}}.}
$$

Thus every balanced [binary sequence](../../../../../bitstream.md) is equally likely.

When $s$ positions are selected, a block succeeds with [probability](../../../../../probability.md) $(2n-s)/(2n)$, so the [geometric distribution](../../../../../geometric-distribution.md) gives [expectation](../../../../../expected-value-split.md) $2n/(2n-s)$ blocks until the next new position. By [linearity of expectation](../../../../../linearity-of-expectation.md), the total expected toss count is

$$
\boxed{m\sum_{s=0}^{n-1}\frac{2n}{2n-s}<2nm=O(n\log n),\qquad n\geq1.}
$$

The strict inequality holds since $s<n$, making each term less than two. A Boolean [array](../../../../../array-data-structure.md) records membership of each position; initializing it and constructing the output require $O(n)$ additional work. The scheme terminates with [probability](../../../../../probability.md) one, since every stage has positive success [probability](../../../../../probability.md).

## ↑ Ancestors (11)

1. [C](../c.md)
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
