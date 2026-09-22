<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Here is an [involution](../../../../../../involution.md) form of the [double-coset criterion for a one-point extension](../../../../../../double-coset-criterion-for-a-one-point-extension.md). Embed $G$ in $\operatorname{Sym}(\Omega\cup\{\infty\})$ by fixing $\infty$, choose $a\in\Omega$, and put $H=G_a$. The necessary and sufficient condition is the existence of an [involution](../../../../../../involution.md) $t$ such that

$$
\boxed{t(\infty)=a,\quad t(a)=\infty,\quad tHt=H,\quad tgt\in GtG\ \text{for every }g\in G\setminus H.}
$$

Products in this part are compositions of maps, with the rightmost map applied first. The criterion is a finite test on permutations of the enlarged set; it does not presuppose that a larger group has already been found.

For sufficiency, put $K=G\cup GtG$. Multiplying a [double coset](../../../../../../double-coset.md) by an element of $G$ on either side leaves it unchanged. A product of two elements of $GtG$ reduces to $g_1tgtg_2$. If $g\in H$, then $tgt\in H\le G$; otherwise the last condition puts it in $GtG$. Hence $K$ is closed under multiplication. It contains the identity and is closed under inverses, since $t^{-1}=t$, so it is a group.

Every element $g_1tg_2$ sends $\infty$ to $g_1(a)\in\Omega$, whereas elements of $G$ fix $\infty$. Thus $K_\infty=G$. Moreover the orbit of $\infty$ contains $a$ and then all of $\Omega$, so $K$ is transitive and is the desired [one-point extension of a permutation group](../../../../../../one-point-extension-of-a-permutation-group.md). For the order check, $G\cap tGt=H$: an element of the intersection fixes both $\infty$ and $a$, and the reverse containment follows from $tHt=H$. Consequently $|GtG|=|G|^2/|H|=|\Omega||G|$, as required.

For necessity, let $K$ be an extension. It is [doubly transitive group action](../../../../../../two-transitive-group-action.md), of order $|\Omega|(|\Omega|+1)|G_a|$, which is even. By [Cauchy theorem for groups](../../../../../../cauchy-theorem-for-groups.md) it contains a nontrivial [involution](../../../../../../involution.md), and a pair interchanged by this [involution](../../../../../../involution.md) can be carried to $(\infty,a)$ by double transitivity. Conjugating gives an [involution](../../../../../../involution.md) $t$ interchanging these two points. Their common [point stabilizer](../../../../../../stabilizer-subgroup.md) is $H$, so $tHt=H$. Finally $G$ has just two orbits on the enlarged set, namely $\{\infty\}$ and $\Omega$, giving $K=G\cup GtG$. More explicitly, for $k\in K\setminus G$, choose $g\in G$ with $g(a)=k(\infty)$; then $tg^{-1}k$ fixes $\infty$ and belongs to $G$. If $g\notin H$, the element $tgt$ moves $\infty$, so it belongs to $GtG$, completing necessity.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
