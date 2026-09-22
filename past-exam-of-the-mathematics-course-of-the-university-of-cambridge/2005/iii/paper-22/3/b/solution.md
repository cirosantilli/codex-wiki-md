<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $A=\Sigma^\infty X_+$ and $H=F(A,E)=F(X_+,E)$. The diagonal of $X$ and its map to a point induce

$$
\Delta:A\longrightarrow A\wedge A,\qquad\epsilon:A\longrightarrow\mathbb S.
$$

Here the identification $(X\times X)_+\cong X_+\wedge X_+$ explains the target of $\Delta$. These maps satisfy the coassociativity, cocommutativity and counit identities, since their underlying maps send $x$ to repeated copies of the same $x$.

Use the defining adjunction of the [function spectrum](../../../../../../function-spectrum.md) to define $m:H\wedge H\to H$. Its adjoint is the composite

$$
H\wedge H\wedge A\xrightarrow{1\wedge\Delta}H\wedge H\wedge A\wedge A\xrightarrow{\text{interchange}}(H\wedge A)\wedge(H\wedge A)\xrightarrow{\mathrm{ev}\wedge\mathrm{ev}}E\wedge E\xrightarrow{\mu}E.
$$

Define $u:\mathbb S\to H$ to have adjoint

$$
A\xrightarrow{\epsilon}\mathbb S\xrightarrow{\eta}E.
$$

Thus $m$ is pointwise multiplication, while $u$ is the constant unit. These are genuine stable maps, defined through the internal [function spectrum](../../../../../../function-spectrum.md), so the argument does not presume that stable functions have ordinary points.

To verify associativity, take the adjoints of $m(m\wedge1)$ and $m(1\wedge m)$. Both are maps $H^{\wedge3}\wedge A\to E$. Both use the triple diagonal $A\to A^{\wedge3}$, evaluate the three copies of $H$, and multiply the three outputs. The triple diagonals agree by coassociativity; the output maps agree by associativity of the [ring spectrum](../../../../../../ring-spectrum.md) $E$. The [function spectrum](../../../../../../function-spectrum.md) adjunction therefore makes the original two maps equal. For the left unit, the adjunct of $m(u\wedge1)$ uses $(\epsilon\wedge1)\Delta=1_A$ and $\mu(\eta\wedge1)=1_E$, leaving exactly evaluation. Its adjoint is $1_H$. The same calculation with $(1\wedge\epsilon)\Delta$ proves the right unit. Hence

$$
\boxed{F(X_+,E)\text{ is a ring spectrum}.}
$$

If $E$ is a [commutative ring spectrum](../../../../../../commutative-ring-spectrum.md), cocommutativity of $\Delta$ proves that this [function spectrum](../../../../../../function-spectrum.md) is commutative as well.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
