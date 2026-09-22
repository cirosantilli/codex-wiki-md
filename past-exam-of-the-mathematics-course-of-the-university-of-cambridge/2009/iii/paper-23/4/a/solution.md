<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Yoneda embedding](../../../../../../yoneda-embedding.md) sends $c$ to the [representable presheaf](../../../../../../representable-functor.md) $H_c=\mathcal C(-,c)$. On a [morphism](../../../../../../morphism.md) $f:c\to d$, it sends a map $u:a\to c$ to $fu:a\to d$, giving $H_f:H_c\to H_d$.

The [Yoneda lemma](../../../../../../yoneda-lemma.md) states that for every [categorical presheaf](../../../../../../presheaf-category-theory.md) $P$ there is a [bijection](../../../../../../bijection.md), natural in both variables,

$$
\operatorname{Nat}(H_c,P)\cong P(c),\qquad \alpha\longmapsto\alpha_c(1_c).
$$

Its inverse sends $x\in P(c)$ to the transformation $u:a\to c\mapsto P(u)x$. Apply it to $P=H_d$ to obtain

$$
\operatorname{Nat}(H_c,H_d)\cong H_d(c)=\mathcal C(c,d).
$$

Under this [bijection](../../../../../../bijection.md) $H_f$ corresponds exactly to $f$, so the map induced by the embedding on each [hom-set](../../../../../../hom-set.md) is bijective. Therefore **the [Yoneda embedding](../../../../../../yoneda-embedding.md) is [full and faithful](../../../../../../full-and-faithful-functor.md)**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
