<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Jacobson radical](../../../../../jacobson-radical.md) is

$$
J(R)=\bigcap_{L\text{ maximal left ideal}}L
=\bigcap_{V\text{ simple left module}}\operatorname{Ann}_R(V).
$$

Here the second intersection ranges over isomorphism classes of nonzero [simple modules](../../../../../irreducible-module.md). For the equality, every nonzero $v$ in a [simple module](../../../../../irreducible-module.md) gives a [surjective](../../../../../surjective-function.md) [module homomorphism](../../../../../module-homomorphism.md) $R\to V$, $r\mapsto rv$, whose [kernel](../../../../../kernel-of-a-linear-map-split.md) is a [maximal left ideal](../../../../../maximal-left-ideal.md). Conversely, every [maximal left ideal](../../../../../maximal-left-ideal.md) $L$ gives the [simple module](../../../../../irreducible-module.md) $R/L$. This description by [annihilators](../../../../../annihilator-ring-theory.md) shows that $J(R)$ is a two-sided [ideal](../../../../../ideal.md).

Let $j\in J(R)$ and put $a=1+j$. If the [left ideal](../../../../../left-ideal.md) $Ra$ were proper, it would lie in a [maximal left ideal](../../../../../maximal-left-ideal.md) $L$. Both $a$ and $j$ would belong to $L$, giving $1\in L$, a contradiction. Therefore there is $u\in R$ with $ua=1$.

A left inverse alone need not be a two-sided inverse in a general [ring](../../../../../ring.md), so one more step is necessary. The equality $u(1+j)=1$ gives $u=1-uj\in1+J(R)$. Applying the same argument to $u$ supplies $v\in R$ with $vu=1$. Then

$$
v=v(ua)=(vu)a=a,
$$

and hence $au=vu=1$. Thus

$$
\boxed{1+J(R)\subseteq R^\times.}
$$

For the [zero ring](../../../../../zero-ring.md) the conclusion holds directly; the [maximal left ideal](../../../../../maximal-left-ideal.md) argument concerns the nonzero case.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the non-commutative rings course of the University of Oxford](../../../../split.md)
6. [Non-commutative rings course of the University of Oxford](../../../../../non-commutative-rings-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
