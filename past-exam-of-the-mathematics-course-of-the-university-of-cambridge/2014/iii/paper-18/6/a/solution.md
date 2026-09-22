<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [monad](../../../../../../monad.md) consists of an endofunctor $T:\mathcal C\to\mathcal C$ and [natural transformations](../../../../../../natural-transformation.md) $\eta:1\Rightarrow T$ and $\mu:T^2\Rightarrow T$, the [unit and multiplication of a monad](../../../../../../unit-and-multiplication-of-a-monad.md), satisfying

$$
\mu_A T\eta_A=\mu_A\eta_{TA}=1_{TA},\qquad
\mu_A T\mu_A=\mu_A\mu_{TA}.
$$

An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is $(A,a)$ with $a:TA\to A$ satisfying $a\eta_A=1_A$ and $a\mu_A=aTa$. A [morphism of algebras for a monad](../../../../../../morphism-of-algebras-for-a-monad.md) $h:(A,a)\to(B,b)$ satisfies $ha=bTh$. These objects and morphisms form the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) $\mathcal C^T$; its composition works because $T$ is a [functor](../../../../../../functor.md).

For the [list monad](../../../../../../list-monad.md), $TX=\coprod_{n\geq0}X^n$ is the set of finite ordered lists, including the empty list. The map $Tf$ applies $f$ to each entry; $\eta_X(x)=[x]$ and $\mu_X$ concatenates a list of lists. The unit laws say that adding singleton brackets and then flattening changes nothing. Associativity says that flattening a list of lists of lists in either order produces the same ordered sequence. These descriptions also prove naturality.

If $a:TX\to X$ is an [algebra for a monad](../../../../../../algebra-for-a-monad.md), define

$$
e=a([]),\qquad x*y=a([x,y]).
$$

The singleton law gives $a([x])=x$. Apply the algebra associativity law to $[[],[x]]$ and $[[x],[]]$ to obtain $e*x=x=x*e$. Applying it to $[[x,y],[z]]$ and $[[x],[y,z]]$ shows

$$
(x*y)*z=a([x,y,z])=x*(y*z).
$$

Thus $(X,*,e)$ is a [monoid](../../../../../../monoid.md). Applying the same law to $[[x_1,\ldots,x_{n-1}],[x_n]]$ shows inductively that $a$ is necessarily ordered multiplication of its entries, with the empty product $e$.

Conversely, any [monoid](../../../../../../monoid.md) defines such a list-fold map $a$. The monoid unit proves $a\eta=1$, and associativity and the unit prove that multiplying flattened lists equals multiplying their individual products, including empty sublists. Hence $a\mu=aTa$. An algebra morphism preserves the empty-list value and two-entry-list values, so it is a [monoid homomorphism](../../../../../../monoid-homomorphism.md); conversely a [monoid homomorphism](../../../../../../monoid-homomorphism.md) preserves every ordered product and is an algebra morphism. Therefore

$$
\boxed{\mathbf{Set}^{\mathrm{List}}\cong\mathbf{Mon}.}
$$

Thus [list-monad algebras are monoids](../../../../../../list-monad-algebras-are-monoids.md), with the identification also matching every morphism.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
