# Center of a group

↑ **Parent:** [Group theory](group-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Center_(group_theory))

The center of a [group](group-split.md) consists of the elements that commute with every element of that [group](group-split.md):

$$
Z(G)=\{z\in G:zg=gz\text{ for every }g\in G\}=\bigcap_{g\in G}C_G(g),
$$

where $C_G(g)$ is the [centralizer](centralizer.md) of $g$. These are operations whose position in any product can be changed freely. The center is an [abelian group](abelian-group.md) and a [characteristic subgroup](characteristic-subgroup.md), hence a [normal subgroup](normal-subgroup.md). A [group](group-split.md) is an [abelian group](abelian-group.md) precisely when $Z(G)=G$.

For the [symmetric group](symmetric-group.md) $S_3$, the [conjugacy classes](conjugacy-class.md) are

$$
\{e\},\qquad\{(12),(13),(23)\},\qquad\{(123),(132)\}.
$$

An element belongs to the center precisely when its [conjugacy class](conjugacy-class.md) has one element, so $Z(S_3)=\{e\}$. Yet [commutator subgroup of the symmetric group on three letters](commutator-subgroup-of-the-symmetric-group-on-three-letters.md) gives $S_3'=A_3$, with three elements. Thus belonging to the [commutator subgroup](commutator-subgroup.md) does not mean commuting with everything. The [alternating group](alternating-group.md) $A_3$ is an [abelian group](abelian-group.md) as a [subgroup](subgroup.md), but its nonidentity elements do not commute with the [transpositions](transposition-permutation.md) in the surrounding $S_3$.

For the [dihedral group](dihedral-group.md) $D_8$ of [group order](order-of-a-finite-group.md) eight in [abelianization of the square symmetry group](abelianization-of-the-square-symmetry-group.md), the center is $\{e,r^2\}$. A [rotation](rotation-mathematics.md) $r^i$ commutes with $s$ precisely when $r^i=r^{-i}$, which requires $i$ even. No [reflection](reflection-mathematics.md) $r^is$ commutes with $r$, since $(r^is)r=r^{i-1}s$ whereas $r(r^is)=r^{i+1}s$. Consequently

$$
Z(D_8)=\{e,r^2\}=D_8'.
$$

The half-turn can be performed before or after any [square](square.md) symmetry with the same result. Its appearance both here and in the [commutator subgroup](commutator-subgroup.md) is a feature of this example, rather than a general equality. See [Conrad, Dihedral groups I, theorem 3.4 and example 3.5](https://kconrad.math.uconn.edu/blurbs/grouptheory/dihedral.pdf).

The center and the [commutator subgroup](commutator-subgroup.md) answer different useful questions: which operations already commute with everything, and which operations must disappear for the entire [group](group-split.md) to commute. In an [abelian group](abelian-group.md) these answers are $Z(G)=G$ and $G'=\{e\}$. Another way to use the center is through [conjugation](conjugation.md): the [group homomorphism](group-homomorphism.md) $g\mapsto(h\mapsto ghg^{-1})$ has [group kernel](kernel-of-a-group-homomorphism.md) $Z(G)$, so the [first isomorphism theorem](first-isomorphism-theorem.md) gives $G/Z(G)\cong\operatorname{Inn}(G)$, the [inner automorphism group](inner-automorphism.md). The [quotient group](quotient-group.md) by the center thus records the distinct conjugation operations; it need not be an [abelian quotient](abelian-quotient.md).

A nontrivial finite [p-group](p-group.md) always has a nontrivial center. In the [class equation](class-equation.md), each noncentral [conjugacy class](conjugacy-class.md) has size divisible by $p$, so $|Z(G)|\equiv|G|\equiv0\pmod p$. The [identity element](identity-element.md) ensures $Z(G)$ is nonempty, hence it has at least $p$ elements. See [McKernan, MIT 18.703, lemmas 23.6–23.7 and definition-lemma 23.10](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/96221ce2d5b1077b3e5d3c5e08c88afe_MIT18_703S13_pra_l_23.pdf).

**Table of contents**

- [Central element of a group](central-element-of-a-group.md)
- [Cyclic quotient by the center](cyclic-quotient-by-the-center.md)

## ↑ Ancestors (5)

1. [Group theory](group-theory-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (49)

- [Abelian subgroup cannot have prime-power index in a nonabelian simple group](abelian-subgroup-cannot-have-prime-power-index-in-a-nonabelian-simple-group.md)
- [Center of a Lie algebra](center-of-a-lie-algebra.md)
- [Center quotient of the real Heisenberg group](center-quotient-of-the-real-heisenberg-group.md)
- [Central element of a group](central-element-of-a-group.md)
- [Central intersection property of normal subgroups of finite p-groups](central-intersection-property-of-normal-subgroups-of-finite-p-groups.md)
- [Centralizer](centralizer.md)
- [Class equation](class-equation.md)
- [Classical group](classical-group.md)
- [Classification of groups of order p squared](classification-of-groups-of-order-p-squared.md)
- [Commutator subgroup of the symmetric group on three letters](commutator-subgroup-of-the-symmetric-group-on-three-letters.md)
- [Conjugacy class](conjugacy-class.md)
- [Conjugacy classes of the symmetric group on three letters](conjugacy-classes-of-the-symmetric-group-on-three-letters.md)
- [Heisenberg group over a commutative ring](heisenberg-group-over-a-commutative-ring.md)
- [Modular Heisenberg group](modular-heisenberg-group.md)
- [Nontrivial center of a finite p-group](nontrivial-center-of-a-finite-p-group.md)
- [Normal subgroup of order two is central](normal-subgroup-of-order-two-is-central.md)
- [Normalizer](normalizer.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-53/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-7/1/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/5d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-4/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/6d/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/8d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-1/18g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-4/2g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/21f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-149/4/c/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ii/paper-1/19i/c/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ia/paper-3/5e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ii/paper-4/19h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2026/iii/paper-133/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/9/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-2/8/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/8/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/8/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-2/9/c/solution.md)
- [Two-step nilpotent group](two-step-nilpotent-group.md)
- [Upper central series](upper-central-series.md)
