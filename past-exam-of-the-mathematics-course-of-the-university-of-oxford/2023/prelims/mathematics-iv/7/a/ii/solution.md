<h1 id="7/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Back-substitution in the [Euclidean algorithm](../../../../../../../euclidean-algorithm.md) gives the [Bezout identity](../../../../../../../bezout-s-identity.md)

$$
7=238-11\cdot21=12\cdot238-11\cdot259=12\cdot497-23\cdot259.
$$

Multiplying by five produces a particular solution $(x,y)=(-115,60)$. Since $259/7=37$ and $497/7=71$ are [coprime integers](../../../../../../../coprime-integers.md), all solutions of the [linear Diophantine equation](../../../../../../../linear-diophantine-equation.md) are

$$
(x,y)=(-115+71t,\ 60-37t),\qquad t\in\mathbb Z.
$$

Replacing $t$ by $t+2$ gives the smaller equivalent starting solution

$$
\boxed{(x,y)=(27+71t,\ -14-37t),\qquad t\in\mathbb Z.}
$$

Indeed $259\cdot27-497\cdot14=35$. Conversely, subtracting this solution from any other gives $37(x-27)=-71(y+14)$. [Coprimality](../../../../../../../coprime-integers.md) forces $71$ to divide $x-27$, and then $y+14$ is the corresponding multiple of $-37$. This proves completeness of the family.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [7](../../../7.md)
4. [Mathematics IV](../../../../mathematics-iv-split.md)
5. [Prelims](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
