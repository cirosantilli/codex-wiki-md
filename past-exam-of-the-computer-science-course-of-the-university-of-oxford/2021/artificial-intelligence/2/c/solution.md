<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**A solution is $(A,B,C,D,E,F,G)=(1,2,1,3,4,2,3)$.** Here is a [backtracking](../../../../../backtracking.md) search with [forward checking](../../../../../forward-checking.md), listing the chosen value order rather than assuming ascending values. No backtrack is needed on this branch.

Start with the [constraint domains](../../../../../constraint-domain.md) in (a). Assign $A=1$; remove $1$ from $B,G,E$. Choose $E=4$; remove $4$ from each remaining neighbour. Now $B,G$ both have domain $\{2,3\}$ and $C,D,F$ each have $\{1,2,3\}$. Choose $B=2$. Its inequality removes $2$ from $G$, forcing $G=3$, and also removes $2$ from $D$, leaving $D\in\{1,3\}$. Assigning $G=3$ removes $3$ from $F$, leaving $F\in\{1,2\}$.

Choose $D=3$. The [edge](../../../../../edge-of-a-graph.md) $DC$ reduces $C$ to $\{1,2\}$; $DF$ makes no further deletion because $3$ is already absent from $F$. Choose $F=2$ and then $C=1$. All [variables](../../../../../variable-mathematics.md) are assigned, and every constrained pair has different values.

In time order, the schedule is

| Slot | Talks in parallel |
| --- | --- |
| $1$ | $A,C$ |
| $2$ | $B,F$ |
| $3$ | $D,G$ |
| $4$ | $E$ |

The Head of Department attends slots $1,2,3$ for $A,B,G$; first-year attendees see $C,D$ in slots $1,3$; second-year attendees see $F,G$ in $2,3$; the third-year Keble group sees $B,D$ in $2,3$; Physics attendees see $D,F$ in $3,2$. Slot $4$ is free of every competing talk, so all assumed society overlaps are respected.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2021](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
