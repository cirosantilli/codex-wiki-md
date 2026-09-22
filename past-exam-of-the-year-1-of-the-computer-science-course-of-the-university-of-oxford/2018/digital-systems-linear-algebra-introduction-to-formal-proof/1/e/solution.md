<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Evaluate the implemented equations from part (d), rather than the don't-care entries of the original table:

$$
\begin{array}{c|cc}
\text{unused state}&x=0&x=1\\\hline
101&000&010\\110&011&010\\111&000&110
\end{array}.
$$

States $101$ and $110$ enter a valid state after one edge. State $111$ does so after one edge for zero, or moves to $110$ and enters a valid state on the following edge for either next input. Thus **every unused state recovers within at most two clock edges**, independently of the incoming bits. The machine cannot become trapped there. This [self-starting finite-state machine](../../../../../self-starting-finite-state-machine.md) property does not guarantee meaningful recognizer output during recovery; initialization to $S_0$ still establishes the intended stream history.

## ↑ Ancestors (12)

1. [E](../e.md)
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
