# Abelianization of the square symmetry group

↑ **Parent:** [Abelianization](abelianization.md)

Let $D_8$ denote the [dihedral group](dihedral-group.md) of [group order](order-of-a-finite-group.md) eight acting on a [square](square.md). Here the subscript specifies [group order](order-of-a-finite-group.md); the same [group](group-split.md) is called $D_4$ in the convention that counts [vertices of a polygon](vertex-of-a-polygon.md), as in the [group action](group-action-split.md) example. Let $r$ be a counterclockwise quarter-turn [rotation](rotation-mathematics.md) and $s$ a [reflection](reflection-mathematics.md) in a diagonal. Then

$$
D_8=\{e,r,r^2,r^3,s,rs,r^2s,r^3s\},\qquad r^4=s^2=e,\quad srs=r^{-1}.
$$

Products act rightmost first. The [group commutator](group-commutator.md) of the [generators of a group](generator-of-a-group.md) is

$$
[r,s]=r^{-1}s^{-1}rs=r^{-1}(srs)=r^{-2}=r^2.
$$

It is a half-turn [rotation](rotation-mathematics.md), so forcing $r$ and $s$ to commute must identify a half-turn with $e$.

<a id="image-the-eight-square-symmetries-become-four-elements-under-abelianization"></a>
![](square-group-abelianization.png)

**[Figure 4](#image-the-eight-square-symmetries-become-four-elements-under-abelianization). The eight square symmetries become four elements under abelianization**. Each column is a [coset](coset.md) of the [commutator subgroup](commutator-subgroup.md) $N=\{e,r^2\}$ in the [dihedral group](dihedral-group.md) of [group order](order-of-a-finite-group.md) eight. Vertex labels show where each original vertex goes. The map $r^is^j\mapsto(i\bmod2,j)$ retains quarter-turn [integer parity](parity-mathematics.md) and the presence of a [reflection](reflection-mathematics.md). The table adds the two bits separately modulo two, giving the [Klein four-group](klein-four-group.md) $C_2\times C_2$.

More concretely, write each element uniquely as $r^is^j$, with $0\leq i<4$ and $j\in\{0,1\}$. The [function](function-split.md)

$$
\phi:D_8\longrightarrow C_2\times C_2,\qquad \phi(r^is^j)=(i\bmod2,j)
$$

is a [surjective group homomorphism](surjective-group-homomorphism.md). Indeed, $srs=r^{-1}$ gives

$$
(r^is^j)(r^ks^\ell)=r^{i+(-1)^jk}s^{j+\ell},
$$

where the exponents are reduced modulo four and two. Modulo two, $-k$ and $k$ agree, so $\phi$ adds the two coordinates separately. Its [group kernel](kernel-of-a-group-homomorphism.md) is $N=\{e,r^2\}$. Since the target is an [abelian group](abelian-group.md), $D_8'\subseteq N$; since $[r,s]=r^2$, also $N\subseteq D_8'$. Thus

$$
D_8'=\{e,r^2\},\qquad D_8^{\mathrm{ab}}\cong C_2\times C_2.
$$

The four [cosets](coset.md) are $\{e,r^2\}$, $\{r,r^3\}$, $\{s,r^2s\}$, and $\{rs,r^3s\}$. Each [coset](coset.md) forgets the difference of a half-turn. The [quotient group](quotient-group.md) still distinguishes [rotations](rotation-mathematics.md) from [reflections](reflection-mathematics.md), and even from odd numbers of quarter-turns; the two surviving choices are independent. This is the [Klein four-group](klein-four-group.md), rather than the [cyclic group](cyclic-group.md) $C_4$, because each nonidentity element squares to the [identity element](identity-element.md). For the general [dihedral group](dihedral-group.md) calculation, see [Conrad, Dihedral groups I, theorem A.1](https://kconrad.math.uconn.edu/blurbs/grouptheory/dihedral.pdf); that source uses the vertex-count convention and $xyx^{-1}y^{-1}$ for individual [group commutators](group-commutator.md).

## ↑ Ancestors (7)

1. [Abelianization](abelianization.md)
2. [Commutator subgroup](commutator-subgroup.md)
3. [Group theory](group-theory-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Abelianization](abelianization.md)
- [Center of a group](center-of-a-group.md)
