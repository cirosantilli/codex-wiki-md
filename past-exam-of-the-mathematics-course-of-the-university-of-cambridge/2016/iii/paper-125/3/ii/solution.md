<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

In fact, **$2,3,5,7$ must all be primes of bad reduction**.

At a prime of [good reduction of an elliptic curve](../../../../../../good-reduction-of-an-elliptic-curve.md), the kernel $E_1(\mathbb Q_p)$ of reduction is the [formal group of an elliptic curve](../../../../../../formal-group-of-an-elliptic-curve.md) evaluated on $p\mathbb Z_p$, using its parameter at the identity. This kernel has no prime-to-$p$ torsion: for an integer $\ell$ prime to $p$, the multiplication series is $[\ell]_F(T)=\ell T+$ higher-degree integral terms, so for nonzero $T\in p\mathbb Z_p$ its first term has strictly smaller valuation than the others and $[\ell]_F(T)\ne0$.

For each odd good prime, the entire given torsion subgroup, of order $16$, would therefore inject into $E(\mathbb F_p)$. But the [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md) gives

$$
\#E(\mathbb F_3)\leq7,\qquad\#E(\mathbb F_5)\leq10,\qquad\#E(\mathbb F_7)\leq13.
$$

None can contain a subgroup of order $16$. Hence $3,5,7$ are bad.

For the [prime-two torsion bound for good reduction](../../../../../../prime-two-torsion-bound-for-good-reduction.md), use the deeper formal subgroup corresponding to $4\mathbb Z_2$. Part (i), with $m=2>1/(2-1)$, shows that $E_2(\mathbb Q_2)$ is torsion-free and has index $2$ in $E_1(\mathbb Q_2)$. Therefore any finite torsion subgroup of $E_1(\mathbb Q_2)$ injects into $E_1/E_2$ and has order at most $2$.

If $E$ had good reduction at $2$, its rational torsion subgroup of order $16$ would consequently have reduction image of order at least $8$. The [Hasse theorem for elliptic curves](../../../../../../hasse-s-theorem-on-elliptic-curves.md) instead gives $\#E(\mathbb F_2)\leq5$. This contradiction proves bad reduction at $2$ as well, and therefore

$$
\boxed{\#\{\text{bad reduction primes of }E\}\geq4.}
$$

The special formal-group argument at $2$ is necessary; prime-to-$p$ injectivity alone says nothing about the given $2$-primary torsion there.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
