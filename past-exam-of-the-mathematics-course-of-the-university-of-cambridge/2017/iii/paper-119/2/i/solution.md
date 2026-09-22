<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [balanced category](../../../../../../balanced-category.md) is one in which every [morphism](../../../../../../morphism.md) that is both a [monomorphism](../../../../../../monomorphism.md) and an [epimorphism](../../../../../../epimorphism.md) is an [isomorphism](../../../../../../isomorphism.md). A [faithful functor](../../../../../../faithful-functor.md) reflects both of these cancellation properties: for instance, $fu=fv$ implies $Ff\,Fu=Ff\,Fv$, so monicity of $Ff$ and faithfulness imply $u=v$; the dual argument applies to [epimorphisms](../../../../../../epimorphism.md). If $Ff$ is invertible, it is both monic and epic. Thus a [faithful functor](../../../../../../faithful-functor.md) from a [balanced category](../../../../../../balanced-category.md) reflects [isomorphisms](../../../../../../isomorphism.md).

For the [adjunction](../../../../../../adjoint-functors.md) $F\dashv G$, the [unit and counit of an adjunction](../../../../../../unit-and-counit-of-an-adjunction.md) satisfy

$$
\varepsilon_{FA}F\eta_A=1_{FA},\qquad G\varepsilon_B\eta_{GB}=1_{GB}.
$$

If $F$ is a [faithful functor](../../../../../../faithful-functor.md) and $\eta_Au=\eta_Av$, applying $F$ and composing with $\varepsilon_{FA}$ gives $Fu=Fv$, hence $u=v$. Thus each $\eta_A$ is a [monomorphism](../../../../../../monomorphism.md). Conversely, if every $\eta_A$ is monic and $Fu=Fv$ for $u,v:X\to A$, [naturality](../../../../../../naturality.md) gives

$$
\eta_Au=GFu\,\eta_X=GFv\,\eta_X=\eta_Av,
$$

so $u=v$. This proves the [faithful left adjoint criterion](../../../../../../faithful-left-adjoint-criterion.md).

Now assume both $\eta$ and $\varepsilon$ are pointwise monic. The first triangle identity makes $\varepsilon_{FA}$ a [split epimorphism](../../../../../../split-epimorphism.md); since it is also a [monomorphism](../../../../../../monomorphism.md), it is invertible and $F\eta_A$ is its inverse. The [faithful left adjoint criterion](../../../../../../faithful-left-adjoint-criterion.md) says that $F$ is faithful, and the [balanced category](../../../../../../balanced-category.md) argument above then reflects the invertibility of $F\eta_A$ to that of $\eta_A$.

For completeness, an invertible unit makes $F$ a [full and faithful functor](../../../../../../full-and-faithful-functor.md). For $h:FA\to FA'$, set $k=\eta_{A'}^{-1}G(h)\eta_A$. The triangle identity gives $F\eta_A=\varepsilon_{FA}^{-1}$, so [naturality](../../../../../../naturality.md) of $\varepsilon$ yields

$$
F(k)=\varepsilon_{FA'}FG(h)\varepsilon_{FA}^{-1}=h.
$$

Faithfulness was already proved.

Let $q:FA\to B$ be a [strong epimorphism](../../../../../../strong-epimorphism.md), and put

$$
t=FG(q)\varepsilon_{FA}^{-1}:FA\to FGB.
$$

Then [naturality](../../../../../../naturality.md) gives $\varepsilon_Bt=q$. The square with left edge $q$, right edge the [monomorphism](../../../../../../monomorphism.md) $\varepsilon_B$, top edge $t$, and bottom edge $1_B$ has a diagonal $s:B\to FGB$ by the defining lifting property of a [strong epimorphism](../../../../../../strong-epimorphism.md). Thus $\varepsilon_Bs=1_B$. A monic [split epimorphism](../../../../../../split-epimorphism.md) is invertible, so $B\cong FGB$. The essential image of $F$ is therefore closed under [strong quotients](../../../../../../strong-quotient.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
