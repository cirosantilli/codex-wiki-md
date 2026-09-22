<h1 id="8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In an [abelian category](../../../../../../abelian-category.md), the [image factorization in an abelian category](../../../../../../image-factorization-in-an-abelian-category.md) of $f:A\to B$ is

$$
A\xrightarrow{p}\operatorname{im}f\xrightarrow{i}B,
\qquad p=\operatorname{coker}(\ker f),\quad i=\ker(\operatorname{coker}f),\quad f=ip,
$$

where the abelian-category axiom identifies coimage with image. Thus $p$ is epic and $i$ is monic. Any other epi-mono factorization $f=jq$ has $\ker q=\ker f$ and $\operatorname{coker}j=\operatorname{coker}f$. Since [epimorphisms](../../../../../../epimorphism.md) are cokernels of their kernels, its middle object is canonically isomorphic to $\operatorname{im}f$, uniquely compatibly with the two factors.

For a square $vf=f'u$, define $I(u,v):\operatorname{im}f\to\operatorname{im}f'$ by

$$
I(u,v)p=p'u,\qquad i'I(u,v)=vi.
$$

The first arrow exists because $u\ker f$ factors through $\ker f'$, so $p'u$ annihilates $\ker f$. Its composite with $i'$ equals $vi$ after the [epimorphism](../../../../../../epimorphism.md) $p$, proving the second equation. Uniqueness after $p$ proves preservation of identities and composition. This gives the [functoriality of abelian image factorization](../../../../../../functoriality-of-abelian-image-factorization.md) as a [functor](../../../../../../functor.md) from the [arrow category](../../../../../../arrow-category.md).

For [pullback stability of abelian image factorization](../../../../../../pullback-stability-of-abelian-image-factorization.md), state the standard facts that pullbacks preserve [monomorphisms](../../../../../../monomorphism.md), [epimorphisms](../../../../../../epimorphism.md) in an [abelian category](../../../../../../abelian-category.md) are stable under pullback, and two adjoining pullback squares have pullback outer rectangle. In the given diagram, $i'$ is therefore monic and $p'$ is epic, while the composite $i'p'$ is the pullback of $f$. Its epi-mono factorization is an image factorization by the uniqueness just proved. Thus the top row is the image factorization of the pulled-back arrow, with its middle object canonically the pullback of the original image subobject.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [8](../../8.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
