# Normalizer

↑ **Parent:** [Centralizer and normalizer](centralizer-and-normalizer.md)

For a [subgroup](subgroup.md) $H$ of a [group](group-split.md) $G$, the [normalizer](normalizer.md) is

$$
N_G(H)=\{g\in G:gHg^{-1}=H\}.
$$

It is the [stabilizer subgroup](stabilizer-subgroup.md) of $H$ under the [conjugation action](conjugation-action.md) on [subgroups](subgroup.md). Its elements can permute members of $H$; they need not commute with them. For $r=(123)$ in the [symmetric group](symmetric-group.md) $S_3$, the [cyclic subgroup](cyclic-subgroup.md) $H=\langle r\rangle$ has [normalizer](normalizer.md) $S_3$, although the [centralizer](centralizer.md) of $r$ has only three elements, as illustrated in [centralizer and normalizer](centralizer-and-normalizer.md).

Every element of $H$ preserves $H$ under [conjugation](conjugation.md), so $H\subseteq N_G(H)$. Moreover, $H$ is a [normal subgroup](normal-subgroup.md) of $N_G(H)$, and this is the largest [subgroup](subgroup.md) of $G$ with that property. Indeed, any [subgroup](subgroup.md) in which $H$ is a [normal subgroup](normal-subgroup.md) consists entirely of elements preserving $H$ under [conjugation](conjugation.md). In particular, $N_G(H)=G$ exactly when $H$ is a [normal subgroup](normal-subgroup.md) of $G$.[Group Theory (v4.01) by James S. Milne](group-theory-v4-01-by-james-s-milne.md)

The [orbit-stabilizer theorem](orbit-stabilizer-theorem.md) counts distinct [conjugate subsets](conjugate-subset.md) of a [subgroup](subgroup.md) by

$$
\#\{gHg^{-1}:g\in G\}=[G:N_G(H)].
$$

For $H=\langle(123)\rangle$ in $S_3$, there is just one, since $[S_3:N_{S_3}(H)]=6/6=1$. For the [subgroup](subgroup.md) $K=\langle(12)\rangle=\{e,(12)\}$, preserving $K$ forces its unique nonidentity element to stay fixed. Hence $N_{S_3}(K)=C_{S_3}((12))=K$, and its three distinct [conjugate subsets](conjugate-subset.md) are $\{e,(12)\}$, $\{e,(13)\}$ and $\{e,(23)\}$. This is the [subgroup](subgroup.md) counterpart of counting a [conjugacy class](conjugacy-class.md) with a [centralizer](centralizer.md): the object being stabilized determines which denominator belongs in the count.[Group Theory (v4.01) by James S. Milne](group-theory-v4-01-by-james-s-milne.md)

The equality in the definition is essential. For a [subgroup](subgroup.md) $H$ that is a [finite group](finite-group.md), an inclusion $gHg^{-1}\subseteq H$ already gives equality by equal [cardinalities](cardinality.md). For an infinite [subgroup](subgroup.md), that inference can fail: [conjugation](conjugation.md) might carry it onto a proper [subgroup](subgroup.md). The [normal subgroup](normal-subgroup.md) criterion is therefore, with the explicit hypothesis $H\leq G$,

$$
H\mathrel{\trianglelefteq}G\quad\Longleftrightarrow\quad N_G(H)=G.
$$

No finiteness or [commutativity](commutativity.md) assumption is needed. A [normal subgroup](normal-subgroup.md) is preserved as a [set](set-split.md); its elements need not lie in the [center of a group](center-of-a-group.md).

There is a second useful count, distinct from counting conjugate [subgroups](subgroup.md). The [normalizer](normalizer.md) acts on $H$ itself by [group automorphisms](group-automorphism.md), giving the [group homomorphism](group-homomorphism.md)

$$
\theta:N_G(H)\longrightarrow\operatorname{Aut}(H),\qquad \theta(g)(h)=ghg^{-1}.
$$

Its [group kernel](kernel-of-a-group-homomorphism.md) is $C_G(H)$, so the [centralizer of a subset](centralizer-of-a-subset.md) is a [normal subgroup](normal-subgroup.md) of $N_G(H)$ and the [first isomorphism theorem](first-isomorphism-theorem.md) gives

$$
N_G(H)/C_G(H)\cong\operatorname{im}\theta\leq\operatorname{Aut}(H).
$$

This [quotient group](quotient-group.md) records the different rearrangements of $H$ induced by the surrounding [group](group-split.md). It gives a [faithful group action](faithful-group-action.md) on $H$, but need not be the entire [automorphism group](automorphism-group.md) of $H$. For example, take the ambient [group](group-split.md) $G=H=\langle(123)\rangle$. Since $G$ is an [abelian group](abelian-group.md), $N_G(H)=C_G(H)=G$, so the [quotient group](quotient-group.md) is trivial; nevertheless $r\mapsto r^{-1}$ is a nonidentity [group automorphism](group-automorphism.md) of $H$. Returning to the ambient [symmetric group](symmetric-group.md) $S_3$ makes that [group automorphism](group-automorphism.md) available through a [reflection](reflection-mathematics.md), and $N_{S_3}(H)/C_{S_3}(H)\cong C_2$. Its two [cosets](coset.md) are the three [rotations](rotation-mathematics.md) and the three [reflections](reflection-mathematics.md).

The [subgroup](subgroup.md) $H$ itself need not be contained in $C_G(H)$: their intersection is the [center of a group](center-of-a-group.md) $Z(H)$. It is contained precisely when $H$ is an [abelian group](abelian-group.md). Thus $N_G(H)/H$, which exists because $H$ is a [normal subgroup](normal-subgroup.md) of its [normalizer](normalizer.md), and $N_G(H)/C_G(H)$ answer different questions and should not be substituted for one another.

**Table of contents**

- [Normalizer of a diagonal subgroup of GL2](normalizer-of-a-diagonal-subgroup-of-gl2.md)

## ↑ Ancestors (8)

1. [Centralizer and normalizer](centralizer-and-normalizer.md)
2. [Conjugation action](conjugation-action.md)
3. [Group action](group-action-split.md)
4. [Group theory](group-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (46)

- [2-modular defect groups of A5](2-modular-defect-groups-of-a5.md)
- [Centralizer](centralizer.md)
- [Centralizer and normalizer](centralizer-and-normalizer.md)
- [Conjugate subgroup](conjugate-subgroup.md)
- [Conjugates of a proper subgroup do not cover a finite group](conjugates-of-a-proper-subgroup-do-not-cover-a-finite-group.md)
- [Degree-ten partition action of S6](degree-ten-partition-action-of-s6.md)
- [Elementary abelian subgroups in GL3 over F2](elementary-abelian-subgroups-in-gl3-over-f2.md)
- [Holomorph](holomorph.md)
- [Least-prime divisibility constraint for a finite simple group](least-prime-divisibility-constraint-for-a-finite-simple-group.md)
- [Normalizer](normalizer.md)
- [Normalizer action determines axial branch parity](normalizer-action-determines-axial-branch-parity.md)
- [Normalizer condition for finite p-groups](normalizer-condition-for-finite-p-groups.md)
- [Normalizer of a diagonal subgroup of GL2](normalizer-of-a-diagonal-subgroup-of-gl2.md)
- [P-local module](p-local-module.md)
- [P-radical subgroup](p-radical-subgroup.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-3/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-1/2f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-5/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-60/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-1/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ib/paper-3/11g/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-7/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-4/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/ia/paper-3/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/1/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-3/7d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/10e/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-4/2g/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-138/6/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/ib/paper-2/9e/solution.md)
- [Simple groups with order a power of two times fifteen](simple-groups-with-order-a-power-of-two-times-fifteen.md)
- [Source of an indecomposable module](source-of-an-indecomposable-module.md)
