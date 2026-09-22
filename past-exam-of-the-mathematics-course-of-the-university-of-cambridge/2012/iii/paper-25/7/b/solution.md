<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix an object $C$. For $x:C\to B$, use $rx:C\to A$ as its identity arrow. For $a:C\to A$, its source is $fa$ and target is $ga$. If $ga=fb$, define the composite of $a$ followed by $b$ by

$$
\boxed{b\circ a=a+b-rga,\qquad a^{-1}=rfa+rga-a.}
$$

These expressions use addition and subtraction in the [hom-set](../../../../../../hom-set.md) of the [preadditive category](../../../../../../preadditive-category.md). The [reflexive pair](../../../../../../reflexive-pair.md) identities $fr=gr=1_B$ give

$$
f(b\circ a)=fa+fb-ga=fa,\qquad g(b\circ a)=ga+gb-ga=gb,
$$

so the composite has the required endpoints. Also $f(a^{-1})=ga$ and $g(a^{-1})=fa$.

The unit identities follow directly: $a\circ rfa=rfa+a-rfa=a$ and $rga\circ a=a+rga-rga=a$. If $ga=fb$ and $gb=fc$, either parenthesization of three arrows equals $a+b+c-rga-rgb$, so composition is associative. The inverse identities are

$$
a^{-1}\circ a=a+a^{-1}-rga=rfa,\qquad a\circ a^{-1}=a^{-1}+a-rfa=rga.
$$

Therefore these operations define a [groupoid](../../../../../../groupoid.md) on the specified object and arrow [sets](../../../../../../set-split.md). Precomposing by $k:C'\to C$ respects each expression, by additivity of composition, so the [groupoids](../../../../../../groupoid.md) are natural in $C$.

**Every [reflexive pair](../../../../../../reflexive-pair.md) therefore has the required [groupoid](../../../../../../groupoid.md) structure on generalized points.** This is the [reflexive-pair groupoid formula in a preadditive category](../../../../../../reflexive-pair-groupoid-formula-in-a-preadditive-category.md). If the composable-arrow [pullback in a category](../../../../../../pullback-category-theory.md) $A\times_{g,B,f}A$ exists, its projections $p,q$ give the actual internal composition map $p+q-rgp$. The printed generalized-point definition does not assume that this pullback exists, and preadditivity alone would not ensure it.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
