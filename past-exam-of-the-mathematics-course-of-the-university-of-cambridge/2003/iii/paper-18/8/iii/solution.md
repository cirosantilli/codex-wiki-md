<h1 id="8/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

First prove strict creation for the canonical forgetful [functor](../../../../../../functor.md) $U:\mathcal C^T\to\mathcal C$. Let a diagram of algebras $(A_i,a_i)$ have a chosen underlying limit cone $p_i:L\to A_i$. The maps $a_iT(p_i):TL\to A_i$ form a cone: if $h:A_i\to A_j$ is a diagram arrow, then $ha_i=a_jT(h)$ and $hp_i=p_j$. Thus the limit property gives a unique action $a:TL\to L$ with

$$
\boxed{p_i a=a_iT(p_i).}
$$

The projections are jointly monic. By naturality of $\eta$ and the algebra unit laws, $p_i a\eta_L=a_i\eta_{A_i}p_i=p_i$, hence $a\eta_L=1_L$. Likewise

$$
p_i a\mu_L=a_i\mu_{A_i}T^2p_i=a_iT(a_i)T^2p_i=p_i aT(a),
$$

so $a\mu_L=aT(a)$. Therefore $(L,a)$ is an algebra and all $p_i$ are algebra morphisms.

For any algebra cone $h_i:(B,b)\to(A_i,a_i)$, let $h:B\to L$ be its unique underlying factor. Then $p_i hb=h_i b=a_iT(h_i)=p_i aT(h)$, so joint monicity gives $hb=aT(h)$. Thus the factor is an algebra morphism, unique as such. The action on the prescribed $L$ was itself forced by the cone equations. This proves [monad algebra forgetful functor creates limits](../../../../../../monad-algebra-forgetful-functor-creates-limits.md), without assuming $T$ preserves them.

For a monadic $G$ with comparison an equivalence, transport $(L,a)$ and its cone across that equivalence. This yields a limiting cone in $\mathcal D$ whose image is identified with the prescribed base cone by an [isomorphism](../../../../../../isomorphism.md), uniquely up to the corresponding cone-compatible [isomorphism](../../../../../../isomorphism.md). Thus **a monadic [functor](../../../../../../functor.md) creates limits in the equivalence-invariant sense**. If monadicity uses a comparison [isomorphism](../../../../../../isomorphism.md) over the base, the lift is literally on the prescribed underlying cone, proving strict creation as well.

A qualification is necessary if equivalence is used to define monadicity but literal unique lifting is demanded. Let $\mathcal C$ be the [indiscrete category](../../../../../../indiscrete-category.md) on two objects $0,1$, let $\mathcal D$ be the terminal category, and let $G$ select $0$. The unique $F:\mathcal C\to\mathcal D$ is left adjoint to $G$, and the comparison to the induced algebra category is an equivalence: the two algebra objects have exactly one map between each pair. Yet the chosen terminal cone with vertex $1$ in $\mathcal C$ has no literal lift, since the only object in the image of $G$ is $0$. The [creation of limits up to isomorphism](../../../../../../creation-of-limits-up-to-isomorphism.md) conclusion holds, because $0$ and $1$ are uniquely isomorphic. This distinguishes the two conventions rather than claiming an invalid strict conclusion from equivalence alone.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
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
