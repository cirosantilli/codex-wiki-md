<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

We bound the [torsion subgroups](../../../../../../torsion-subgroup.md) by [reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md). At a prime $p$ of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), reduction is injective on the prime-to-$p$ torsion. Indeed, a point in the kernel is represented by the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) on the maximal ideal. Multiplication by an integer prime to $p$ has a unit linear coefficient and is invertible there, so the kernel has no nonzero torsion of such order.

Both curves have [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md) at $2$ and $5$. For $E$ this follows from $\Delta=-91^3$, which is a unit at both primes. For $E'$ at $2$, its reduction is $x^3+y^3+z^3=0$ and its three partial derivatives cannot vanish at a projective point. At $5$, the singularity calculation in part (i) would require $351-8=343$ to vanish modulo $5$, which it does not; $3$ and $13$ are also units there.

Direct counting gives:

| Curve | Affine over $\mathbb F_2$ | At infinity | Total | Affine over $\mathbb F_5$ | At infinity | Total |
| --- | --- | --- | --- | --- | --- | --- |
| $E$ | $2$ | $1$ | $3$ | $8$ | $1$ | $9$ |
| $E'$ | $2$ | $1$ | $3$ | $8$ | $1$ | $9$ |

For $E$ over $\mathbb F_5$, the numbers of ordinate solutions at $x=0,1,2,3,4$ are $2,2,2,2,0$. For $E'$ in the chart $z=1$, they are $1,2,0,3,2$, with the single infinity point $(1:-1:0)$. These give the displayed totals without identifying the finite-field groups through the given [isogeny of elliptic curves](../../../../../../isogeny-of-elliptic-curves.md).

For either rational [torsion subgroup](../../../../../../torsion-subgroup.md), every odd-primary part injects at $2$, so the whole odd torsion has order dividing three. The two-primary part injects at $5$ and must be trivial, since the reduced group has odd order nine. Thus either rational [torsion subgroup](../../../../../../torsion-subgroup.md) has order at most three. For $E$, the point $P$ already has order three, so

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\{O,(0,0),(0,13)\}\cong\mathbb Z/3\mathbb Z.}
$$

For the plane cubic $E'$, the chosen identity $O'$ is a [plane cubic flex](../../../../../../inflection-point-of-a-plane-cubic.md). The fact that [three-torsion points are flexes of a plane cubic](../../../../../../three-torsion-points-are-flexes-of-a-plane-cubic.md) therefore identifies $E'[3]$ with its nine geometric flexes. Part (i) found only the identity among the rational flexes. No nonidentity rational three-torsion exists, and the preceding bound excludes every other order. Hence

$$
\boxed{E'(\mathbb Q)_{\mathrm{tors}}=\{O'\}.}
$$

This also illustrates that [isogenous elliptic curves can have different rational point groups](../../../../../../isogenous-elliptic-curves-can-have-different-rational-point-groups.md); the given degree-three isogeny does not imply equality of rational torsion.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
