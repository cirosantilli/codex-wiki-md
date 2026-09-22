<h1 id="10/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [monad](../../../../../../monad.md) on $\mathcal C$ consists of an [endofunctor](../../../../../../endofunctor.md) $T$ and [natural transformations](../../../../../../natural-transformation.md) $\eta:1\to T$, $\mu:T^2\to T$ satisfying, at every object $A$,

$$
\mu_A T\mu_A=\mu_A\mu_{TA},\qquad\mu_A\eta_{TA}=1_{TA}=\mu_A T\eta_A.
$$

These are the associativity and unit laws. An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is $(A,a:TA\to A)$ with

$$
a\eta_A=1_A,\qquad aT a=a\mu_A.
$$

A [monad algebra morphism](../../../../../../morphism-of-algebras-for-a-monad.md) $h:(A,a)\to(B,b)$ is a [morphism](../../../../../../morphism.md) $h:A\to B$ satisfying $ha=bTh$. [Identity morphisms](../../../../../../identity-morphism.md) satisfy this equation, and if $h,k$ satisfy it, then $kha=kbTh=cTkTh=cT(kh)$. Hence these objects and [morphisms](../../../../../../morphism.md) form the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) $\mathcal C^T$, with the [forgetful functor](../../../../../../forgetful-functor.md) $U(A,a)=A$ and $Uh=h$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [10](../../10.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
