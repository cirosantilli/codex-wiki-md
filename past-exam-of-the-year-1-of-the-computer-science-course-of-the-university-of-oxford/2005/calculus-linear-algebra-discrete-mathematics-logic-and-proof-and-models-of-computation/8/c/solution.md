<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the direction of the [divisibility](../../../../../divisibility-split.md) relation matters: $R(x,z)$ means $z\mid x$. The first two clauses say that $z$ is a common [divisor](../../../../../divisor.md) of $x,y$. The last clause says that every common [divisor](../../../../../divisor.md) $w$ divides $z$. These are precisely the defining properties of the [greatest common divisor](../../../../../greatest-common-divisor.md). Choose $z=\gcd(x,y)$; then

$$
z\mid x,\quad z\mid y,\qquad (w\mid x\land w\mid y)\Longrightarrow w\mid z.
$$

Hence

$$
\boxed{\mathbf N'\models\psi.}
$$

This also holds if the [natural numbers](../../../../../natural-number.md) include zero: use $\gcd(x,0)=x$ and $\gcd(0,0)=0$. Every [natural number](../../../../../natural-number.md) divides zero, so for $x=y=z=0$ the last clause remains true. In the order obtained by reversing [divisibility](../../../../../divisibility-split.md), the [greatest common divisor](../../../../../greatest-common-divisor.md) is the [least upper bound](../../../../../least-upper-bound-in-a-partially-ordered-set.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [8](../../8.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
