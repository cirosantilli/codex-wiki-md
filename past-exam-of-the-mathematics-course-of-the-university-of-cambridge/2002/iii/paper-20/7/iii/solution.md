<h1 id="7/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For a [presheaf of sets on a topological space](../../../../../../presheaf-of-sets-on-a-topological-space.md) $P$, define $LP=P(\varnothing)$ and $RP=P(S)$. Then the [adjoints to constant presheaves on open sets](../../../../../../adjoints-to-constant-presheaves-on-open-sets.md) are

$$
\boxed{\operatorname{ev}_{\varnothing}\dashv\Delta\dashv\operatorname{ev}_S.}
$$

To prove the first [adjunction](../../../../../../adjoint-functors.md), a [natural transformation](../../../../../../natural-transformation.md) $a:P\to\Delta A$ must satisfy $a_U=a_{\varnothing}\circ\operatorname{res}_{U,\varnothing}$ by [naturality](../../../../../../naturality.md) at the inclusion $\varnothing\subseteq U$. Hence it is uniquely determined by a [function](../../../../../../function-split.md) $P(\varnothing)\to A$. Every such [function](../../../../../../function-split.md) defines a [natural transformation](../../../../../../natural-transformation.md) by this formula, because restriction maps compose. This gives $\operatorname{Nat}(P,\Delta A)\cong\mathbf{Set}(P(\varnothing),A)$.

For the second [adjunction](../../../../../../adjoint-functors.md), a [natural transformation](../../../../../../natural-transformation.md) $b:\Delta A\to P$ satisfies $b_U=\operatorname{res}_{S,U}\circ b_S$, so it is uniquely determined by a [function](../../../../../../function-split.md) $A\to P(S)$. Every such [function](../../../../../../function-split.md) defines the remaining components by restriction, giving $\operatorname{Nat}(\Delta A,P)\cong\mathbf{Set}(A,P(S))$. Evaluation acts on [presheaf morphisms](../../../../../../morphism-of-presheaves.md) componentwise, so these object assignments are indeed [functors](../../../../../../functor.md). The use of $P(\varnothing)$ is essential: a [constant presheaf of sets](../../../../../../constant-presheaf-of-sets.md) has value $A$ there, whereas a [sheaf](../../../../../../sheaf-mathematics.md) has a singleton value there. No sheaf condition is imposed in this question.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [7](../../7.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
