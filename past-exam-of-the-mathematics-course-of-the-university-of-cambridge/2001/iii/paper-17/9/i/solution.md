<h1 id="9/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [monad](../../../../../../monad.md) on $\mathcal C$ consists of an [endofunctor](../../../../../../endofunctor.md) $T$ and [natural transformations](../../../../../../natural-transformation.md) $\eta:1\to T$, $\mu:T^2\to T$ satisfying the [unit and multiplication of a monad](../../../../../../unit-and-multiplication-of-a-monad.md) laws

$$
\boxed{\mu\circ T\eta=1_T=\mu\circ\eta T,\qquad
\mu\circ T\mu=\mu\circ\mu T.}
$$

An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is an object $A$ equipped with $a:TA\to A$ such that

$$
a\eta_A=1_A,\qquad aT(a)=a\mu_A.
$$

A [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md) $f:(A,a)\to(B,b)$ is a [morphism](../../../../../../morphism.md) $f:A\to B$ satisfying $fa=bT(f)$. Identities and composition obey this equation, giving the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) $\mathcal C^T$ and its [forgetful functor](../../../../../../forgetful-functor.md) $U^T(A,a)=A$.

For an [adjunction](../../../../../../adjoint-functors.md) $F\dashv U:\mathcal D\to\mathcal C$ with induced [monad](../../../../../../monad.md) $T=UF$, the [Eilenberg-Moore comparison functor](../../../../../../eilenberg-moore-comparison-functor.md) is

$$
K:\mathcal D\to\mathcal C^T,\qquad
K(D)=(UD,U\varepsilon_D),\quad K(h)=Uh.
$$

The [functor](../../../../../../functor.md) $U$ is monadic when it has such a [left adjoint](../../../../../../adjoint-functors.md) and this comparison is an [equivalence of categories](../../../../../../equivalence-of-categories.md); a stricter convention requires an [isomorphism of categories](../../../../../../isomorphism-of-categories.md) over $\mathcal C$. We will identify which limit-lifting conclusion each convention supports in part (iii).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [9](../../9.md)
3. [Paper 17](../../../paper-17-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
