<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [extended Euclidean algorithm](../../../../../extended-euclidean-algorithm.md) gives

$$
29=17+12,\qquad17=12+5,\qquad12=2\cdot5+2,\qquad5=2\cdot2+1.
$$

Back-substituting in these equations produces the [Bezout identity](../../../../../bezout-identity.md)

$$
1=5-2(12-2\cdot5)=5\cdot5-2\cdot12
=5\cdot17-7\cdot12=12\cdot17-7\cdot29.
$$

Thus **one integer solution** is $\boxed{x=12,\ y=-7}$. In fact, subtracting this [Bezout identity](../../../../../bezout-identity.md) from any other solution and using that $17$ and $29$ are [coprime integers](../../../../../coprime-integers.md) gives all solutions: $x=12+29t$, $y=-7-17t$, where $t\in\mathbb Z$.

For the [modular arithmetic](../../../../../modular-arithmetic.md) calculation, $29$ is a [prime number](../../../../../prime-number.md) and $17$ is [coprime](../../../../../coprime-integers.md) to it, so [Fermat little theorem](../../../../../fermat-little-theorem.md) gives $17^{28}\equiv1\pmod{29}$. Since $138=5\cdot28-2$, and the preceding [Bezout identity](../../../../../bezout-identity.md) identifies $12$ as the [modular multiplicative inverse](../../../../../modular-multiplicative-inverse.md) of $17$, we obtain

$$
17^{138}\equiv17^{-2}\equiv12^2=144\equiv28\pmod{29}.
$$

Consequently **the least positive representative** is $\boxed{28}$.

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
