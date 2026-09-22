<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We prove the vanishing by an [injective resolution of sheaves](../../../../../../injective-resolution-of-sheaves.md) and the [flasque-kernel section-lifting lemma](../../../../../../flasque-kernel-section-lifting-lemma.md).

For a [short exact sequence of sheaves](../../../../../../short-exact-sequence-of-sheaves.md) $0\to\mathcal F\to\mathcal G\to\mathcal H\to0$ with flasque kernel, every section of $\mathcal H$ on an open set lifts to $\mathcal G$ there. Indeed choose a maximal partial lift by the [Zorn lemma](../../../../../../zorn-s-lemma.md), using the [sheaf gluing axiom](../../../../../../sheaf-gluing-axiom.md) on chains. At any point outside its domain choose a local lift. The difference on the overlap is a section of $\mathcal F$ and extends to the new open set by flasqueness; subtract that extension from the new lift and glue. Maximality forces the lift's domain to be the whole open set. Thus taking sections preserves this short exact sequence.

Every [injective sheaf](../../../../../../injective-sheaf.md) is flasque: for $U\subseteq V$, the monomorphism between the [extension by zero](../../../../../../extension-by-zero.md) sheaves $\mathbb Z_U\hookrightarrow\mathbb Z_V$ and the defining extension property of injectivity make the restriction $\mathcal J(V)\to\mathcal J(U)$ surjective. Embed $\mathcal F$ into an injective sheaf $\mathcal J$. The quotient $\mathcal Q$ is flasque as well: lift a section of $\mathcal Q$ on a smaller open to $\mathcal J$, extend it in $\mathcal J$, and project.

The [long exact sequence in sheaf cohomology](../../../../../../long-exact-sequence-in-sheaf-cohomology.md) now gives $H^1(X,\mathcal F)=0$, since $\Gamma(X,\mathcal J)\to\Gamma(X,\mathcal Q)$ is surjective, and for $i\ge2$ gives $H^i(X,\mathcal F)\cong H^{i-1}(X,\mathcal Q)$, since injectives have zero positive-degree derived functors. Repeat the construction for the flasque quotient. After finitely many such shifts any specified positive degree reduces to a vanishing first group. Hence

$$
\boxed{H^i(X,\mathcal F)=0\qquad(i>0).}
$$

No separation, compactness or scheme hypothesis is used.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 113](../../../paper-113-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
