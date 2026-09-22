<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [monad](../../../../../../monad.md) $\mathbb T=(T,\eta,\mu)$ consists of an [endofunctor](../../../../../../endofunctor.md) $T:\mathcal C\to\mathcal C$ and [natural transformations](../../../../../../natural-transformation.md) $\eta:1_{\mathcal C}\Rightarrow T$ and $\mu:T^2\Rightarrow T$ satisfying

$$
\mu_A\eta_{TA}=1_{TA}=\mu_A T\eta_A,\qquad \mu_A\mu_{TA}=\mu_A T\mu_A.
$$

An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is $(A,a)$ with $a:TA\to A$ satisfying $a\eta_A=1_A$ and $a\mu_A=aT(a)$. A [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md) $h:(A,a)\to(B,b)$ obeys $ha=bT(h)$. The [functor](../../../../../../functor.md) laws show that identities and composites obey this equation, giving the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) $\mathcal C^{\mathbb T}$.

For an [adjunction](../../../../../../adjoint-functors.md) $F\dashv G$, let $\eta$ be its [adjunction unit](../../../../../../unit-of-an-adjunction.md) and $\varepsilon$ its [adjunction counit](../../../../../../counit-of-an-adjunction.md). The [monad induced by an adjunction](../../../../../../monad-induced-by-an-adjunction.md) is

$$
\boxed{T=GF,\qquad \eta:1\Rightarrow GF,\qquad \mu_A=G(\varepsilon_{FA}).}
$$

The two unit laws are $G\varepsilon_{FA}\eta_{GFA}=1_{GFA}$ and $G(\varepsilon_{FA}F\eta_A)=1_{GFA}$, respectively the two [triangle identities for an adjunction](../../../../../../triangle-identities-for-an-adjunction.md).

For associativity, [naturality](../../../../../../naturality.md) of the [adjunction counit](../../../../../../counit-of-an-adjunction.md) at $\varepsilon_{FA}:FGFA\to FA$ says

$$
\varepsilon_{FA}\,\varepsilon_{FGFA}=\varepsilon_{FA}\,FG(\varepsilon_{FA}).
$$

Apply $G$ to obtain $\mu_A\mu_{TA}=\mu_AT\mu_A$. The composites defining $\eta$ and $\mu$ are [natural transformations](../../../../../../natural-transformation.md), so all [monad](../../../../../../monad.md) axioms have been checked, not only their underlying objectwise types.

## ↑ Ancestors (11)

1. [A](../a.md)
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
