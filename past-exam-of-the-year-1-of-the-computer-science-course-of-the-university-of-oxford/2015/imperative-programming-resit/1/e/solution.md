<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The `VAR` marker passes a [reference parameter](../../../../../reference-parameter.md), so every [recursive call](../../../../../recursive-call.md) accesses the same [array](../../../../../array-data-structure.md) without copying it. Read-only access does not make copying necessary. Under the examination's [value parameter](../../../../../value-parameter.md) convention, omitting `VAR` copies the whole actual [array](../../../../../array-data-structure.md), not merely the selected segment $u[a..b)$.

If its length is $L$, the $\Theta(n+1)$ calls therefore cost $\Theta(L(n+1))$ for $n=b-a$. For a whole-input construction, $L=n>0$:

$$
\boxed{\Theta(n)\text{ with VAR},\qquad\Theta(n^2)\text{ with whole-array value copying}.}
$$

Copying only the shrinking segments would instead lead to $\Theta(n\log n)$, but that is a different [parameter passing](../../../../../parameter-passing.md) model from passing the same actual [array](../../../../../array-data-structure.md) on every call.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [1](../../1.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2015](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
