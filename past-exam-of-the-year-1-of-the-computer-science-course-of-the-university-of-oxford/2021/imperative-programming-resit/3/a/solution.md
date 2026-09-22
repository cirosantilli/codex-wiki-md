<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [abstract data type invariant](../../../../../abstract-data-type-invariant.md) constrains a total count [function](../../../../../function-split.md) on [integer](../../../../../integer-split.md) keys as follows:

$$
\forall x:\quad bag(x)\geq0,\qquad x\notin\{0,\ldots,MAX-1\}\Rightarrow bag(x)=0.
$$

The initial state has every count zero, and $MAX>0$. These conditions make the abstract state a [multiset](../../../../../multiset.md) supported on the allowed finite key range. Since the interface returns an `Int`, the implementations below use representable nonnegative multiplicities; equivalently add $bag(x)\leq M$ to the [invariant](../../../../../invariant-mathematics.md), where $M=\operatorname{Int.MaxValue}$. The corresponding add [precondition](../../../../../precondition.md) below prevents overflow. An idealized unbounded-[integer](../../../../../integer-split.md) specification can omit that machine bound.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2021](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
