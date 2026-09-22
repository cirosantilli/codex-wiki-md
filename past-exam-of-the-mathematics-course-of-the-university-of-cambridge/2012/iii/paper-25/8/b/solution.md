<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In an [abelian category](../../../../../../abelian-category.md), for $f:A\to B$ set $\operatorname{coim}f=\operatorname{coker}(\ker f)$ and $\operatorname{im}f=\ker(\operatorname{coker}f)$. The canonical map from coimage to image is an [isomorphism](../../../../../../isomorphism.md). Thus the [image factorization in an abelian category](../../../../../../image-factorization-in-an-abelian-category.md) is

$$
\boxed{A\xrightarrow{e}\operatorname{im}f\xrightarrow{m}B,\qquad f=me,\quad e\text{ epic},\quad m\text{ monic},}
$$

unique up to a unique compatible [isomorphism](../../../../../../isomorphism.md).

The [short five lemma](../../../../../../short-five-lemma.md) states that in a commuting diagram of [short exact sequences](../../../../../../short-exact-sequence.md) $0\to L\to M\to R\to0$ and $0\to L'\to M'\to R'\to0$ in an [abelian category](../../../../../../abelian-category.md), if the vertical maps $L\to L'$ and $R\to R'$ are [isomorphisms](../../../../../../isomorphism.md), then so is $M\to M'$.

For the [Five lemma](../../../../../../five-lemma.md), consider commuting exact rows

$$
A_1\xrightarrow{d_1}A_2\xrightarrow{d_2}A_3\xrightarrow{d_3}A_4\xrightarrow{d_4}A_5,
\qquad
B_1\xrightarrow{d'_1}B_2\xrightarrow{d'_2}B_3\xrightarrow{d'_3}B_4\xrightarrow{d'_4}B_5,
$$

with vertical maps $v_i:A_i\to B_i$. We prove the usual stronger version: $v_1$ epic, $v_2$ and $v_4$ invertible, and $v_5$ monic imply that $v_3$ is invertible. In particular the conclusion holds if all four outer vertical maps are [isomorphisms](../../../../../../isomorphism.md).

Put $L=\operatorname{im}d_2$ and $R=\operatorname{im}d_3$, and define $L',R'$ similarly. Exactness gives [short exact sequences](../../../../../../short-exact-sequence.md)

$$
0\longrightarrow L\longrightarrow A_3\longrightarrow R\longrightarrow0,
\qquad
0\longrightarrow L'\longrightarrow B_3\longrightarrow R'\longrightarrow0.
$$

The [functoriality of abelian image factorization](../../../../../../functoriality-of-abelian-image-factorization.md) supplies their vertical outer maps. We show that both are [isomorphisms](../../../../../../isomorphism.md).

First, $L\cong\operatorname{coker}d_1$ and $L'\cong\operatorname{coker}d'_1$: exactness at $A_2$ identifies $\operatorname{im}d_1$ with $\ker d_2$, and the image-coimage [isomorphism](../../../../../../isomorphism.md) for $d_2$ gives the claimed cokernel. Write $q:A_2\to L$ and $q':B_2\to L'$ for these [categorical cokernels](../../../../../../cokernel-in-a-category.md). To construct an inverse to the induced map $\ell:L\to L'$, observe

$$
(qv_2^{-1}d'_1)v_1=qv_2^{-1}v_2d_1=0.
$$

Cancellation of the [epimorphism](../../../../../../epimorphism.md) $v_1$ gives $qv_2^{-1}d'_1=0$, so $qv_2^{-1}$ factors uniquely as $\bar\ell q'$ with $\bar\ell:L'\to L$. From $\ell q=q'v_2$, composing with the epic $q,q'$ gives $\bar\ell\ell=1_L$ and $\ell\bar\ell=1_{L'}$.

Second, $R\cong\ker d_4$ and $R'\cong\ker d'_4$ by exactness at the fourth objects. Write their inclusions as $j:R\to A_4$ and $j':R'\to B_4$. The equality $d'_4v_4=v_5d_4$ gives the induced map $\rho:R\to R'$. Since

$$
v_5d_4v_4^{-1}j'=d'_4j'=0
$$

and $v_5$ is a [monomorphism](../../../../../../monomorphism.md), $d_4v_4^{-1}j'=0$. Kernel universality gives $\bar\rho:R'\to R$ with $j\bar\rho=v_4^{-1}j'$. Cancelling the monic $j,j'$ proves $\bar\rho\rho=1_R$ and $\rho\bar\rho=1_{R'}$.

Apply the [short five lemma](../../../../../../short-five-lemma.md) to the two [short exact sequences](../../../../../../short-exact-sequence.md): their outer maps $\ell,\rho$ are invertible, so **$v_3$ is an [isomorphism](../../../../../../isomorphism.md)**. This [five lemma via image factorization](../../../../../../five-lemma-via-image-factorization.md) argument uses only universal properties and therefore works in any [abelian category](../../../../../../abelian-category.md), without treating its objects as literal sets of elements.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 25](../../../paper-25-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
