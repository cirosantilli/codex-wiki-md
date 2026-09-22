<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $bag_0$ for the incoming state and $M=\operatorname{Int.MaxValue}$. Use the following explicit contracts.

For `add(x)`, the [precondition](../../../../../precondition.md) is $0\leq x<MAX$ and $bag_0(x)<M$. The [postcondition](../../../../../postcondition.md) is $bag(x)=bag_0(x)+1$ and $bag(y)=bag_0(y)$ for every $y\neq x$.

For `remove(x)`, the [precondition](../../../../../precondition.md) is $0\leq x<MAX$ and $bag_0(x)>0$. The [postcondition](../../../../../postcondition.md) is $bag(x)=bag_0(x)-1$, with every other count unchanged. This convention rejects removal of an absent occurrence rather than silently treating it as a no-op.

For `count(x)`, the [precondition](../../../../../precondition.md) is $0\leq x<MAX$. The result is $bag_0(x)$ and the whole abstract state is unchanged. Counts outside the allowed range are zero in the mathematical total [function](../../../../../function-split.md), but this chosen interface requires an in-range query.

## ↑ Ancestors (12)

1. [B](../b.md)
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
