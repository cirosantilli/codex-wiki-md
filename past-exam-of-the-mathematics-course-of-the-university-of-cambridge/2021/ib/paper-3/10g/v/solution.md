<h1 id="10g/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

By the [prime ideal quotient criterion](../../../../../../prime-ideal-quotient-criterion.md),

$$
R/(p)\text{ is an integral domain}
\quad\Longleftrightarrow\quad
(p)\text{ is a prime ideal}.
$$

For a principal ideal, this is precisely the assertion that $p$ is a prime element. This closes the cycle and proves that (i)--(v) are equivalent.

Now let $\varphi:R\to S$ be a surjective ring homomorphism, where $R$ is a [principal ideal domain](../../../../../../principal-ideal-domain.md) and $S$ is an integral domain. Write

$$
\ker\varphi=(a).
$$

If $a=0$, the [first isomorphism theorem for rings](../../../../../../first-isomorphism-theorem-for-rings.md) makes $\varphi$ an isomorphism. Otherwise

$$
S\cong R/(a)
$$

is an integral domain, so the equivalences just proved show that $(a)$ is maximal and $S$ is a field.

Next suppose that the [polynomial ring](../../../../../../polynomial-ring.md) $R[X]$ is a principal ideal domain. It follows first that $R$ is an integral domain. For nonzero $a\in R$, the ideal

$$
(a,X)=(f)
$$

is principal. Since $f$ divides the nonzero constant $a$, it is constant; since it also divides $X$, that constant divides the coefficient $1$, so $f$ is a unit. Therefore $(a,X)=R[X]$, and there are polynomials $g,h$ such that

$$
1=ag(X)+Xh(X).
$$

Setting $X=0$ gives $1=ag(0)$, so every nonzero $a\in R$ is a unit. Hence

$$
\boxed{R\text{ is a field}}.
$$

Finally, let $R$ be an integral domain in which every two nonzero elements have a [greatest common divisor](../../../../../../greatest-common-divisor.md). If an irreducible $p$ divides $ab$, then $\gcd(p,a)$ is either a unit or an associate of $p$. In the second case $p\mid a$. In the first case, the [Euclid lemma in a greatest-common-divisor domain](../../../../../../euclid-lemma-in-a-greatest-common-divisor-domain.md) gives $p\mid b$. Thus every irreducible element of $R$ is prime.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [10G](../../10g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
