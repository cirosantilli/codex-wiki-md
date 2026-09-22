<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $H_A=\mathcal C(-,A)$ for a [representable presheaf](../../../../../../representable-functor.md). The contravariant [Yoneda lemma](../../../../../../yoneda-lemma.md) states that, for every [presheaf on a category](../../../../../../presheaf-category-theory.md) $X$, evaluation at the identity is a bijection

$$
\boxed{\operatorname{Nat}(H_A,X)\longrightarrow X(A),\qquad\alpha\longmapsto\alpha_A(1_A),}
$$

natural in both $A$ and $X$. Smallness of $\mathcal C$ ensures the relevant families and natural-transformation collections are sets.

For $x\in X(A)$ define $\alpha^x_B(h)=X(h)(x)$ for each $h:B\to A$. This family is a [natural transformation](../../../../../../natural-transformation.md): for $u:B'\to B$, $X(u)\alpha^x_B(h)=X(u)X(h)x=X(hu)x=\alpha^x_{B'}(hu)$. Its identity value is $x$. Conversely, naturality of any $\alpha$ at $h:B\to A$ gives $\alpha_B(h)=X(h)\alpha_A(1_A)$. Thus evaluation and the displayed construction are inverse.

For a map $v:A\to A'$, precomposing a transformation $H_{A'}\to X$ with postcomposition $H_A\to H_{A'}$ corresponds to applying $X(v):X(A')\to X(A)$. For a transformation $\tau:X\to Y$, postcomposition corresponds to $x\mapsto\tau_A(x)$. These identities prove the stated [naturality](../../../../../../naturality.md) in both variables.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
