<h1 id="2/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Partition the items into successive groups of size two, with a singleton final group if $n$ is [odd](../../../../../odd-function.md). For a pair $(x,y)$ on the east bank, execute

$$
\mathrm{LoadFirst}(x,\mathrm{EAST}),\
\mathrm{LoadLast}(y,\mathrm{EAST}),\
\mathrm{Move}(\mathrm{EAST},\mathrm{WEST}),\
\mathrm{UnloadFirst}(y,\mathrm{WEST}),\
\mathrm{UnloadLast}(x,\mathrm{WEST}).
$$

For a singleton $x$, execute

$$
\mathrm{LoadFirst}(x,\mathrm{EAST}),\
\mathrm{Move}(\mathrm{EAST},\mathrm{WEST}),\
\mathrm{UnloadLast}(x,\mathrm{WEST}).
$$

Return the empty boat east between groups. Each group starts and ends with marker $q_0$, and its items finish west, proving all [preconditions](../../../../../precondition.md) and the final goal by [mathematical induction](../../../../../mathematical-induction.md) over the groups. For $n\ge1$ there are $\lceil n/2\rceil$ outward journeys and **$2\lceil n/2\rceil-1$ crossings** in total; $\lceil\cdot\rceil$ is the [ceiling function](../../../../../ceiling-function.md). Again $n=0$ needs no actions.

## ↑ Ancestors (11)

1. [F](../f.md)
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
