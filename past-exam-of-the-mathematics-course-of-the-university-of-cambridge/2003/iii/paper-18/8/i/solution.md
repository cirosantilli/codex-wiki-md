<h1 id="8/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [monad](../../../../../../monad.md) on $\mathcal C$ consists of an endofunctor $T$ and [natural transformations](../../../../../../natural-transformation.md) $\eta:1\Rightarrow T$, $\mu:T^2\Rightarrow T$, satisfying

$$
\mu\,T\eta=1_T=\mu\,\eta_T,\qquad\mu\,T\mu=\mu\,\mu_T.
$$

An [algebra for a monad](../../../../../../algebra-for-a-monad.md) is $(A,a)$ with $a:TA\to A$, $a\eta_A=1_A$ and $a\mu_A=aT(a)$. A morphism $(A,a)\to(B,b)$ is an arrow $h:A\to B$ with $ha=bT(h)$. These form the [Eilenberg-Moore category](../../../../../../eilenberg-moore-category.md) $\mathcal C^T$.

A [functor](../../../../../../functor.md) $G:\mathcal D\to\mathcal C$ is monadic when it has a left adjoint $F$ and its comparison $K:\mathcal D\to\mathcal C^{GF}$ is an equivalence; this is the [monadic adjunction](../../../../../../monadic-adjunction.md) convention. Some strict formulations require $K$ to be an [isomorphism](../../../../../../isomorphism.md) over the base. The distinction affects the meaning of literal limit creation, discussed in part (iii), but not the algebra construction.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [8](../../8.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
