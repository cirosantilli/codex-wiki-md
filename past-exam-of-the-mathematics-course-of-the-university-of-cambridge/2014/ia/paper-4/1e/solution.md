<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [Euclidean algorithm](../../../../../euclidean-algorithm.md) gives

$$
203=147+56,\quad147=2\cdot56+35,\quad56=35+21,\quad35=21+14,\quad21=14+7,\quad14=2\cdot7.
$$

Thus the [greatest common divisor](../../../../../greatest-common-divisor.md) is **$d=7$**. The [extended Euclidean algorithm](../../../../../extended-euclidean-algorithm.md) reverses these divisions:

$$
7=21-14=2\cdot21-35=2\cdot56-3\cdot35=8\cdot56-3\cdot147=8\cdot203-11\cdot147.
$$

This supplies the [Bezout identity](../../../../../bezout-identity.md) with $x=8$, $y=-11$.

To obtain [all solutions of a linear Diophantine equation](../../../../../all-solutions-of-a-linear-diophantine-equation.md), subtract this particular solution from any other and divide by $7$. The result is $29(x-8)+21(y+11)=0$. Since $29$ and $21$ are [coprime integers](../../../../../coprime-integers.md), $21$ divides $x-8$, giving

$$
\boxed{x=8+21t,\qquad y=-11-29t,\qquad t\in\mathbb Z.}
$$

Every displayed pair satisfies the original [linear Diophantine equation](../../../../../linear-diophantine-equation.md), so the parametrization is exhaustive.

For the [modular arithmetic](../../../../../modular-arithmetic.md) calculation, $21\cdot18=378\equiv1\pmod{29}$, so $18$ is the [modular inverse](../../../../../modular-multiplicative-inverse.md) of $21$. Multiplication gives $n\equiv25\cdot18\equiv15\pmod{29}$. The admissible [integers](../../../../../integer.md) are $15+29t$ for $0\leq t\leq68$, ending at $1987$; the next is $2016$. **There are $\boxed{69}$ such integers.**

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
