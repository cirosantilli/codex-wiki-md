<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Five distinct states require **three [D flip-flops](../../../../../d-flip-flop.md)**, since $2^2<5\leq2^3$. Choose the [state encoding](../../../../../state-encoding.md) $S_i$ equal to the three-bit binary expansion of $i$. Write the present bits as $A,B,C$, in decreasing significance. The [state transition table](../../../../../state-transition-table.md) is

$$
\begin{array}{c|cc|c}
ABC&x=0:\ A^+B^+C^+&x=1:\ A^+B^+C^+&y\\\hline
000&000&001&0\\001&000&010&0\\010&011&010&0\\011&000&100&0\\100&000&010&1\\101&---&---&-\\110&---&---&-\\111&---&---&-
\end{array}.
$$

The dashes are [don't-care conditions](../../../../../don-t-care-term.md) for minimizing the logic. They do not prescribe what the actual circuit will do in those unused states; part (e) determines that from the chosen equations.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
