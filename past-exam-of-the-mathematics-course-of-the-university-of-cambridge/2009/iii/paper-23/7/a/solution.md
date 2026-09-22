<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [monad](../../../../../../monad.md) on $\mathcal C$ consists of an [endofunctor](../../../../../../endofunctor.md) $T:\mathcal C\to\mathcal C$ and [natural transformations](../../../../../../natural-transformation.md) $\eta:1_{\mathcal C}\Rightarrow T$ and $\mu:T^2\Rightarrow T$ satisfying, at every object $A$,

$$
\boxed{\mu_A T\eta_A=1_{TA}=\mu_A\eta_{TA},\qquad
\mu_A T\mu_A=\mu_A\mu_{TA}.}
$$

These are the unit and associativity laws for the [unit and multiplication of a monad](../../../../../../unit-and-multiplication-of-a-monad.md).

An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is a pair $(A,a)$ with $a:TA\to A$ satisfying

$$
\boxed{a\eta_A=1_A,\qquad a\mu_A=aT a.}
$$

A [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) $f:(A,a)\to(B,b)$ is a [morphism](../../../../../../morphism.md) $f:A\to B$ with $fa=bT f$. Identities satisfy this condition, and composing two such maps preserves it by functoriality of $T$. The resulting [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) is denoted $\mathcal C^T$. Its [forgetful functor](../../../../../../forgetful-functor.md) $U:\mathcal C^T\to\mathcal C$ sends $(A,a)$ to $A$ and leaves the underlying arrows unchanged.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [7](../../7.md)
3. [Paper 23](../../../paper-23-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
