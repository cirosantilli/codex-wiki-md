<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The printed input $x^rx^s$ is a genuine typo in the PDF as well as in the TeX: $E$ annihilates every power of $x$, whereas the displayed right-hand side is generally nonzero. The intended input is $x^ry^s$, and the calculation below proves that corrected identity.

The given [comultiplications](../../../../../../comultiplication.md) make $C_q$ a [coalgebra](../../../../../../coalgebra.md), with [counit](../../../../../../counit.md) one on $K,K^{-1},I$ and zero on $E,F$. Write $I_0=p(I)$, $K_0=p(K)$ and $E_0=p(E)$, and similarly for $F$. The [measuring coalgebra](../../../../../../measuring-coalgebra.md) identities are

$$
E_0(ab)=E_0(a)K_0(b)+I_0(a)E_0(b),\qquad
F_0(ab)=F_0(a)I_0(b)+p(K^{-1})(a)F_0(b).
$$

The [group-like elements](../../../../../../group-like-element.md) act multiplicatively. Although the statement omits an explicit specification of $p(I)$, its identity action follows from the other data and the [quantum plane](../../../../../../quantum-plane.md) relation. Applying $E_0$ to $yx=qxy$ gives $qx^2=qI_0(x)x$, so cancellation in the [noncommutative domain](../../../../../../noncommutative-domain.md) gives $I_0(x)=x$. Applying $F_0$ to the same relation gives $qy^2=qyI_0(y)$, so $I_0(y)=y$. Thus $I_0$ is the identity on the entire [quantum plane](../../../../../../quantum-plane.md).

Now $E_0(x^r)=0$ by induction. Suppose $E_0(y^{s-1})=[s-1]xy^{s-2}$. The measuring rule and $y^{s-1}x=q^{s-1}xy^{s-1}$ give

$$
\begin{aligned}
E_0(y^s)
&=E_0(y^{s-1})K_0(y)+y^{s-1}E_0(y)\\
&=\bigl(q^{-1}[s-1]+q^{s-1}\bigr)xy^{s-1}
=[s]xy^{s-1}.
\end{aligned}
$$

The induction starts with $E_0(y)=x$ and $[1]=1$. A final product rule gives

$$
\boxed{p(E)(x^ry^s)=x^r E_0(y^s)=[s]x^{r+1}y^{s-1}.}
$$

For $s=0$ the answer is zero. By contrast the literal printed input has $\boxed{p(E)(x^rx^s)=0}$; it cannot satisfy the printed right-hand side for $s=1$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
