<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Write $h^*(s)$ for the optimal remaining cost and suppose $h_i(s)\le h^*(s)$ for $i=1,2$. The conclusions hold pointwise:

- **$\max(h_1,h_2)$ is an [admissible heuristic](../../../../../admissible-heuristic.md)**, because both arguments are at most $h^*$.
- **$\min(h_1,h_2)$ is an [admissible heuristic](../../../../../admissible-heuristic.md)**, since it is no larger than either argument.
- **$h_1+h_2$ is not necessarily an [admissible heuristic](../../../../../admissible-heuristic.md).** A state with a single cost-one move to a goal can have $h_1=h_2=1$ at that state and both zero at the goal. Both original [heuristic functions](../../../../../heuristic-function.md) are exact, but their sum is $2>1$.
- **$\alpha h_1+(1-\alpha)h_2$ is an [admissible heuristic](../../../../../admissible-heuristic.md) for $0\le\alpha\le1$**, since nonnegative weighting gives $\alpha h_1+(1-\alpha)h_2\le\alpha h^*+(1-\alpha)h^*=h^*$.

These are [admissible heuristic combinations](../../../../../admissible-heuristic-combination.md). An unweighted sum needs an extra condition, such as distributing action costs between the component estimates, to prevent counting the same required work twice.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2022](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
