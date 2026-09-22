<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For $i=1,\ldots,n$, execute

$$
\mathrm{Load}(\mathrm{ITEM}i,\mathrm{EAST}),\quad
\mathrm{Move}(\mathrm{EAST},\mathrm{WEST}),\quad
\mathrm{Unload}(\mathrm{ITEM}i,\mathrm{WEST}),
$$

and, if $i<n$, append $\mathrm{Move}(\mathrm{WEST},\mathrm{EAST})$ before the next iteration.

Each load starts with an empty boat beside an undelivered item. Each unload leaves that item west and restores the loading [precondition](../../../../../precondition.md). By [mathematical induction](../../../../../mathematical-induction.md) on $i$, after iteration $i$ the first $i$ items are west and the remaining items are east. Thus the [automated planning](../../../../../automated-planning.md) goal holds after **$2n-1$ crossings and $4n-1$ actions** for $n\ge1$. For $n=0$, the empty plan already achieves the goal.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2023](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
