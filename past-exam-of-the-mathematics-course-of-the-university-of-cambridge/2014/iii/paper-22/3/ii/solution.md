<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We use two precise facts about the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md). At a [prime](../../../../../../prime-number.md) $p$ of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), its [kernel of reduction of an elliptic curve](../../../../../../kernel-of-reduction-of-an-elliptic-curve.md) is identified by the [uniformizer](../../../../../../uniformizer.md) $t=-x/y$ with the group $\widehat E(p\mathbb Z_p)$. For odd $p$ this group is torsion-free. To see the second fact, the integral [invariant differential of a formal group law](../../../../../../invariant-differential-of-a-formal-group-law.md) has the form $(1+\sum_{j\geq1}c_jT^j)dT$, with $c_j\in\mathbb Z_p$. Integrating constructs the [formal logarithm](../../../../../../formal-logarithm.md)

$$
\log_F(T)=T+\sum_{j\geq2}d_jT^j/j,\qquad d_j\in\mathbb Z_p.
$$

It is a [group homomorphism](../../../../../../group-homomorphism.md) to the [additive group](../../../../../../additive-group.md). For $0\ne t\in p\mathbb Z_p$ and $j\geq2$,

$$
v_p(d_jt^j/j)\geq jv_p(t)-v_p(j)>v_p(t)
$$

when $p$ is odd. Hence the series converges and $v_p(\log_F(t))=v_p(t)$, so it is injective. The target has no nonzero torsion. Therefore reduction is injective on the entire rational [torsion subgroup](../../../../../../torsion-subgroup.md) at an odd [prime](../../../../../../prime-number.md) of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md), including its $p$-primary part.

For the present [elliptic curve](../../../../../../elliptic-curve.md), $\Delta=64D^6$, so every odd $p\nmid D$ is a [prime](../../../../../../prime-number.md) of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md). If $p\equiv3\pmod4$, the [Legendre symbol](../../../../../../legendre-symbol.md) of $-1$ is $-1$. The values $x$ and $-x$ cancel in the sum of the [Legendre symbols](../../../../../../legendre-symbol.md) of $x^3-D^2x$, yielding

$$
\#E(\mathbb F_p)=p+1.
$$

The rational [torsion subgroup](../../../../../../torsion-subgroup.md) injects into each of these groups, so it is finite and its order $M$ divides every such $p+1$.

For any odd [prime](../../../../../../prime-number.md) $\ell$, the [Dirichlet theorem on primes in arithmetic progressions](../../../../../../dirichlet-s-theorem-on-arithmetic-progressions.md) supplies infinitely many $p$ with $p\equiv3\pmod4$ and $p\equiv1\pmod\ell$. Discard the finitely many dividing $D$. Since $\ell\nmid p+1$, it cannot divide $M$. Similarly choose $p\equiv3\pmod8$, again avoiding $D$; then $v_2(p+1)=2$, so $M\mid4$.

There are already four rational [2-torsion](../../../../../../2-torsion.md) points,

$$
O,\quad(0,0),\quad(D,0),\quad(-D,0),
$$

which are distinct because a squarefree integer $D$ is nonzero. Thus

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=E(\mathbb Q)[2]\cong(\mathbb Z/2\mathbb Z)^2.}
$$

**Its order is four.** In fact the argument works for every nonzero integer $D$; squarefreeness is not needed for this torsion conclusion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
