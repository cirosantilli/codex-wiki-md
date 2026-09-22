<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Take an [epimorphism](../../../../../../epimorphism.md) $\alpha:F\Rightarrow G$ in $[\mathcal C,\mathbf{Set}]$ and a [natural transformation](../../../../../../natural-transformation.md) $\beta:\mathcal C(A,-)\Rightarrow G$. By the [Yoneda lemma](../../../../../../yoneda-lemma.md), $\beta$ corresponds to $x=\beta_A(1_A)\in G(A)$. By the [pointwise epimorphism in a functor category](../../../../../../pointwise-epimorphism-in-a-functor-category.md) criterion, choose $y\in F(A)$ with $\alpha_A(y)=x$.

The [Yoneda lemma](../../../../../../yoneda-lemma.md) gives $\gamma_B(f)=F(f)(y)$, a [natural transformation](../../../../../../natural-transformation.md) $\mathcal C(A,-)\Rightarrow F$. Naturality of $\alpha$ yields

$$
\alpha_B\gamma_B(f)=\alpha_BF(f)(y)=G(f)(\alpha_Ay)=G(f)(x)=\beta_B(f).
$$

Therefore **[covariant representables are projective](../../../../../../covariant-representables-are-projective.md)** in the set-valued [functor category](../../../../../../functor-category.md). Local smallness ensures that $\mathcal C(A,-)$ is set-valued.

## ↑ Ancestors (11)

1. [D](../d.md)
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
