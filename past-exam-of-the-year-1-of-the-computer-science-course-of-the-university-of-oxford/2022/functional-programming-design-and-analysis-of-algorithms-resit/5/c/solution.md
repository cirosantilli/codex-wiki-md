<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For each segment retain its total weight $S$, largest possibly-empty prefix weight $P$, largest possibly-empty suffix weight $Q$, and largest possibly-empty internal contiguous weight $B$. The [maximum-subarray segment summary](../../../../../maximum-subarray-segment-summary.md) combines adjacent segments as

$$
\begin{aligned}
S&=S_L+S_R,\\
P&=\max(P_L,S_L+P_R),\\
Q&=\max(Q_R,S_R+Q_L),\\
B&=\max(B_L,B_R,Q_L+P_R).
\end{aligned}
$$

An empty segment has all four values zero. For a singleton of weight $x$, use $(x,\max(0,x),\max(0,x),\max(0,x))$. The recursive procedure splits into halves, computes their summaries and applies these four formulas; the root's $B$ is the desired maximum weight.

To return an actual subsequence, attach half-open endpoints to each of $P,Q,B$. A prefix endpoint starts at its segment's left boundary, and a suffix endpoint ends at its right boundary, including empty prefixes and suffixes. Store the interval belonging to whichever candidate wins a maximum. The crossing candidate joins a left suffix to a right prefix, which meet at the split point; the other candidates keep their child endpoints. Choose an empty interval on ties at weight zero. Return the root's winning interval as a slice of the original input. This augmentation still has constant-size state and constant-time combinations.

For correctness, a prefix either stays inside the left half or consists of the entire left half and a right prefix. The suffix argument is symmetric. An optimal contiguous segment either lies in one half or crosses the split, in which case it consists of a left suffix and a right prefix. Each upper bound in the formulas is attained by its recorded candidate, proving exactness. Empty candidates ensure that an all-negative input returns the empty subsequence.

There are $\Theta(n)$ tree nodes, each using a constant number of additions and comparisons. The [divide-and-conquer algorithm](../../../../../divide-and-conquer-algorithm.md) therefore takes **$\Theta(n)$ time** and $O(\log n)$ stack space, plus the cost of copying the returned slice if a copy is required. In the stated example it selects zero-based interval $[3,6)$ of weight **8**. Carrying all four summary values avoids rescanning the halves at each split.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Functional programming, design and analysis of algorithms (resit)](../../../functional-programming-design-and-analysis-of-algorithms-resit-split.md)
4. [2022](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
