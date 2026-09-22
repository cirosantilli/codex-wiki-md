<h1 id="5/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Start with $(d[1],d[2],d[3],d[4])=(0,\infty,\infty,\infty)$. With in-place [edge relaxation](../../../../../../edge-relaxation.md), the [Bellman-Ford algorithm](../../../../../../bellman-ford-algorithm.md) makes the following changes during its first lexicographic pass:

$$
\begin{array}{c|c|c}
\text{edge}&\text{improved entry}&\text{new value}\\\hline
(1,2)&d[2]&6\\
(1,3)&d[3]&2\\
(3,2)&d[2]&5\\
(3,4)&d[4]&3\\
(4,2)&d[2]&4
\end{array}
$$

The next pass makes no change; any remaining fixed-count passes also make none. Thus the final vector is **$(0,4,2,3)$**. These are sequential updates within a pass, rather than the simultaneous values of the [Synchronous Bellman-Ford recurrence](../../../../../../synchronous-bellman-ford-recurrence.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [Functional programming, design and analysis of algorithms](../../../../functional-programming-design-and-analysis-of-algorithms-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
