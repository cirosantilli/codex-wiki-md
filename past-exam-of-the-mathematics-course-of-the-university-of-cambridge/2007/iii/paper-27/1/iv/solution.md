<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Set $d=-7$. The affine rational pair $(u,v)=(2,-1)$ gives $P=(84,756)$ on the [elliptic curve](../../../../../../elliptic-curve.md) $y^2=x^3-21168$. It is a point of infinite order: in the [rational torsion of a diagonal cubic](../../../../../../rational-torsion-of-a-diagonal-cubic.md) classification, neither $-7$ nor $-7/2$ is a rational cube, so this curve has trivial rational [torsion subgroup](../../../../../../torsion-subgroup.md).

There is also a short direct torsion check specific to this curve. The [primes](../../../../../../prime-number.md) $5$ and $11$ are good and have point counts $6$ and $12$, respectively, because cubing is bijective in their [finite fields](../../../../../../finite-field.md). Reduction at these two [primes](../../../../../../prime-number.md) bounds the entire rational torsion by order dividing $6$, including its possible $5$- and $11$-primary parts by reduction at the other [prime](../../../../../../prime-number.md). The flex calculation excludes order $3$, and the inversion calculation excludes order $2$. Hence $P$ is indeed nontorsion.

Every nonzero multiple $nP$ is distinct, and its inverse projective image has $Z\ne0$: the only [rational point](../../../../../../rational-point.md) at infinity on the diagonal cubic is its identity. Thus each yields a distinct rational pair. More explicitly, if $nP=(x_n,y_n)$ on the [Weierstrass model](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), then

$$
\boxed{u_n=\frac{y_n+252}{6x_n},\qquad v_n=\frac{252-y_n}{6x_n},\qquad u_n^3+v_n^3=7\quad(n\ge1).}
$$

Here $x_n\ne0$, since $x_n=0$ would require a rational square equal to $-21168$. For example the [elliptic-curve addition formula](../../../../../../elliptic-curve-addition-formula.md) gives $2P=(28,28)$, which produces $(u_2,v_2)=(5/3,4/3)$. This proves **there are infinitely many rational pairs of cubes summing to seven**.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
