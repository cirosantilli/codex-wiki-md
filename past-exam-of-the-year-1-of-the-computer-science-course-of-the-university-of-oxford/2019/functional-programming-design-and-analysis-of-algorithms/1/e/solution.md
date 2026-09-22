<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $F=\mathrm{foldl}\ (\ominus)\ 0$, using the specified operation $u\ominus v=v-u$. Direct evaluation gives $F([])=0$, $F([0])=0$, $F([1])=1$, and $F([1,0])=-1$.

Suppose $F=\mathrm{foldr}\ c\ b$ with the same [integer](../../../../../integer-split.md) result type. The empty [list](../../../../../list-abstract-data-type.md) forces $b=0$. The two singleton calculations force $c\ 0\ 0=0$ and $c\ 1\ 0=1$. But then

$$
F([1,0])=c\ 1\ (c\ 0\ 0)=c\ 1\ 0=1,
$$

contrary to $F([1,0])=-1$. **No such `c,b` exist.** This is the information restriction in the [fold factorisation criterion](../../../../../fold-factorisation-criterion.md): equal folded tails must remain indistinguishable after the same head is attached. A larger, [function](../../../../../function-split.md)-valued result type can retain the missing information, as the [continuation representation of a left fold](../../../../../continuation-representation-of-a-left-fold.md) does below.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Functional programming, design and analysis of algorithms](../../../functional-programming-design-and-analysis-of-algorithms-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
