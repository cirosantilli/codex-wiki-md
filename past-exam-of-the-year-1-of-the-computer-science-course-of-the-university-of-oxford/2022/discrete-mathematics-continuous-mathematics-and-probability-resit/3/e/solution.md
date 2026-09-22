<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Prove the stronger statement with a nonempty [subset](../../../../../subset.md). Order the $n\geq1$ [integers](../../../../../integer-split.md) as $a_1,\ldots,a_n$, and form the [prefix sums](../../../../../prefix-sum.md)

$$
s_0=0,\qquad s_j=\sum_{k=1}^ja_k\quad(1\leq j\leq n).
$$

There are $n+1$ such sums but only $n$ [residue classes](../../../../../residue-class.md) modulo $n$. The [pigeonhole principle](../../../../../pigeonhole-principle.md) gives indices $0\leq i<j\leq n$ with $s_i\equiv s_j\pmod n$. Their difference satisfies

$$
s_j-s_i=a_{i+1}+\cdots+a_j\equiv0\pmod n.
$$

The selected elements form a nonempty [subset](../../../../../subset.md) of $S$, proving the claim. Neither positivity nor distinct values in a general ordered [sequence](../../../../../sequence.md) are needed for the [consecutive sum divisible by the sequence length](../../../../../consecutive-sum-divisible-by-the-sequence-length.md) argument; distinctness merely makes the present input a [set](../../../../../set-split.md).

## ↑ Ancestors (12)

1. [E](../e.md)
2. [3](../../3.md)
3. [Discrete mathematics, continuous mathematics and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
