<h1 id="9g/solution">Solution</h1>

↑ **Parent:** [9G](../9g.md)

The [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) is $d=b^2-4ac$; it is unchanged by a [unimodular matrix](../../../../../unimodular-matrix.md) change of integral variables and satisfies $d\equiv0$ or $1\pmod4$. For such a $d$, the [discriminant criterion for prime representation by a binary quadratic form](../../../../../discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form.md) says that some integral [binary quadratic form](../../../../../binary-quadratic-form.md) of [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) $d$ represents an odd [prime](../../../../../prime-number.md) $p$ exactly when $d$ is a square modulo $p$, including zero. Equivalently,

$$
\boxed{\text{there is an integer }B\text{ with }B^2\equiv d\pmod{4p}.}
$$

These versions agree: a square root modulo $p$ can be chosen even when $d\equiv0\pmod4$ and odd when $d\equiv1\pmod4$, by adding $p$ if needed, and then the [Chinese remainder theorem](../../../../../chinese-remainder-theorem.md) applies.

For completeness, if $f(x,y)=p$, then $(x,y)$ is primitive, since any common divisor would have its square divide $p$. Complete $(x,y)$ to a basis of $\mathbb Z^2$ with [determinant](../../../../../determinant.md) one using [Bézout's identity](../../../../../bezout-identity.md). The transformed [binary quadratic form](../../../../../binary-quadratic-form.md) has leading coefficient $p$ and [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) $B^2-4pC=d$. Conversely, a suitable $B$ makes $[p,B,(B^2-d)/(4p)]$ an integral [binary quadratic form](../../../../../binary-quadratic-form.md) representing $p$ at $(1,0)$.

For $x^2+3y^2$, the [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) is $-12$. The [prime](../../../../../prime-number.md) $3$ is represented. If $p\ne3$ is represented, reducing modulo $3$ gives $p\equiv x^2\equiv1\pmod3$, which also excludes $p=2$. To prove sufficiency for $p\equiv1\pmod3$, [quadratic reciprocity](../../../../../quadratic-reciprocity.md) gives

$$
\left(\frac{-3}{p}\right)=\left(\frac{-1}{p}\right)\left(\frac3p\right)=\left(\frac p3\right)=1.
$$

The criterion constructs a positive definite [binary quadratic form](../../../../../binary-quadratic-form.md) $[p,B,C]$ of [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) $-12$. It is primitive: a common divisor of its coefficients would divide $p$, and if that divisor were $p$, then $p^2$ would divide $12$, impossible for $p\ne2,3$.

We must still establish that this form is equivalent to $x^2+3y^2$, rather than merely some form of the same [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md). In a positive definite integral [binary quadratic form](../../../../../binary-quadratic-form.md), replace $x$ by $x+ky$ to arrange $|b|\leq a$. If $c<a$, apply $(x,y)\mapsto(-y,x)$ and repeat. Each such exchange strictly decreases the positive integer leading coefficient, so this [reduction algorithm for a positive definite binary quadratic form](../../../../../reduction-algorithm-for-a-positive-definite-binary-quadratic-form.md) terminates with $|b|\leq a\leq c$. Then $12=4ac-b^2\geq3a^2$, so $a\leq2$. With $a=1$, parity forces $b=0$, giving $c=3$. With $a=2$, the only integral choices are $b=\pm2,c=2$, and these are not primitive. Thus every primitive positive definite [binary quadratic form](../../../../../binary-quadratic-form.md) of [discriminant of a binary quadratic form](../../../../../discriminant-of-a-binary-quadratic-form.md) $-12$ is equivalent to $[1,0,3]$, and preserves its represented integers. Therefore

$$
\boxed{p=x^2+3y^2\text{ for integers }x,y\quad\Longleftrightarrow\quad p=3\text{ or }p\equiv1\pmod3.}
$$

## ↑ Ancestors (10)

1. [9G](../9g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
