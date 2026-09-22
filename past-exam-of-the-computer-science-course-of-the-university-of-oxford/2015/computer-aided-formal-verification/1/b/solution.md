<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Splitting the [Boolean function](../../../../../boolean-function.md) according to the first tested [Boolean variable](../../../../../boolean-variable.md) gives

$$
f=(\neg x\land y)\lor\bigl(x\land((\neg y\land z)\lor y)\bigr).
$$

The identity $y\lor(\neg y\land z)=y\lor z$ follows by considering $y=0$ and $y=1$. Using it and distributing [Boolean conjunction](../../../../../logical-conjunction.md) over [Boolean disjunction](../../../../../logical-disjunction.md),

$$
f=(\neg x\land y)\lor(x\land y)\lor(x\land z)
 =\boxed{y\lor(x\land z)}.
$$

The first two terms combine to $y$ because $x\lor\neg x=1$. This also explains the [truth table](../../../../../truth-table.md): $y=1$ always makes the output one, while with $y=0$ the output is one exactly when both $x$ and $z$ are one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
