<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

$\boxed{\text{No.}}$ A [disjunctive Datalog](../../../../../disjunctive-datalog.md) [knowledge base](../../../../../knowledge-base.md) can have several incomparable minimal [Herbrand models](../../../../../herbrand-model.md) without a [least Herbrand model](../../../../../least-herbrand-model.md). Take the single disjunctive fact

$$
\top\to P(a)\lor Q(a).
$$

Both $M_1=\{P(a)\}$ and $M_2=\{Q(a)\}$ are [Herbrand models](../../../../../herbrand-model.md). Any [least Herbrand model](../../../../../least-herbrand-model.md) would have to be contained in both, hence contained in $M_1\cap M_2=\varnothing$. But the empty [Herbrand interpretation](../../../../../herbrand-structure.md) falsifies the disjunctive fact. This is a contradiction. Taking the intersection of all models therefore fails because that intersection need not itself be a model.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Knowledge representation and reasoning](../../../knowledge-representation-and-reasoning-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
