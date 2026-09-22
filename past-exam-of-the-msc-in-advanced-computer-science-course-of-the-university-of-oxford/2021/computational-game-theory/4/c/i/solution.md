<h1 id="4/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**The [core](../../../../../../core-game-theory.md) is the singleton $\{(1/2,1/2,1/2,1/2)\}$.** Here the [characteristic function of a coalitional game](../../../../../../characteristic-function-of-a-coalitional-game.md) is $v(C)=\lfloor |C|/2\rfloor$, the two-person instance of the [core of the miners game](../../../../../../core-of-the-miners-game.md) calculation.

Let $x$ be in the [core](../../../../../../core-game-theory.md). Efficiency requires $x_1+x_2+x_3+x_4=2$, and every pair [coalition](../../../../../../coalition-game-theory.md) requires $x_i+x_j\ge1$. Summing the six pair inequalities counts each coordinate three times, giving $3\sum_i x_i\ge6$. Efficiency makes this an equality; since every individual slack is nonnegative, all six pair inequalities must be equalities. In particular $x_1+x_2=x_1+x_3=x_1+x_4=1$ forces $x_2=x_3=x_4$, and comparison with $x_2+x_3=1$ gives every $x_i=1/2$.

Conversely, for the uniform allocation every [coalition](../../../../../../coalition-game-theory.md) satisfies

$$
\sum_{i\in C}x_i=\frac{|C|}{2}\ge\left\lfloor\frac{|C|}{2}\right\rfloor=v(C),
$$

and its total is $2=v(N)$. It is therefore a [core](../../../../../../core-game-theory.md) member, completing both existence and uniqueness. In particular, a three-player [coalition](../../../../../../coalition-game-theory.md) receives $3/2\ge1$; the pair constraints are the tight ones.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Computational game theory](../../../../computational-game-theory-split.md)
5. [2021](../../../../split.md)
6. [Past exam of the MSc in advanced computer science course of the University of Oxford](../../../../../split.md)
7. [MSc in advanced computer science course of the University of Oxford](../../../../../../msc-in-advanced-computer-science-course-of-the-university-of-oxford.md)
8. [Master's course of the University of Oxford](../../../../../../master-s-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
