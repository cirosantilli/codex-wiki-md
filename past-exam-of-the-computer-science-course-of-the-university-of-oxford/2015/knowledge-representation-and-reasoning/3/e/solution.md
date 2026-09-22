<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A safe one-rule [Datalog with negation](../../../../../datalog-with-negation.md) example with no [stable model](../../../../../stable-model.md) is

$$
\boxed{\operatorname{not}P(a)\to P(a).}
$$

There are no variables, so no safety condition is violated. If $P(a)$ is absent from a proposed [stable model](../../../../../stable-model.md), its reduct contains the fact $P(a)$, whose [least Herbrand model](../../../../../least-herbrand-model.md) contains $P(a)$. If $P(a)$ is present, the rule is deleted, and the reduct has empty [least Herbrand model](../../../../../least-herbrand-model.md). Either choice disagrees with its reduct's [least Herbrand model](../../../../../least-herbrand-model.md). Additional unsupported atoms cannot repair the disagreement. Hence there is no [stable model](../../../../../stable-model.md).

## ↑ Ancestors (11)

1. [E](../e.md)
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
