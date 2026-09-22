<h1 id="10g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write an integral [binary quadratic form](../../../../../../binary-quadratic-form.md) as $Q(u,v)=Au^2+Buv+Cv^2$, with [discriminant of a binary quadratic form](../../../../../../discriminant-of-a-binary-quadratic-form.md) $d=B^2-4AC$. If $Q(u,v)=p$ is [prime](../../../../../../prime-number.md), then $\gcd(u,v)=1$: any common [divisor](../../../../../../divisor.md) would have its square dividing $p$. Complete $(u,v)$ to a matrix in $\operatorname{SL}_2(\mathbb Z)$ using [Bezout identity](../../../../../../bezout-identity.md). After the associated integral [change of variables](../../../../../../change-of-variables-formula.md), the properly equivalent form has leading coefficient $p$, say $[p,b,c]$. Its [discriminant of a binary quadratic form](../../../../../../discriminant-of-a-binary-quadratic-form.md) gives $d=b^2-4pc$, hence $b^2\equiv d\pmod p$.

Conversely suppose $b_0^2\equiv d\pmod p$. Since $d$ is an integral-form [discriminant of a binary quadratic form](../../../../../../discriminant-of-a-binary-quadratic-form.md), $d\equiv0$ or $1\pmod4$. Choose $b\equiv b_0\pmod p$ with even [integer parity](../../../../../../parity-mathematics.md) for $d\equiv0\pmod4$ and odd [integer parity](../../../../../../parity-mathematics.md) for $d\equiv1\pmod4$. This is possible because $p$ is odd. Then $b^2-d$ is divisible by $4p$, and

$$
\boxed{Q(u,v)=pu^2+buv+\frac{b^2-d}{4p}v^2}
$$

is an integral form of [discriminant of a binary quadratic form](../../../../../../discriminant-of-a-binary-quadratic-form.md) $d$ representing $p=Q(1,0)$. This proves the [discriminant criterion for prime representation by a binary quadratic form](../../../../../../discriminant-criterion-for-prime-representation-by-a-binary-quadratic-form.md), including the case $p\mid d$; no assumption that $d$ is a [fundamental discriminant](../../../../../../fundamental-discriminant.md) was used.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [10G](../../10g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
