# Centralizer and normalizer

↑ **Parent:** [Conjugation action](conjugation-action.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Centralizer_and_normalizer)

Both constructions are [stabilizer subgroups](stabilizer-subgroup.md) for the [conjugation action](conjugation-action.md). The [centralizer](centralizer.md) $C_G(x)$ fixes an individual element $x$; the [normalizer](normalizer.md) $N_G(H)$ preserves a [subgroup](subgroup.md) $H$ as a whole, while possibly moving its elements. The [centralizer of a subset](centralizer-of-a-subset.md) $C_G(H)$ fixes every member of $H$ individually, so

$$
C_G(H)\subseteq N_G(H).
$$

For a [cyclic subgroup](cyclic-subgroup.md) $H=\langle r\rangle$, commuting with the [group generator](generator-of-a-group.md) $r$ is equivalent to commuting with all its powers, giving $C_G(H)=C_G(r)$.

In the [symmetric group](symmetric-group.md) $S_3$, let $r=(123)$ and $H=\langle r\rangle=\{e,(123),(132)\}$. Then

$$
C_{S_3}(r)=C_{S_3}(H)=H,\qquad N_{S_3}(H)=S_3.
$$

Every [transposition](transposition-permutation.md) sends $r$ to $r^{-1}$ under [conjugation](conjugation.md). In particular, for $t=(12)$,

$$
trt^{-1}=r^{-1}\ne r,\qquad tHt^{-1}=\{e,r^{-1},r\}=H.
$$

Thus $t$ belongs to the [normalizer](normalizer.md) of $H$ but not to the [centralizer](centralizer.md) of $r$. Preserving the collection of powers allows the two possible directions of its [group generator](generator-of-a-group.md) to be exchanged.

<a id="image-the-centralizer-fixes-r-123-while-the-normalizer-preserves-h-langle-r-rangle-and-may-exchange-r-with-its-inverse-element"></a>
![](s3-centralizer-versus-normalizer.png)

**[Figure 10](#image-the-centralizer-fixes-r-123-while-the-normalizer-preserves-h-langle-r-rangle-and-may-exchange-r-with-its-inverse-element). The centralizer fixes $r=(123)$, while the normalizer preserves $H=\langle r\rangle$ and may exchange $r$ with its inverse element**.

This distinction lets one ask separately which operations leave a chosen operation unchanged and which operations preserve the [subgroup](subgroup.md) it generates. The [normalizer](normalizer.md) also supplies a [group homomorphism](group-homomorphism.md) to the [automorphism group](automorphism-group.md) of $H$, by $g\mapsto(h\mapsto ghg^{-1})$; its [group kernel](kernel-of-a-group-homomorphism.md) is $C_G(H)$. In this example the [group homomorphism](group-homomorphism.md) has two possible outputs, fixing $r$ or replacing it by $r^{-1}$. The [quotient group](quotient-group.md) $N_{S_3}(H)/C_{S_3}(H)$ is therefore a [cyclic group](cyclic-group.md) of [group order](order-of-a-finite-group.md) two. Milne develops the [normalizer](normalizer.md) as a [stabilizer subgroup](stabilizer-subgroup.md) in [Group Theory (v4.01) by James S. Milne](group-theory-v4-01-by-james-s-milne.md).

**Table of contents**

- [Centralizer](centralizer.md)
  - [Centralizer of a subset](centralizer-of-a-subset.md)
  - [Centraliser of a fixed-point-free involution](centraliser-of-a-fixed-point-free-involution.md)
  - [Centraliser of a transposition](centraliser-of-a-transposition.md)
- [Normalizer](normalizer.md)
  - [Normalizer of a diagonal subgroup of GL2](normalizer-of-a-diagonal-subgroup-of-gl2.md)

## ↑ Ancestors (7)

1. [Conjugation action](conjugation-action.md)
2. [Group action](group-action.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Conjugacy classes of the symmetric group on three letters](conjugacy-classes-of-the-symmetric-group-on-three-letters.md)
- [Normalizer](normalizer.md)
