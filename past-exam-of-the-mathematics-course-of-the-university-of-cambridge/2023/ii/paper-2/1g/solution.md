<h1 id="1g/solution">Solution</h1>

↑ **Parent:** [1G](../1g.md)

The [Lagrange root bound over a field](../../../../../lagrange-root-bound-over-a-field.md) says that a nonzero [polynomial](../../../../../polynomial-split.md) of [degree](../../../../../degree-of-a-polynomial.md) $r$ over a [field](../../../../../field.md) has at most $r$ roots. In particular, a polynomial [modular congruence](../../../../../modular-congruence.md) of degree $r$ modulo a [prime number](../../../../../prime-number.md) has at most $r$ incongruent solutions unless all its coefficients vanish modulo that prime.

Suppose that $d$ is good and that the positive [integer divisor](../../../../../divisor.md) $e$ divides $d$. The $d$ roots of $X^d-1$ form a finite multiplicative [subgroup](../../../../../subgroup.md) $H$ of $\mathbb F_p^\times$. By the fact that every [finite multiplicative subgroup of a field is cyclic](../../../../../finite-multiplicative-subgroup-of-a-field-is-cyclic.md), $H=\langle g\rangle$ is a [cyclic group](../../../../../cyclic-group.md) of order $d$. The solutions in $H$ of $x^e=1$ are

$$
1,g^{d/e},g^{2d/e},\ldots,g^{(e-1)d/e},
$$

so there are at least $e$ of them. The [Lagrange root bound over a field](../../../../../lagrange-root-bound-over-a-field.md) gives at most $e$ roots in all of $\mathbb F_p$, hence exactly $e$. Thus every divisor of a good number is good.

Now put $n=pq$. By the [Chinese remainder theorem for unit groups](../../../../../chinese-remainder-theorem-for-unit-groups.md), a base $b$ is a [Fermat-pseudoprime](../../../../../fermat-pseudoprime.md) base precisely when its two components satisfy

$$
b^{n-1}=1\quad\hbox{in }\mathbb F_p^\times
\qquad\hbox{and}\qquad
b^{n-1}=1\quad\hbox{in }\mathbb F_q^\times.
$$

The [power roots in a finite field](../../../../../power-roots-in-a-finite-field.md) and

$$
\gcd(n-1,p-1)=\gcd(q-1,p-1)=10,
\qquad
\gcd(n-1,q-1)=\gcd(p-1,q-1)=10
$$

show that each component has ten choices. Therefore there are

$$
10\cdot10=100
$$

Fermat-pseudoprime bases.

To impose the [strong pseudoprime](../../../../../strong-pseudoprime.md) condition, write $n-1=2^s m$ with $m$ odd. Since $10\mid n-1$, we have $5\mid m$. In each cyclic group of ten Fermat components, raising to the $m$th power sends five elements to $1$ and five elements to $-1$. A pair of components passes the strong test exactly when their signs agree: the pair $(1,1)$ satisfies the first alternative, and $(-1,-1)$ satisfies the second at $j=0$. Components of opposite sign become $(1,1)$ after squaring and can never jointly equal $-1$. Hence the number of strong-pseudoprime bases is

$$
\boxed{5^2+5^2=50.}
$$

## ↑ Ancestors (10)

1. [1G](../1g.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
