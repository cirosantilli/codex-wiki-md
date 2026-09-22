<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [isomorphism](../../../../../../isomorphism.md) $f:A\to B$ gives a [natural isomorphism](../../../../../../natural-isomorphism.md) $h_f:h_A\to h_B$ by postcomposition, with inverse $h_{f^{-1}}$.

Conversely suppose $\alpha:h_A\to h_B$ is a [natural isomorphism](../../../../../../natural-isomorphism.md), with inverse $\beta$. Since the [Yoneda embedding](../../../../../../yoneda-embedding.md) is a [full and faithful functor](../../../../../../full-and-faithful-functor.md), there are unique $f:A\to B$ and $g:B\to A$ with $h_f=\alpha$ and $h_g=\beta$. Their composites satisfy

$$
h_{gf}=\beta\alpha=1_{h_A}=h_{1_A},\qquad
h_{fg}=\alpha\beta=1_{h_B}=h_{1_B}.
$$

Faithfulness gives $gf=1_A$ and $fg=1_B$. Thus

$$
\boxed{A\cong B\quad\Longleftrightarrow\quad
\mathcal C(-,A)\cong\mathcal C(-,B)\text{ naturally}.}
$$

The [naturality](../../../../../../naturality.md) requirement ensures that all incoming [morphisms](../../../../../../morphism.md) are respected; unrelated componentwise [bijections](../../../../../../bijection.md) alone would not justify the conclusion.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
