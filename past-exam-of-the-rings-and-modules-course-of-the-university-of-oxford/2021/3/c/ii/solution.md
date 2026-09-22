<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $q=|\mathbb F|$. The [unit group](../../../../../unit-group.md) $U(\mathbb F)=\mathbb F\setminus\{0\}$ is a [finite abelian group](../../../../../finite-abelian-group.md) of [group order](../../../../../order-of-a-finite-group.md) $q-1$, since [multiplication](../../../../../multiplication.md) in a [field](../../../../../field.md) satisfies [commutativity](../../../../../commutativity.md). The [structure theorem for finitely generated abelian groups](../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md), applied to this finite [group](../../../../../group-split.md), gives [invariant factors of a finitely generated module](../../../../../invariant-factor-of-a-finitely-generated-module.md)

$$
U(\mathbb F)\cong\mathbb Z_{d_1}\oplus\cdots\oplus\mathbb Z_{d_r},\qquad
1<d_1\mid d_2\mid\cdots\mid d_r,
$$

after omitting trivial factors. If there are no factors, the [unit group](../../../../../unit-group.md) is trivial and hence a [cyclic group](../../../../../cyclic-group.md).

Otherwise put $D=d_r$. Every element $u\in U(\mathbb F)$ satisfies $u^D=1$, because the [order of a group element](../../../../../order-of-a-group-element.md) in each coordinate divides $D$. Hence all $q-1$ distinct nonzero elements of $\mathbb F$ are [roots of a polynomial](../../../../../root-of-a-polynomial.md) $X^D-1$. The [root bound for a polynomial](../../../../../lagrange-root-bound-over-a-field.md) over a [field](../../../../../field.md) gives

$$
q-1\leq D.
$$

For completeness, that bound follows by induction from the [factor theorem](../../../../../factor-theorem.md): if a nonzero [polynomial](../../../../../polynomial-split.md) $f$ vanishes at $a$, write $f=(X-a)g$; every other [root of a polynomial](../../../../../root-of-a-polynomial.md) is a root of $g$, because a [field](../../../../../field.md) has no [zero divisors](../../../../../zero-divisor.md). Each new distinct root therefore uses one unit of [polynomial degree](../../../../../degree-of-a-polynomial.md).

On the other hand, the [group order](../../../../../order-of-a-finite-group.md) in the decomposition is

$$
q-1=d_1\cdots d_r\geq d_r=D.
$$

Equality is forced, so $d_1\cdots d_{r-1}=1$. As every retained factor is greater than $1$, there can be only one. Consequently

$$
\boxed{U(\mathbb F)\cong\mathbb Z_{q-1}\text{ is cyclic}}.
$$

The same proof establishes the more general result [finite multiplicative subgroup of a field is cyclic](../../../../../finite-multiplicative-subgroup-of-a-field-is-cyclic.md). The [square-free integer](../../../../../square-free-integer.md) result in part (c)(i) alone would not suffice, since $q-1$ need not be a [square-free integer](../../../../../square-free-integer.md); the [root bound for a polynomial](../../../../../lagrange-root-bound-over-a-field.md) rules out multiple [invariant factors of a finitely generated module](../../../../../invariant-factor-of-a-finitely-generated-module.md) even then.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the rings and modules course of the University of Oxford](../../../../split.md)
6. [Rings and modules course of the University of Oxford](../../../../../rings-and-modules-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
