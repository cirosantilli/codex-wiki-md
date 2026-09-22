# Coset action

↑ **Parent:** [Group action](group-action-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Coset_action)

A group acts on the left cosets of a subgroup by left multiplication; its kernel is the core of that subgroup.

Let $H\leq G$ be a [subgroup](subgroup.md). The notation $G/H$ here means the [set](set-split.md) of left [cosets](coset.md) $\{aH:a\in G\}$, even when $H$ is not a [normal subgroup](normal-subgroup.md). Define

$$
g\cdot(aH)=(ga)H,\qquad
\rho_H:G\longrightarrow\operatorname{Sym}(G/H).
$$

This gives a [group action](group-action-split.md) without needing a [quotient group](quotient-group.md) structure on $G/H$.[Example 2.12, printed pages 7–8: left multiplication on left cosets, without normality](group-actions-by-keith-conrad.md)

The representative check is essential: if $aH=bH$, then $a=bh$ for some $h\in H$, and $(ga)H=(gbh)H=(gb)H$. Thus equal input [cosets](coset.md) give equal output [cosets](coset.md). The [identity element](identity-element.md) fixes every [coset](coset.md), and [associativity](associative-property.md) gives $g_1\cdot(g_2\cdot aH)=(g_1g_2)\cdot aH$. Each induced map is a [permutation](permutation.md), with inverse induced by $g^{-1}$. This is a [transitive group action](transitive-group-action.md) because $ba^{-1}$ sends $aH$ to $bH$.

The [stabilizer subgroup](stabilizer-subgroup.md) of $H$ is $H$ itself. At a general [coset](coset.md), the [stabilizer subgroup](stabilizer-subgroup.md) and the [group kernel](kernel-of-a-group-homomorphism.md) are

$$
G_{aH}=aHa^{-1},\qquad
\ker\rho_H=\bigcap_{a\in G}aHa^{-1}=\operatorname{Core}_G(H).
$$

Consequently the [coset action](coset-action.md) is a [faithful group action](faithful-group-action.md) exactly when the [subgroup core](core-group-theory.md) is trivial.[Chapter 4, Action on the left cosets, printed page 64, formulas preceding Remark 4.22 and Remark 4.22(a)](group-theory-v4-01-by-james-s-milne.md)

Indeed, $g\cdot(aH)=aH$ exactly when $a^{-1}ga\in H$, or $g\in aHa^{-1}$. Intersecting these membership conditions over all [cosets](coset.md) gives the [group kernel](kernel-of-a-group-homomorphism.md). [Conjugation](conjugation.md) permutes the [subgroups](subgroup.md) in this intersection, making it a [normal subgroup](normal-subgroup.md) of $G$ contained in $H$. Conversely, any [normal subgroup](normal-subgroup.md) of $G$ contained in $H$ lies in every $aHa^{-1}$. This explains why the [subgroup core](core-group-theory.md) is the largest such [normal subgroup](normal-subgroup.md): it is exactly the portion of $H$ invisible at every label, rather than merely at the label $H$.

For a [normal subgroup](normal-subgroup.md) $H$, every $aHa^{-1}$ equals $H$, so $\ker\rho_H=H$. For $H=\{e\}$, the construction is the [regular group action](regular-group-action.md) behind [Cayley's theorem](cayley-s-theorem.md). Between these extremes, a nontrivial [subgroup](subgroup.md) with trivial [subgroup core](core-group-theory.md) can give a [faithful group action](faithful-group-action.md) on fewer labels. If the [index of a subgroup](index-of-a-subgroup.md) is finite, $[G:H]=n$, the [first isomorphism theorem](first-isomorphism-theorem.md) gives

$$
G/\operatorname{Core}_G(H)\cong\operatorname{im}\rho_H\leq S_n.
$$

Thus a [subgroup](subgroup.md) of small [index of a subgroup](index-of-a-subgroup.md) exposes a small [permutation group](permutation-group.md) associated with $G$. The two examples below and in [nonfaithful coset action of the symmetric group on three letters](nonfaithful-coset-action-of-the-symmetric-group-on-three-letters.md) show exactly which information can survive.

**Table of contents**

- [Faithful coset action of the symmetric group on three letters](faithful-coset-action-of-the-symmetric-group-on-three-letters.md)

## ↑ Ancestors (6)

1. [Group action](group-action-split.md)
2. [Group theory](group-theory-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Coset](coset.md)
- [Coset action](coset-action.md)
- [Faithful coset action of the symmetric group on three letters](faithful-coset-action-of-the-symmetric-group-on-three-letters.md)
- [Faithful group action](faithful-group-action.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-1/10e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-3/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-3/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-151/3/a/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/9e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ia/paper-3/7d/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ib/paper-1/9e/a/solution.md)
- [Permutation character of a coset action](permutation-character-of-a-coset-action.md)
