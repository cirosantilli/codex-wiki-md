<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use $\mathbb N=\{0,1,\ldots\}$, as required by the formula at zero, and composition of functions as multiplication in $M$. The displayed $T$ preserves identities, and for $n>0$,

$$
T(gf)(n)=g(f(n-1))+1=Tg(Tf(n));
$$

both sides send zero to zero. Thus $T$ is a [functor](../../../../../../functor.md) on the one-object [category](../../../../../../category-split.md).

For the [shift monad on order-preserving maps of natural numbers](../../../../../../shift-monad-on-order-preserving-maps-of-natural-numbers.md), set

$$
\eta(n)=n+1,\qquad\mu(n)=\max(n-1,0).
$$

These are [order-preserving functions](../../../../../../order-preserving-function.md). The equations $Tf\,\eta=\eta f$ and $\mu T^2f=Tf\,\mu$ hold pointwise, giving the required [natural transformations](../../../../../../natural-transformation.md). For the second equation, both sides are zero at $n=0,1$, and are $f(n-2)+1$ for $n\geq2$. The two unit laws are $\mu\eta=\mu T\eta=1$. Associativity is checked by

$$
(\mu T\mu)(n)=(\mu\mu)(n)=\max(n-2,0).
$$

Consequently these maps define a [monad](../../../../../../monad.md). It is not an [idempotent monad](../../../../../../idempotent-monad.md), since $\mu(0)=\mu(1)$, so $\mu$ cannot be invertible.

An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is a map $a\in M$ with $a\eta=1$ and $aTa=a\mu$. The first equation forces $a(n+1)=n$; monotonicity then forces $a(0)=0$. Thus $a=\mu$, which satisfies the second equation by the monad associativity law. The [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) therefore has exactly one object. Its endomorphisms $h$ satisfy $h\mu=\mu Th$, and this equation holds precisely when $h(0)=0$: evaluate at zero for necessity, and at $n>0$ both sides equal $h(n-1)$.

The [Kleisli comparison functor](../../../../../../kleisli-comparison-functor.md) takes its only object to this only algebra and sends $f\in M$ to

$$
K(f)=\mu Tf,\qquad K(f)(0)=0,\qquad K(f)(n+1)=f(n).
$$

It is a bijection from the Kleisli arrows to the algebra endomorphisms, with inverse $h\mapsto(n\mapsto h(n+1))$. It preserves identities and composition by the comparison construction; directly, $K(\eta)=1$ and $K(g\star f)=K(g)K(f)$. Bijectivity on objects and arrows makes it an isomorphism of [categories](../../../../../../category-split.md):

$$
\boxed{M_T\cong M^T,\qquad \mu\text{ is not invertible}.}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 119](../../../paper-119-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
