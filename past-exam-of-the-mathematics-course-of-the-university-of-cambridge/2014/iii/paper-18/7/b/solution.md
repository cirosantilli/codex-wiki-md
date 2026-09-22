<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [preadditive category](../../../../../../preadditive-category.md) has an [abelian group](../../../../../../abelian-group.md) structure on every hom-set, with composition additive in each variable. Neither a [zero object](../../../../../../zero-object.md) nor [biproducts](../../../../../../biproduct.md) are part of this definition.

Fix $C$ and use the [reflexive pair](../../../../../../reflexive-pair.md) $f,g:A\rightrightarrows B$, $r:B\to A$, with $fr=gr=1_B$. Take objects $x:C\to B$ and arrows $a:C\to A$, with source $fa$, target $ga$, and identity at $x$ equal to $rx$. For composable $a,b$, so $ga=fb$, define

$$
\boxed{b\circ a=a+b-rga.}
$$

The [preadditive category](../../../../../../preadditive-category.md) axioms give

$$
f(b\circ a)=fa+fb-ga=fa,\qquad
g(b\circ a)=ga+gb-ga=gb.
$$

Thus the formula has the required endpoints. The identities satisfy $(rga)\circ a=a$ and $a\circ(rfa)=a$, using $gr=fr=1_B$.

For $ga=fb$ and $gb=fc$, both ways of composing three arrows equal

$$
a+b+c-rga-rgb.
$$

Indeed $g(b\circ a)=gb$, while expanding $c\circ b$ and then composing with $a$ gives the same expression. Hence composition is associative.

Every arrow has inverse

$$
\boxed{a^{-1}=rfa+rga-a.}
$$

Its source is $ga$ and its target is $fa$. Substituting in the composition formula gives $a^{-1}\circ a=rfa$ and $a\circ a^{-1}=rga$. Therefore this is a [groupoid](../../../../../../groupoid.md).

For $u:C'\to C$, precomposition by $u$ preserves sources, targets, identities, composition and inverses by bilinearity. Thus the construction is natural in $C$, giving the requested [internal groupoid](../../../../../../internal-groupoid.md) structure in its hom-set formulation. If the composable-arrow [pullback in a category](../../../../../../pullback-category-theory.md) exists, the same formula defines its internal composition morphism. The [reflexive-pair groupoid formula in a preadditive category](../../../../../../reflexive-pair-groupoid-formula-in-a-preadditive-category.md) requires no extra additive-category hypotheses.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
