<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [monad](../../../../../../monad.md) $\mathbb T=(T,\eta,\mu)$ define the [free algebra functor](../../../../../../free-algebra-functor.md) by

$$
F^{\mathbb T}X=(TX,\mu_X),\qquad F^{\mathbb T}f=Tf.
$$

The unit and associativity identities of the [monad](../../../../../../monad.md) make $(TX,\mu_X)$ an [algebra for a monad](../../../../../../algebra-for-a-monad.md), and [naturality](../../../../../../naturality.md) of $\mu$ makes $Tf$ a [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md). Let $G^{\mathbb T}$ be the [forgetful functor](../../../../../../forgetful-functor.md). For $(A,a)$ in the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md), set

$$
\Phi(h)=h\eta_X,\qquad \Psi(f)=a\,Tf.
$$

The inverse candidate is a [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md), since

$$
a\,Tf\,\mu_X=a\mu_A\,T^2f=a\,Ta\,T^2f
=a\,T(a\,Tf).
$$

The two composites are identities:

$$
\Phi\Psi(f)=a\eta_Af=f,\qquad
\Psi\Phi(h)=a\,Th\,T\eta_X=h\mu_X\,T\eta_X=h.
$$

These use respectively the [unit law for a monad algebra](../../../../../../unit-law-for-a-monad-algebra.md), the algebra-morphism equation, and a unit identity of the [monad](../../../../../../monad.md). The formulas commute with precomposition in $X$ and postcomposition by [monad algebra morphisms](../../../../../../morphism-of-algebras-for-a-monad.md), so they form a [natural bijection](../../../../../../natural-bijection.md). Therefore **the free-algebra functor is left adjoint to forgetting**:

$$
\boxed{\mathcal X^{\mathbb T}(F^{\mathbb T}X,(A,a))\cong\mathcal X(X,A),
\qquad F^{\mathbb T}\dashv G^{\mathbb T}.}
$$

Its [adjunction unit](../../../../../../unit-of-an-adjunction.md) is $\eta_X$, and its [adjunction counit](../../../../../../counit-of-an-adjunction.md) at $(A,a)$ is $a:(TA,\mu_A)\to(A,a)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 22](../../../paper-22-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
