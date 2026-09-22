<h1 id="4h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The procedure in part (i) sometimes needs five tests, for items one or two. A binary [decision tree](../../../../../../decision-tree.md) of height $N$ has at most $2^N$ leaves, so distinguishing ten possibilities requires $N\geq\lceil\log_2 10\rceil=4$.

A [prefix code](../../../../../../prefix-code.md) attaining this worst-case bound is

$$
\begin{array}{c|cccccccccc}
\text{item}&1&2&3&4&5&6&7&8&9&10\\\hline
\text{code}&1100&1101&1110&1111&000&001&010&011&100&101.
\end{array}
$$

Use the same subset-testing rule. **The minimum worst-case number is four, so the expected-optimal procedure is not worst-case optimal.** This four-test procedure has expectation $175/55$, illustrating the small cost of imposing the smaller maximum depth.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4H](../../4h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
