<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

Suppose first that a simple [continued fraction](../../../../../continued-fraction.md) is eventually periodic. Its periodic tail $\xi$ is fixed by the [Möbius transformation](../../../../../mobius-transformation.md) represented by the [continued-fraction matrix](../../../../../continued-fraction-matrix.md) of one full period:

$$
\xi=\frac{a\xi+b}{c\xi+d}.
$$

Thus

$$
c\xi^2+(d-a)\xi-b=0.
$$

The infinite tail is not [rational](../../../../../rational-number.md), since a rational simple continued fraction terminates. Hence $\xi$ is a [quadratic irrational](../../../../../quadratic-irrational-number.md), and the finite initial block expresses the original number as another rational Möbius transform of $\xi$. Therefore **every eventually periodic simple continued fraction represents a quadratic irrational**.

For the purely periodic fraction $x=[7,7,7,\ldots]$,

$$
x=7+\frac1x,
$$

so $x^2-7x-1=0$. Positivity selects

$$
\boxed{x=\frac{7+\sqrt{53}}2.}
$$

Apply the [continued-fraction algorithm](../../../../../continued-fraction-algorithm.md) to $\sqrt{23}$:

$$
\sqrt{23}
=4+\frac1{\frac{\sqrt{23}-4}{1}}
=4+\cfrac1{1+\cfrac1{3+\cfrac1{1+\cfrac1{8+\cdots}}}}.
$$

The complete quotient then repeats, giving

$$
\boxed{\sqrt{23}=[4;\overline{1,3,1,8}].}
$$

The [convergents](../../../../../continued-fraction-convergent.md) through one term before the final $8$ are

$$
4,\quad5,\quad\frac{19}{4},\quad\frac{24}{5}.
$$

The last of these satisfies the [Pell equation](../../../../../pell-equation.md)

$$
24^2-23\cdot5^2=576-575=1,
$$

so a positive solution is

$$
\boxed{(x,y)=(24,5).}
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
