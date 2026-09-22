<h1 id="10e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $G=\mathbb F_p^\times$, and let $m$ be the least common multiple of the orders of its elements. For every prime power $q^a$ dividing $m$, some element of $G$ has order divisible by $q^a$, and a suitable power of it has order exactly $q^a$. Multiplying these elements over the distinct primes produces, because their orders are coprime, an element of order $m$.

Every element of $G$ is a root of $X^m-1$. A nonzero [polynomial](../../../../../../polynomial-split.md) of degree $m$ over a field has at most $m$ roots, so $p-1\leq m$. On the other hand, every element order divides $p-1$ by Lagrange's theorem, so $m\leq p-1$. Hence $m=p-1$, and

$$
\boxed{\mathbb F_p^\times\text{ is cyclic}}.
$$

The squaring homomorphism has kernel $\{1,-1\}$ because $p$ is odd. Its image $H$ therefore has order $(p-1)/2$ and index two. If $p=3$, then $3=0$ is already a square. Otherwise $2,3\in G$. In the two-element quotient $G/H$, either $2H=H$, or $3H=H$, or both are the nontrivial coset, in which case $6H=H$. Thus one of $2,3,6$ is a square modulo $p$.

Finally,

$$
f(x)=(x^2-2)(x^2-3)(x^2-6).
$$

Whichever of $2,3,6$ is a square supplies a root, so

$$
\boxed{f\text{ has a root in }\mathbb F_p}.
$$

This is the [index-two square-class argument for three related residues](../../../../../../index-two-square-class-argument-for-three-related-residues.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10E](../../10e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
