<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [elliptic-curve discriminant](../../../../../../elliptic-curve-discriminant.md) is supported at $2$ and $3$, so $5$ and $7$ are primes of [good reduction](../../../../../../good-reduction-of-an-elliptic-curve.md). Direct point counts give

$$
\#\widetilde E(\mathbb F_5)=8,
\qquad
\#\widetilde E(\mathbb F_7)=8.
$$

For example, summing $1+\chi_p(x(x+1)(x+4))$ over $x\in\mathbb F_p$ and adding the point at infinity gives these values.

The [reduction of torsion points on an elliptic curve](../../../../../../reduction-of-torsion-points-on-an-elliptic-curve.md) at the two primes shows that $|E(\mathbb Q)_{\mathrm{tors}}|$ divides eight. Part (a) shows that $P_2$ has order four, and $P_1$ is an independent point of order two because it does not lie in $\langle P_2\rangle$. They already generate eight points, so

$$
\boxed{E(\mathbb Q)_{\mathrm{tors}}=\langle P_2\rangle\oplus\langle P_1\rangle
\cong\mathbb Z/4\mathbb Z\oplus\mathbb Z/2\mathbb Z.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
