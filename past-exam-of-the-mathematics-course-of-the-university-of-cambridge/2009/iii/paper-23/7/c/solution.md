<h1 id="7/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Define the [free algebra functor](../../../../../../free-algebra-functor.md) by

$$
F^T(X)=(TX,\mu_X),\qquad F^T(f)=Tf.
$$

The [monad](../../../../../../monad.md) laws say precisely that $\mu_X$ defines an [monad algebra](../../../../../../algebra-for-a-monad.md) structure on $TX$, while [naturality](../../../../../../naturality.md) of $\mu$ makes $Tf$ an [monad algebra](../../../../../../algebra-for-a-monad.md) [morphism](../../../../../../morphism.md). We construct the [adjunction](../../../../../../adjoint-functors.md) explicitly.

For an [monad algebra](../../../../../../algebra-for-a-monad.md) $(A,a)$ and a [morphism](../../../../../../morphism.md) $f:X\to A$, put $\overline f=aTf:TX\to A$. It is an [monad algebra](../../../../../../algebra-for-a-monad.md) [morphism](../../../../../../morphism.md) because

$$
\overline f\mu_X=aTf\mu_X=a\mu_A T^2f
=aTaT^2f=aT\overline f.
$$

Conversely, from an [monad algebra](../../../../../../algebra-for-a-monad.md) [morphism](../../../../../../morphism.md) $h:(TX,\mu_X)\to(A,a)$ obtain $h\eta_X:X\to A$. These operations are inverse: [naturality](../../../../../../naturality.md) of $\eta$ and the [monad algebra](../../../../../../algebra-for-a-monad.md) unit law give

$$
aTf\eta_X=a\eta_A f=f,
$$

and the algebra-morphism equation together with the [monad](../../../../../../monad.md) unit law gives

$$
aT(h\eta_X)=aThT\eta_X=h\mu_XT\eta_X=h.
$$

The formulas commute with precomposition in $X$ and composition with [monad algebra](../../../../../../algebra-for-a-monad.md) [morphisms](../../../../../../morphism.md) in $(A,a)$, so the [bijections](../../../../../../bijection.md) are natural. Therefore the [free-forgetful Eilenberg-Moore adjunction](../../../../../../free-forgetful-eilenberg-moore-adjunction.md) is

$$
\boxed{F^T\dashv U,\qquad\mathcal C^T(F^TX,(A,a))\cong\mathcal C(X,A).}
$$

Its unit is $\eta_X$ and its counit at $(A,a)$ is the [monad algebra](../../../../../../algebra-for-a-monad.md) action $a$.

## ↑ Ancestors (11)

1. [C](../c.md)
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
