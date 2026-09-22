# Class equation

↑ **Parent:** [Conjugacy class](conjugacy-class.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Class_equation)

For a [finite group](finite-group.md) $G$, choose one representative $x_i$ from each [conjugacy class](conjugacy-class.md) with more than one element. The [class equation](class-equation.md) is

$$
|G|=|Z(G)|+\sum_i[G:C_G(x_i)]=|Z(G)|+\sum_i\frac{|G|}{|C_G(x_i)|},
$$

where $Z(G)$ is the [center of a group](center-of-a-group.md) and $C_G(x_i)$ is the [centralizer](centralizer.md) of $x_i$. Each central element contributes its own one-element [conjugacy class](conjugacy-class.md). Every remaining [conjugacy class](conjugacy-class.md) contributes its size, given by the [orbit-stabilizer theorem](orbit-stabilizer-theorem.md). The sum counts each element exactly once. See [McKernan, Group actions and automorphisms, lemma 23.6](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/96221ce2d5b1077b3e5d3c5e08c88afe_MIT18_703S13_pra_l_23.pdf).

For [conjugacy classes of the symmetric group on three letters](conjugacy-classes-of-the-symmetric-group-on-three-letters.md), take $x_1=(12)$ and $x_2=(123)$. Their [centralizers](centralizer.md) have sizes two and three, and the [center of a group](center-of-a-group.md) has size one, giving

$$
6=1+\frac62+\frac63=1+3+2.
$$

For an [abelian group](abelian-group.md), every [centralizer](centralizer.md) is the whole [group](group-split.md), every [conjugacy class](conjugacy-class.md) has size one, and the sum over noncentral representatives is empty.

The power of this counting identity is that the sizes of [conjugacy classes](conjugacy-class.md) constrain [group](group-split.md) structure. For a nontrivial finite [p-group](p-group.md) with [group order](order-of-a-finite-group.md) $p^n$, every noncentral [conjugacy class](conjugacy-class.md) has size a positive power of $p$, by [Lagrange's theorem](lagrange-s-theorem.md). The [class equation](class-equation.md) therefore gives $|Z(G)|\equiv0\pmod p$. Since the [identity element](identity-element.md) lies in the [center of a group](center-of-a-group.md), the [center of a group](center-of-a-group.md) must have at least $p$ elements. This obtains an element commuting with the entire [group](group-split.md) without constructing one. See [McKernan, lemma 23.7](https://ocw.mit.edu/courses/18-703-modern-algebra-spring-2013/96221ce2d5b1077b3e5d3c5e08c88afe_MIT18_703S13_pra_l_23.pdf).

Historically, these ideas belong to the nineteenth-century development of [permutation groups](permutation-group.md) and [normal subgroups](normal-subgroup.md). Milne's historical opening records Galois's introduction of [normal subgroups](normal-subgroup.md) in 1832 and Jordan's systematic treatment of [permutation groups](permutation-group.md) in 1870. This is context for the [conjugation action](conjugation-action.md) and the [class equation](class-equation.md), rather than a claim that either author first stated the modern formula.[Group Theory (v4.01) by James S. Milne](group-theory-v4-01-by-james-s-milne.md)

**Table of contents**

- [Prime-to-p conjugacy class lemma](prime-to-p-conjugacy-class-lemma.md)

## ↑ Ancestors (8)

1. [Conjugacy class](conjugacy-class.md)
2. [Conjugation action](conjugation-action.md)
3. [Group action](group-action-split.md)
4. [Group theory](group-theory-split.md)
5. [Algebra](algebra-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Center of a group](center-of-a-group.md)
- [Class equation](class-equation.md)
- [Conjugacy class](conjugacy-class.md)
- [Conjugacy classes of the symmetric group on three letters](conjugacy-classes-of-the-symmetric-group-on-three-letters.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-1/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ia/paper-3/5d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/11f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/1/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ia/paper-3/7d/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ia/paper-3/8d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/ib/paper-4/2g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/ia/paper-3/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-3/8d/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-1/10e/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/2e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/ib/paper-1/10g/b/solution.md)
- [Prime-to-p conjugacy class lemma](prime-to-p-conjugacy-class-lemma.md)
