<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the [forgetful functor](../../../../../../forgetful-functor.md) $G^{\mathbb T}(A,a)=A$, acting as the identity on underlying [morphisms](../../../../../../morphism.md). Define the [free algebra functor](../../../../../../free-algebra-functor.md) by

$$
F^{\mathbb T}(X)=(TX,\mu_X),\qquad F^{\mathbb T}(h)=T(h).
$$

The [monad](../../../../../../monad.md) laws make $\mu_X$ an [algebra for a monad](../../../../../../algebra-for-a-monad.md) structure, and [naturality](../../../../../../naturality.md) of $\mu$ makes $T(h)$ an [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md).

For $(A,a)$, define the transpose maps

$$
\Phi(h)=h\eta_X,\qquad \Psi(k)=aT(k),\qquad
\Phi:\mathcal C^{\mathbb T}(F^{\mathbb T}X,(A,a))\longrightarrow\mathcal C(X,A).
$$

The map $\Psi(k)$ is an [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md), because [naturality](../../../../../../naturality.md) of $\mu$ and the algebra associativity law give

$$
aT(k)\mu_X=a\mu_A T^2(k)=aT(a)T^2(k)=aT(aT(k)).
$$

For $k:X\to A$, [naturality](../../../../../../naturality.md) of $\eta$ gives $\Phi\Psi(k)=aT(k)\eta_X=a\eta_A k=k$. Conversely, if $h$ is an [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md), then

$$
\Psi\Phi(h)=aT(h)T\eta_X=h\mu_X T\eta_X=h.
$$

Precomposing by a map into $X$ or postcomposing by an [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) respects both formulas. Thus the [bijection](../../../../../../bijection.md) is natural and **$F^{\mathbb T}\dashv G^{\mathbb T}$**. This is the [free-forgetful Eilenberg-Moore adjunction](../../../../../../free-forgetful-eilenberg-moore-adjunction.md).

Its [adjunction unit](../../../../../../unit-of-an-adjunction.md) is the given $\eta_X$; its [adjunction counit](../../../../../../counit-of-an-adjunction.md) at $(A,a)$ is the [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) $a:(TA,\mu_A)\to(A,a)$. Hence $G^{\mathbb T}F^{\mathbb T}=T$, and the induced multiplication is the underlying counit at $(TX,\mu_X)$, namely $\mu_X$. Therefore **this [adjunction](../../../../../../adjoint-functors.md) induces exactly the original [monad](../../../../../../monad.md), including its [unit and multiplication of a monad](../../../../../../unit-and-multiplication-of-a-monad.md)**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
