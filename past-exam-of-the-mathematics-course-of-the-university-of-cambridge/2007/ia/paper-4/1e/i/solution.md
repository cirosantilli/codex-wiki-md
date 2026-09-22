<h1 id="1e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Euclidean algorithm](../../../../../../euclidean-algorithm.md) gives

$$
18=2\cdot7+4,\qquad 7=4+3,\qquad 4=3+1.
$$

Back-substitution supplies the [Bezout identity](../../../../../../bezout-identity.md)

$$
1=4-3=2\cdot4-7=2(18-2\cdot7)-7=2\cdot18-5\cdot7.
$$

Thus one solution is $(x,y)=(-5,2)$. If $(x,y)$ is any solution, subtraction gives $7(x+5)+18(y-2)=0$. Since $7$ and $18$ are coprime, $18$ divides $x+5$. Write $x+5=18t$; substitution then gives $y-2=-7t$. Conversely these values satisfy the equation for every [integer](../../../../../../integer.md) $t$. Hence **all solutions** are

$$
\boxed{x=-5+18t,\qquad y=2-7t,\qquad t\in\mathbb Z.}
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1E](../../1e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
