<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [categorical presheaf](../../../../../../presheaf-category-theory.md) $P$ on the open subsets, define the [functors](../../../../../../functor.md) on objects by

$$
L(P)=P(\varnothing),\qquad R(P)=P(S).
$$

To prove $L\dashv\Delta$, a [natural transformation](../../../../../../natural-transformation.md) $t:P\to\Delta A$ must satisfy

$$
t_U=t_{\varnothing}\circ\operatorname{res}^{U}_{\varnothing}
$$

for every open $U$, since the restrictions of $\Delta A$ are identities. Thus it is determined by the [function](../../../../../../function-split.md) $P(\varnothing)\to A$. Conversely such a [function](../../../../../../function-split.md) defines all $t_U$ by that equation, and the [categorical presheaf](../../../../../../presheaf-category-theory.md) restriction laws make the components compatible. Hence

$$
\operatorname{Nat}(P,\Delta A)\cong\operatorname{Set}(P(\varnothing),A).
$$

For the other [adjunction](../../../../../../adjoint-functors.md), a transformation $s:\Delta A\to P$ is determined by its component $s_S:A\to P(S)$, since

$$
s_U=\operatorname{res}^{S}_U\circ s_S.
$$

Every [function](../../../../../../function-split.md) $A\to P(S)$ supplies compatible components by this formula. Therefore $\operatorname{Nat}(\Delta A,P)\cong\operatorname{Set}(A,P(S))$, giving the [adjoints to constant presheaves on open sets](../../../../../../adjoints-to-constant-presheaves-on-open-sets.md):

$$
\boxed{\operatorname{ev}_{\varnothing}\dashv\Delta\dashv\operatorname{ev}_S.}
$$

These are adjoints of the stated constant-presheaf [functor](../../../../../../functor.md), with its value at every [open set](../../../../../../open-set.md) including the empty one; no sheafification is involved.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
