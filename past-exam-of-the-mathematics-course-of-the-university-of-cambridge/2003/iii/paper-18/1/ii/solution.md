<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [Yoneda embedding](../../../../../../yoneda-embedding.md) is the [functor](../../../../../../functor.md) $H_\bullet:\mathcal C\to[\mathcal C^{\mathrm{op}},\mathbf{Set}]$ sending $A$ to $H_A=\mathcal C(-,A)$ and $f:A\to B$ to postcomposition, $(H_f)_U(h)=fh$. Composition and identities are preserved by associativity and the identity laws in $\mathcal C$.

Apply the [Yoneda lemma](../../../../../../yoneda-lemma.md) with $X=H_B$. It gives a bijection $\operatorname{Nat}(H_A,H_B)\cong\mathcal C(A,B)$. The inverse sends $f$ precisely to $H_f$, since $H_B(h)(f)=fh$. Hence every transformation between the representables comes from exactly one morphism of $\mathcal C$. This proves that **$H_\bullet$ is a full and faithful [functor](../../../../../../functor.md)**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
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
