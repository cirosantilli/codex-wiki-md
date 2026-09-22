<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

**The exact orders printed in the question are inconsistent.** The source PDF says that the [orders of group elements](../../../../order-of-a-group-element.md) $a,b,c$ are $4,12,24$, respectively, and also imposes $3a+2b=0$. Multiplying this relation by $6$ and using $12b=0$ gives $18a=0$. Since $4a=0$ also holds, subtracting $4(4a)=0$ gives $2a=0$, contradicting the stated [order of a group element](../../../../order-of-a-group-element.md) $4$. Thus

$$
\boxed{\text{no group satisfies all the hypotheses literally as printed}}.
$$

The natural [abelian group presentation](../../../../abelian-group-presentation.md) interpretation is to impose the relations $4a=12b=24c=0$ and $3a+2b=0$, with no further relations, without requiring the orders of the images of the generators to stay $4,12,24$. Under this interpretation the calculation is as follows. Since $3a=-a$ follows from $4a=0$, the mixed relation gives $a=2b$. Consequently $8b=0$, and together with $12b=0$ this gives $4b=0$. Conversely, $a=2b$, $4b=0$, and $24c=0$ imply every original relation. Eliminating $a$ leaves two independent [cyclic groups](../../../../cyclic-group.md):

$$
\boxed{G_{\mathrm{pres}}\cong\mathbb Z_4\oplus\mathbb Z_{24},\qquad n=2,\quad d_1=4,\quad d_2=24}.
$$

To verify that these relations force no further identifications, map $a,b,c$ to $(2,0),(1,0),(0,1)$ in $\mathbb Z_4\oplus\mathbb Z_{24}$. All defining relations hold, and the inverse [group homomorphism](../../../../group-homomorphism.md) sends the two standard generators to $b,c$. These [group homomorphisms](../../../../group-homomorphism.md) are mutually inverse. The [divisibility](../../../../divisibility-split.md) condition $4\mid24$ gives the requested [invariant factors of a finitely generated module](../../../../invariant-factor-of-a-finitely-generated-module.md) over $\mathbb Z$. In this presented [group](../../../../group-split.md), $a,b,c$ actually have orders $2,4,24$.

Equivalently, the relation [matrix](../../../../matrix.md)

$$
\begin{pmatrix}4&0&0\\0&12&0\\0&0&24\\3&2&0\end{pmatrix}
$$

has nonzero [Smith normal form](../../../../smith-normal-form.md) entries $1,4,24$, with the trivial $\mathbb Z_1$ factor omitted. The displayed [direct sum of modules](../../../../direct-sum-of-modules.md) is the answer to the presentation interpretation; the inconsistency of the literal exact-order formulation remains.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the rings and modules course of the University of Oxford](../../../split.md)
5. [Rings and modules course of the University of Oxford](../../../../rings-and-modules-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
