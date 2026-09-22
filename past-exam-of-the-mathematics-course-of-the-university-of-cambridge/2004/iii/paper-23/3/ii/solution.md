<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [connected-component presheaf of a functor](../../../../../../connected-component-presheaf-of-a-functor.md). For $F:\mathcal C\to\mathcal D$, define $\mathcal E$ to have objects $(b,z)$, where $z$ is a [categorical connected component](../../../../../../connected-component-of-a-category.md) of $(b\downarrow F)$. An arrow $(b,z)\to(b',z')$ is an arrow $u:b\to b'$ such that $u^*z'=z$, where precomposition induces $u^*:\pi_0(b'\downarrow F)\to\pi_0(b\downarrow F)$. Identity and composition follow from precomposition, so this is a [category](../../../../../../category-split.md).

The projection $G:\mathcal E\to\mathcal D$ is a [discrete fibration](../../../../../../discrete-fibration.md): the unique lift of $u:b\to b'$ with codomain $(b',z')$ has domain $(b,u^*z')$.

Define $J:\mathcal C\to\mathcal E$ by

$$
Ja=(Fa,[(a,1_{Fa})]),\qquad Jv=Fv.
$$

For $v:a\to a'$, the objects $(a,1_{Fa})$ and $(a',Fv)$ lie in the same component of $(Fa\downarrow F)$, proving this is well-defined. Clearly $GJ=F$.

For $(b,z)\in\mathcal E$, the objects and arrows of $((b,z)\downarrow J)$ are exactly the objects and arrows of the component $z$ of $(b\downarrow F)$. Indeed, an arrow $(b,z)\to Ja$ is $u:b\to Fa$ with $[(a,u)]=z$, and its commuting triangles are precisely those in the original comma category. This category is nonempty and connected. Hence $J$ is a [final functor](../../../../../../final-functor.md), proving the [final-discrete-fibration factorization](../../../../../../final-discrete-fibration-factorization.md)

$$
\boxed{\mathcal C\xrightarrow{J}\mathcal E\xrightarrow{G}\mathcal D.}
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Section B](../../section-b.md)
4. [Paper 23](../../../paper-23-split.md)
5. [Iii](../../../split.md)
6. [2004](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
