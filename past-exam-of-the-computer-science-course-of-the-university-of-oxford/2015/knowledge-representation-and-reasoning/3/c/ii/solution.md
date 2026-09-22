<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The remaining classification rule is

$$
\boxed{\mathit{Year}(x)\land\operatorname{not}\mathit{Leap}(x)\to\mathit{Common}(x).}
$$

The positive premise restricts the rule to years. Its [negation as failure](../../../../../../negation-as-failure.md) premise is evaluated by [stable model semantics](../../../../../../stable-model-semantics.md); it does not assert a separately stored negative fact. This gives a [stratified Datalog](../../../../../../stratified-datalog.md) program: divisibility and year facts are inputs, leap status is computed next, and common status last.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [Knowledge representation and reasoning](../../../../knowledge-representation-and-reasoning-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the computer science course of the University of Oxford](../../../../../split.md)
7. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
