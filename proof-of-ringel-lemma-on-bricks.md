# Proof of Ringel lemma on bricks

↑ **Parent:** [Ringel lemma on bricks](ringel-lemma-on-bricks.md)

The [Fitting lemma](fitting-lemma.md) supplies a nonzero nilpotent endomorphism $f$ of a non-brick indecomposable $X$. Minimize its nonzero rank; nilpotence and minimality give $f^2=0$. Set $I=\operatorname{im}f\subset K=\ker f=\bigoplus_jK_j$. Choose a nonzero component $u:I\to K_j$. The square-zero endomorphism $X\xrightarrow fI\xrightarrow uK_j\hookrightarrow X$ has rank at least $\dim I$, so $u$ is injective.

If $\operatorname{Ext}^1(I,K_j)=0$, the projection $K\to K_j$ extends to $X\to K_j$ by the [long exact sequence of Ext groups](long-exact-sequence-of-ext-groups.md), giving a [module retraction](module-retraction.md) and contradicting indecomposability. Thus this extension group is nonzero. Since [path algebras are hereditary](path-algebras-are-hereditary.md), $u$ induces a surjection $\operatorname{Ext}^1(K_j,K_j)\twoheadrightarrow\operatorname{Ext}^1(I,K_j)$. Hence $K_j$ is a proper indecomposable submodule with self-extensions. Iterate until a [brick module](brick-module.md) is reached; dimensions strictly decrease.

This minimal-rank argument is given in section 2 of [William Crawley-Boevey's quiver lectures](https://www.math.uni-bielefeld.de/~wcrawley/quivlecs.pdf).

## ↑ Ancestors (11)

1. [Ringel lemma on bricks](ringel-lemma-on-bricks.md)
2. [Brick module](brick-module.md)
3. [Endomorphism ring](endomorphism-ring.md)
4. [Module homomorphism](module-homomorphism.md)
5. [Module (mathematics)](module-mathematics.md)
6. [Module theory](module-theory-split.md)
7. [Commutative algebra](commutative-algebra-split.md)
8. [Algebra](algebra-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-3/6/ii/solution.md)
