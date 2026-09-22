<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

**No.** Write $x_i=t_i+I$ in the [quotient ring](../../../../quotient-ring.md) $R=L/I$. Its defining relations are

$$
x_1^2=0,\qquad x_i=x_{i+1}^2\quad(i\geq1).
$$

Consequently $x_i^{2^{i-1}}=x_1\ne0$, using the permitted assumption, while $x_i^{2^i}=0$. Thus every $x_i$ is a nonzero [nilpotent element](../../../../nilpotent.md).

The [principal ideals](../../../../principal-ideal.md) satisfy

$$
(x_1)\subseteq(x_2)\subseteq(x_3)\subseteq\cdots.
$$

Every inclusion is strict. Otherwise $x_{i+1}=a x_i=a x_{i+1}^2$ for some $a\in R$, and hence

$$
x_{i+1}(1-a x_{i+1})=0.
$$

The fact that [one minus a nilpotent element is a unit](../../../../one-minus-a-nilpotent-element-is-a-unit.md) applies: if $z^m=0$, then $(1-z)(1+z+\cdots+z^{m-1})=1$. Here $z=a x_{i+1}$ is [nilpotent](../../../../nilpotent.md), so multiplication by this inverse would give $x_{i+1}=0$, a contradiction. The strictly ascending chain of [ideals](../../../../ideal.md) violates the [ascending chain condition](../../../../ascending-chain-condition.md). Therefore

$$
\boxed{L/I\text{ is not Noetherian}.}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the commutative algebra course of the University of Oxford](../../../split.md)
5. [Commutative algebra course of the University of Oxford](../../../../commutative-algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
