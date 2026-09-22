<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [covariant Yoneda embedding](../../../../../../covariant-yoneda-embedding.md) $Y(A)=\mathcal C(A,-)$. An arrow $f:B\to A$, viewed as an arrow $A\to B$ in the [opposite category](../../../../../../opposite-category.md), induces precomposition $h\mapsto hf$. Identities and composition are preserved because composition in $\mathcal C$ is associative.

The covariant [Yoneda lemma](../../../../../../yoneda-lemma.md) is the [bijection](../../../../../../bijection.md)

$$
\operatorname{Nat}(\mathcal C(A,-),F)\longrightarrow F(A),\qquad \alpha\longmapsto\alpha_A(1_A).
$$

Its inverse sends $x\in F(A)$ to $\alpha_B(h)=F(h)(x)$. This is a [natural transformation](../../../../../../natural-transformation.md): for $k:B\to C$, functoriality gives $F(k)\alpha_B(h)=F(kh)(x)=\alpha_C(kh)$. Conversely, naturality of an arbitrary $\alpha$ at $h:A\to B$ gives $\alpha_B(h)=F(h)\alpha_A(1_A)$. Evaluation at the [identity morphism](../../../../../../identity-morphism.md) therefore makes the two constructions inverse. Their formulas also prove naturality in $F$ and, contravariantly, in $A$.

Taking $F=Y(B)$ identifies [natural transformations](../../../../../../natural-transformation.md) $Y(A)\to Y(B)$ with $\mathcal C(B,A)$. Thus $Y$ is [full and faithful](../../../../../../full-and-faithful-functor.md), and reflects [isomorphisms](../../../../../../isomorphism.md); two image objects are isomorphic exactly when the original objects are isomorphic. It also carries existing [colimits](../../../../../../colimit.md) in $\mathcal C$ to [categorical limits](../../../../../../categorical-limit.md) of covariant [representable functors](../../../../../../representable-functor.md): maps out of a colimit are exactly compatible families of maps out of its diagram. Equivalently, this embedding preserves existing [categorical limits](../../../../../../categorical-limit.md) in $\mathcal C^{\mathrm{op}}$. The direction matters: the paper uses covariant representables, rather than the more usual contravariant [Yoneda embedding](../../../../../../yoneda-embedding.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
