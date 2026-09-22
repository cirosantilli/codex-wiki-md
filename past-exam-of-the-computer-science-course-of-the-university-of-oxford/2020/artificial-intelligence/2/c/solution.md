<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**One solution is $(a,b,c,d,e)=(1,2,3,2,1)$.** Use ascending value order; after [minimum remaining values](../../../../../minimum-remaining-values.md) and the [degree heuristic](../../../../../degree-heuristic.md), break any remaining [variable](../../../../../variable-mathematics.md) tie alphabetically. Apply the unary restrictions first:

$$
D_a=\{1,2\},\quad D_b=\{1,2,3\},\quad D_c=D_d=D_e=\{1,2,3,4\}.
$$

[Minimum remaining values](../../../../../minimum-remaining-values.md) selects $a$, even though $c$ has greater initial [vertex degree](../../../../../degree-graph-theory.md). Set $a=1$. [Forward checking](../../../../../forward-checking.md) removes $1$ from the three neighbors $b,c,d$:

$$
D_b=\{2,3\},\quad D_c=D_d=\{2,3,4\},\quad D_e=\{1,2,3,4\}.
$$

Now $b$ is the unique [minimum remaining values](../../../../../minimum-remaining-values.md) choice. Set $b=2$. [Forward checking](../../../../../forward-checking.md) removes $2$ from $c,e$, giving

$$
D_c=\{3,4\},\quad D_d=\{2,3,4\},\quad D_e=\{1,3,4\}.
$$

Select $c$ and set $c=3$. Its remaining neighbors are $d,e$, so [forward checking](../../../../../forward-checking.md) gives

$$
D_d=\{2,4\},\qquad D_e=\{1,4\}.
$$

The two remaining [variables](../../../../../variable-mathematics.md) tie on [constraint domain](../../../../../constraint-domain.md) size and each has one unassigned neighbor, so the [degree heuristic](../../../../../degree-heuristic.md) also ties. Alphabetical order selects $d$; take $d=2$. Since $2$ is already absent from $D_e$, [forward checking](../../../../../forward-checking.md) makes no further deletion. Finally choose $e=1$. No empty [constraint domain](../../../../../constraint-domain.md) or violation occurs, so this branch needs no [backtracking](../../../../../backtracking.md).

All eight [binary constraints](../../../../../binary-constraint.md) are checked explicitly by the unequal value pairs

$$
(a,b)=(1,2),\ (a,d)=(1,2),\ (a,c)=(1,3),\ (b,e)=(2,1),\ (b,c)=(2,3),\ (c,e)=(3,1),\ (c,d)=(3,2),\ (d,e)=(2,1).
$$

The unary restrictions also hold. Equalities $a=e$ and $b=d$ are permitted because those pairs have no [edges](../../../../../edge-of-a-graph.md) in the [constraint graph](../../../../../constraint-graph.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Artificial intelligence](../../../artificial-intelligence-split.md)
4. [2020](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
