<h1 id="1d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the [Euclidean algorithm](../../../../../../euclidean-algorithm.md): $23=18+5$, $18=3\cdot5+3$, $5=3+2$, and $3=2+1$. Back-substitution gives the [Bezout identity](../../../../../../bezout-identity.md) $1=9\cdot18-7\cdot23$. Multiplying by $101$ gives one solution of the [linear Diophantine equation](../../../../../../linear-diophantine-equation.md), and shifting the coefficients by multiples of $(23,-18)$ reduces it to

$$
\boxed{x=12,\qquad y=-5.}
$$

Indeed, $18\cdot12+23(-5)=216-115=101$. More generally all solutions are $x=12+23k$, $y=-5-18k$, $k\in\mathbb Z$: subtracting this particular solution gives $18(x-12)=-23(y+5)$, and the [coprime integers](../../../../../../coprime-integers.md) $18,23$ [force](../../../../../../force.md) $23\mid(x-12)$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1D](../../1d.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
