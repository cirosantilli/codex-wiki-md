<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here is a precise [base change of a pullback square](../../../../../../base-change-of-a-pullback-square.md) statement. Suppose $A=B\times_D C$ is a [pullback in a category](../../../../../../pullback-category-theory.md) and $t:D'\to D$ is a [morphism](../../../../../../morphism.md). Assume the [pullbacks in a category](../../../../../../pullback-category-theory.md)

$$
A'=A\times_D D',\quad B'=B\times_D D',\quad C'=C\times_D D'
$$

exist, where $A\to D$ is the common composite. The induced square with vertices $A',B',C',D'$ is a [pullback in a category](../../../../../../pullback-category-theory.md); equivalently,

$$
\boxed{(B\times_D C)\times_D D'\cong(B\times_D D')\times_{D'}(C\times_D D').}
$$

Indeed, compatible [morphisms](../../../../../../morphism.md) $T\to B'$ and $T\to C'$ give [morphisms](../../../../../../morphism.md) $b:T\to B$, $c:T\to C$, and a common $v:T\to D'$, with the composites of $b,c$ to $D$ both equal to $tv$. The original [pullback in a category](../../../../../../pullback-category-theory.md) gives a unique [morphism](../../../../../../morphism.md) $h:T\to A$ with projections $b,c$. Its composite to $D$ is $tv$, so the defining [pullback in a category](../../../../../../pullback-category-theory.md) for $A'$ gives a unique [morphism](../../../../../../morphism.md) $T\to A'$ above $h,v$. Its maps to $B'$ and $C'$ are the prescribed ones by uniqueness in those [pullbacks in a category](../../../../../../pullback-category-theory.md). Conversely, these projections recover $b,c,v$, so every possible factorization is the same. This proves the [universal property](../../../../../../universal-property.md) without requiring arbitrary [categorical limits](../../../../../../categorical-limit.md) in the ambient [category](../../../../../../category-split.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
