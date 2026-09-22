<h1 id="1/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

When the values of several [admissible heuristics](../../../../../admissible-heuristic.md) are already available, choose their maximum:

$$
\boxed{h(R)=\max_i h_i(R).}
$$

Every $h_i(R)\le h^*(R)$, so their maximum is still an [admissible heuristic](../../../../../admissible-heuristic.md). It has [heuristic dominance](../../../../../heuristic-dominance.md) over their minimum and their arithmetic average, which are also [admissible heuristics](../../../../../admissible-heuristic.md) but give no larger lower bound. Thus the maximum supplies the most informative generally valid choice among these alternatives.

Their sum can overestimate by counting the same remaining action repeatedly. If two [heuristic functions](../../../../../heuristic-function.md) both give the exact value $1$ at a state one action from the goal, their sum gives $2$. A valid sum requires extra structure such as dividing each action's cost between the component estimates; admissibility of the components alone does not provide that structure.

Larger admissible values reduce the region $g+h<C^*$ that [A-star search](../../../../../a-star-search.md) must expand before an optimal solution of cost $C^*$ can be removed. This is a statement about [heuristic dominance](../../../../../heuristic-dominance.md), not a strict claim about running time under every tie-breaking rule or evaluation cost.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [1](../../1.md)
3. [Intelligent systems](../../../intelligent-systems-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
