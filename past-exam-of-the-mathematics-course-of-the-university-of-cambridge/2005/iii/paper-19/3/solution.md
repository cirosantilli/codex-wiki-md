<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

First correct the group-ring condition in the PDF. For an infinite [group](../../../../../group-split.md), a left-invariant element of $\mathbb Z\Gamma$ would have constant coefficients on the whole [group](../../../../../group-split.md); finite support then forces it to be zero. Hence $H^0(\Gamma,\mathbb Z\Gamma)=0$. For a [Poincare duality group](../../../../../poincare-duality-group.md) of positive dimension, the correct condition is

$$
\boxed{H^k(\Gamma,\mathbb Z\Gamma)=0\ (k\ne n),\qquad
H^n(\Gamma,\mathbb Z\Gamma)=D\cong\mathbb Z\ \text{as an abelian group}.}
$$

It must be accompanied by the finiteness condition: the trivial module has a finite-length resolution by [finitely generated projective modules](../../../../../finite-projective-module.md). The module $D$ has a right [group](../../../../../group-split.md) action, possibly an orientation-sign action. The degree-zero exception only applies to the trivial $PD^0$ [group](../../../../../group-split.md), not simultaneously to positive-dimensional [groups](../../../../../group-split.md).

Here is how the duality follows. Put $R=\mathbb Z\Gamma$ and take a length-$n$ [projective resolution](../../../../../projective-resolution.md) $P_*\to\mathbb Z$. Dualize to $P^* =\operatorname{Hom}_R(P_*,R)$. Its cohomology is zero except in degree $n$, where it is $D$. Reversing degrees therefore makes $Q_j=P_{n-j}^*$ a projective right-$R$ resolution of $D$. Finite generation and projectivity give, for every left $R$-module $V$, an isomorphism of cochain complexes

$$
\operatorname{Hom}_R(P_*,V)\cong P^*\otimes_R V.
$$

Taking cohomology and reversing the grading yields

$$
H^k(\Gamma,V)\cong\operatorname{Tor}^R_{n-k}(D,V).
$$

Since $D$ has underlying abelian [group](../../../../../group-split.md) $\mathbb Z$, its action is a sign character $\omega:\Gamma\to\{\pm1\}$. Twisting the resolution by this character identifies the right side with [group homology](../../../../../group-homology.md) having coefficient module $D\otimes_{\mathbb Z}V$, with diagonal left action $\gamma(d\otimes v)=\omega(\gamma)d\otimes\gamma v$. Thus

$$
\boxed{H^k(\Gamma,V)\cong H_{n-k}(\Gamma,D\otimes V).}
$$

For an orientable [Poincare duality group](../../../../../poincare-duality-group.md), $D$ is trivial and this is untwisted [Poincare duality](../../../../../poincare-duality.md). The natural isomorphism can equivalently be realized by [cap product](../../../../../cap-product.md) with the [group](../../../../../group-split.md) fundamental class. The reversed finite projective complex explains why the top group-ring condition produces duality for every coefficient module, rather than just matching integral Betti numbers.

Now let $H$ have finite index in $\Gamma$. There is an isomorphism of left $\Gamma$-modules

$$
\mathbb Z\Gamma\cong\operatorname{Coind}_H^\Gamma(\mathbb ZH).
$$

One explicit map sends $r\in\mathbb Z\Gamma$ to the $H$-linear function $g\mapsto\operatorname{pr}_H(gr)$, where $\operatorname{pr}_H$ retains only terms in $H$. Finite index ensures that all such functions arise in this way. [Shapiro's lemma](../../../../../shapiro-s-lemma.md) gives the isomorphism

$$
H^k(\Gamma,\mathbb Z\Gamma)\cong H^k(H,\mathbb ZH)
$$

as abelian [groups](../../../../../group-split.md). If $\Gamma$ is a [Poincare duality group](../../../../../poincare-duality-group.md), restricting its finite [projective resolution](../../../../../projective-resolution.md) to $H$ preserves projectivity and finite generation: the [group](../../../../../group-split.md) ring is finite free over $\mathbb ZH$. This proves that $H$ is $PD^n$.

For the converse one needs the usual ambient torsion-free hypothesis. The standard finite-index resolution lemmas say that type $FP_\infty$ is preserved under finite-index passage, and that a torsion-free [group](../../../../../group-split.md) of finite virtual cohomological dimension has the same integral cohomological dimension as a finite-index subgroup. Thus if $H$ is $PD^n$ and $\Gamma$ is torsion-free, $\Gamma$ has a finite resolution by finitely generated projective modules of length $n$. The preceding explicit coinduction and Shapiro calculation transfers exactly the required group-ring cohomology, and proves the [finite-index invariance of Poincare duality for torsion-free groups](../../../../../finite-index-invariance-of-poincare-duality-for-torsion-free-groups.md).

Without that hypothesis the claimed converse is false. Take $\Gamma=\mathbb Z\times C_2$ and $H=\mathbb Z\times1$. Then $H$ is index two and is $PD^1$, while $\Gamma$ contains torsion. Its [integral cohomological dimension of a group](../../../../../integral-cohomological-dimension-of-a-group.md) is infinite: restriction of any putative finite [projective resolution](../../../../../projective-resolution.md) to $C_2$ would contradict the nonzero cohomology $H^{2j}(C_2,\mathbb Z)=\mathbb Z/2$ for every $j\ge1$. Also, orientability need not ascend: the [torus](../../../../../torus.md) subgroup of the Klein-bottle [group](../../../../../group-split.md) has trivial orientation action, whereas the full [group](../../../../../group-split.md) has a nontrivial one. The invariant theorem concerns the possibly twisted notion of $PD^n$.

Finally, a closed aspherical [surface](../../../../../topological-surface.md) has a two-dimensional contractible [universal cover](../../../../../universal-cover.md) and exactly this compact-support duality, so its [surface group](../../../../../fundamental-group-of-a-surface.md) is $PD^2$. Conversely the algebraic condition forces the same local duality dimension and, in the orientable case, a nonsingular skew pairing on first cohomology, the familiar algebra of a closed orientable [surface](../../../../../topological-surface.md). Infinite-index subgroups behave like noncompact [surfaces](../../../../../topological-surface.md) rather than closed ones. These are strong reasons to expect a [surface group](../../../../../fundamental-group-of-a-surface.md); in fact the $PD^2$ classification theorem confirms that every integral $PD^2$ [group](../../../../../group-split.md) is the [fundamental group](../../../../../fundamental-group.md) of a closed aspherical [surface](../../../../../topological-surface.md). This includes the [torus](../../../../../torus.md) and, with orientation twist, the Klein bottle; the sphere and projective plane do not give $PD^2$ [groups](../../../../../group-split.md).

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 19](../../paper-19-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
