<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose a generator $u$ of the [cyclic group](../../../../../cyclic-group.md) $U(R)$, so $u^p=1$. Part (a)(iii) gives a unital [ring homomorphism](../../../../../ring-homomorphism.md) $\mathbb F_2\to R$. Its image lies in the centre of $R$, so even if $R$ is not a [commutative ring](../../../../../commutative-ring.md), evaluating a [polynomial](../../../../../polynomial-split.md) at $u$ defines a [ring homomorphism](../../../../../ring-homomorphism.md)

$$
\phi:\mathbb F_2[X]\longrightarrow R,\qquad\sum_ja_jX^j\longmapsto\sum_ja_ju^j.
$$

Because $\phi(X^p-1)=0$, it factors through the [quotient ring](../../../../../quotient-ring.md) to give

$$
\boxed{\overline\phi:\mathbb F_2[X]/(X^p-1)\longrightarrow R,\qquad\overline X\longmapsto u}.
$$

Its image is the [subring](../../../../../subring.md) $S=\mathbb F_2[u]$. Every [unit](../../../../../unit-in-a-ring.md) of $S$ is a [unit](../../../../../unit-in-a-ring.md) of $R$, because an inverse in $S$ also lies in $R$. Conversely, every member of $U(R)$ is $u^j$ for some $j$, and both $u^j$ and its inverse $u^{p-j}$ lie in $S$. Hence

$$
\boxed{U(S)=U(R)}.
$$

The inverse argument matters: merely belonging to a [subring](../../../../../subring.md) would not by itself make an ambient [unit](../../../../../unit-in-a-ring.md) invertible there.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
