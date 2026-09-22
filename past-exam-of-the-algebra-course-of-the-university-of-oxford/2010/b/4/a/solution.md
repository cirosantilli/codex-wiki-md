<h1 id="b/4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [Abelian](../../../../../abelian-group.md) case of [Cauchy theorem for groups](../../../../../cauchy-theorem-for-groups.md), use induction on $|G|$. Choose $a\ne e$. If $p$ divides $m=|a|$, then $a^{m/p}$ has order $p$. Otherwise $\langle a\rangle$ is a nontrivial [normal subgroup](../../../../../normal-subgroup.md) of order prime to $p$, and $G/\langle a\rangle$ has smaller order still divisible by $p$. Induction gives a coset of order $p$; any lift $b$ has order divisible by $p$, because the order of its [image](../../../../../image-of-a-function.md) divides its own order. A suitable power of $b$ then has order $p$. This uses no classification of finite [Abelian groups](../../../../../abelian-group.md).

For a finite [p-group](../../../../../p-group.md), the [class equation](../../../../../class-equation.md) is

$$
|G|=|Z(G)|+\sum_{[g]\ne\{z\}}[G:C_G(g)],
$$

where the sum is over noncentral [conjugacy classes](../../../../../conjugacy-class.md). Each index is a positive power of $p$, hence divisible by $p$. Therefore $p$ divides $|Z(G)|$, and the [center of a group](../../../../../center-of-a-group.md) is nontrivial.

If $|G|=p^n$ with $n>1$ and $Z(G)\ne G$, this is already a proper nontrivial [normal subgroup](../../../../../normal-subgroup.md). If $Z(G)=G$, the [group](../../../../../group-split.md) is [Abelian](../../../../../abelian-group.md); the established case of [Cauchy theorem for groups](../../../../../cauchy-theorem-for-groups.md) gives a subgroup of order $p$, which is normal and proper. Thus

$$
\boxed{\text{No group of order }p^n\ (n>1)\text{ is simple}.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the algebra course of the University of Oxford](../../../../split.md)
6. [Algebra course of the University of Oxford](../../../../../algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
