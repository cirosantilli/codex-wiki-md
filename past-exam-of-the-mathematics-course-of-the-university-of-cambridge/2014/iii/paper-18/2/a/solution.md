<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The covariant form of the [Yoneda lemma](../../../../../../yoneda-lemma.md) says that for a [locally small category](../../../../../../locally-small-category.md) $\mathcal C$, a [functor](../../../../../../functor.md) $F:\mathcal C\to\mathbf{Set}$ and an object $A$, there is a [bijection](../../../../../../bijection.md), natural in $A$ and $F$,

$$
\operatorname{Nat}(\mathcal C(A,-),F)\cong F(A).
$$

Explicitly its two directions are

$$
\boxed{\alpha\longmapsto\alpha_A(1_A),\qquad x\longmapsto\alpha^x,
\quad\alpha^x_B(f)=F(f)(x).}
$$

For $u:B\to B'$, functoriality gives $F(u)\alpha^x_B(f)=F(uf)(x)=\alpha^x_{B'}(uf)$, so $\alpha^x$ is a [natural transformation](../../../../../../natural-transformation.md). Conversely, naturality of $\alpha$ at $f:A\to B$ gives $\alpha_B(f)=F(f)(\alpha_A(1_A))$. This proves that the displayed maps are inverses.

Naturality in $F$ follows because postcomposition by $\theta:F\Rightarrow F'$ sends $x$ to $\theta_A(x)$. For $u:A'\to A$, precomposition of transformations by $\mathcal C(u,-)$ sends $\alpha^x$ to $\alpha^{F(u)(x)}$. This also verifies naturality in the representing object.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
