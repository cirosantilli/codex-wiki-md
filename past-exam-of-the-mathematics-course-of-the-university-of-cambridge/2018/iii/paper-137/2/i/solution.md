<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $x=g^{-1}h$ and $S(x)=\sum_{\chi\in\widehat G}\chi(x)$, where $\widehat G$ is the [character group of a finite abelian group](../../../../../../character-group-of-a-finite-abelian-group.md). The [Fundamental theorem of finitely generated abelian groups](../../../../../../fundamental-theorem-of-finitely-generated-abelian-groups.md) writes the [finite group](../../../../../../finite-group.md) $G$ as a product of [cyclic groups](../../../../../../cyclic-group.md). A character of a [cyclic group](../../../../../../cyclic-group.md) factor of order $r$ is determined by an arbitrary $r$th [root of unity](../../../../../../root-of-unity.md), so $|\widehat G|=|G|$. This description also shows that the characters separate points: if $x\ne1$, a nonzero coordinate of $x$ is detected by a character $\psi$ with $\psi(x)\ne1$.

Multiplication by $\psi$ permutes $\widehat G$, so

$$
S(x)=\sum_\chi(\chi\psi)(x)=\psi(x)S(x).
$$

For $x\ne1$ this forces $S(x)=0$. For $x=1$ every summand is one. Since $\chi(g)^{-1}\chi(h)=\chi(g^{-1}h)$, the [character-sum cancellation lemma](../../../../../../character-sum-cancellation-lemma.md) gives

$$
\boxed{\sum_{\chi\in\widehat G}\chi(g)^{-1}\chi(h)
=|G|\,\mathbf1_{g=h}.}
$$

All character values are [roots of unity](../../../../../../root-of-unity.md), so inversion here is also complex conjugation. This is the finite-abelian version of [character orthogonality](../../../../../../character-orthogonality.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 137](../../../paper-137-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
