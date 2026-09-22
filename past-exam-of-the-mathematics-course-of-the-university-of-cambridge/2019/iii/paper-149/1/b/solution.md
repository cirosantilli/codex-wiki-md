<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Noncommutative Ruzsa triangle inequality](../../../../../../noncommutative-ruzsa-triangle-inequality.md) says that nonempty finite subsets $B,C,D$ of a [group](../../../../../../group-split.md) satisfy

$$
|B|\,|CD^{-1}|\leq |CB^{-1}|\,|BD^{-1}|.
$$

The [Ruzsa covering lemma](../../../../../../ruzsa-covering-lemma.md) says that if $|CD|\leq K|D|$, then some $X\subseteq C$ with $|X|\leq K$ satisfies

$$
C\subseteq XDD^{-1}.
$$

Now let $A$ be a [symmetric subset of a group](../../../../../../symmetric-subset-of-a-group.md), so $A^{-1}=A$ and $1\in A$. Apply the triangle inequality with the middle set $A$ to obtain, for $m\geq4$,

$$
|A|\,|A^m|\leq |A^{m-1}|\,|A^3|.
$$

The hypothesis therefore gives $|A^m|\leq K|A^{m-1}|$. Starting from $|A^3|\leq K|A|$ proves

$$
\boxed{|A^m|\leq K^{m-2}|A|\qquad(m\geq3).}
$$

In particular $|A^5|\leq K^3|A|$. Apply the covering lemma to $C=A^4$ and $D=A$. There is $X\subseteq A^4$ with $|X|\leq K^3$ such that

$$
A^4\subseteq XAA^{-1}=XA^2.
$$

The set $A^2$ is symmetric and contains the [identity element](../../../../../../identity-element.md), so this inclusion is exactly the covering condition showing that

$$
\boxed{A^2\text{ is a }K^3\text{-approximate group}.}
$$

Small doubling alone is insufficient in a [noncommutative group](../../../../../../non-abelian-group.md). Let $H$ be a finite group, let $G=H*\langle x\rangle$ be its [free product](../../../../../../free-product.md) with an [infinite cyclic group](../../../../../../infinite-cyclic-group.md), and put

$$
A=H\cup\{x,x^{-1}\}.
$$

Then $A$ is symmetric and $|A^2|\leq5|H|+4=O(|A|)$, while $A^3$ contains the [double coset](../../../../../../double-coset.md) $HxH$. Distinct pairs $(h_1,h_2)\in H^2$ give distinct reduced words $h_1xh_2$, so $|HxH|=|H|^2$. Letting $|H|\to\infty$ proves the [small doubling does not control tripling in a noncommutative group](../../../../../../small-doubling-does-not-control-tripling-in-a-noncommutative-group.md) phenomenon.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 149](../../../paper-149-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
