<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First check the [ordered right cosets of a convex lattice subgroup](../../../../../../ordered-right-cosets-of-a-convex-lattice-subgroup.md). Replacing $g,h$ by $p_1g,p_2h$ changes a witness $g\le ph$ into $p_1g\le p_1pp_2^{-1}(p_2h)$, so the relation is independent of representatives. Reflexivity uses $p=1$. If $g\le ph$ and $h\le qk$, two-sided invariance of the [partial order](../../../../../../partially-ordered-set.md) gives $g\le pqk$, proving transitivity. If both inequalities hold in opposite directions, then

$$
g\le ph\le pqg,\qquad 1\le phg^{-1}\le pq.
$$

Both endpoints are in $P$, so convexity gives $phg^{-1}\in P$ and hence $hg^{-1}\in P$. Thus $Pg=Ph$, proving antisymmetry. The [join](../../../../../../least-upper-bound-in-a-partially-ordered-set.md) and [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) formulas are $Pg\vee Ph=P(g\vee h)$ and $Pg\wedge Ph=P(g\wedge h)$. For example, if $g\le pk$ and $h\le qk$, then $g\vee h\le(p\vee q)k$, giving the least-upper-bound property.

The coset order is total exactly when $P$ is a [prime convex lattice subgroup](../../../../../../prime-convex-lattice-subgroup.md). If it is total and $a,b\ge1$ have $a\wedge b=1$, assume $Pa\le Pb$. The coset [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) is then $Pa=P(a\wedge b)=P$, so $a\in P$. Conversely, for $u=gh^{-1}$, its [positive and negative parts in a lattice-ordered group](../../../../../../positive-and-negative-parts-in-a-lattice-ordered-group.md) satisfy $u^+\wedge u^-=1$. Primality puts one of them in $P$. If $u^+\in P$, then $u\le u^+$ gives $Pg\le Ph$; if $u^-\in P$, use $u^{-1}\le u^-$ to obtain $Ph\le Pg$.

It remains to identify the stated intersection condition. If $P$ is prime and $C,D$ properly contain it, choose positive $c\in C\setminus P$ and $d\in D\setminus P$. The cosets $Pc,Pd$ are strictly above $P$. Their [meet](../../../../../../greatest-lower-bound-in-a-partially-ordered-set.md) is therefore strictly above $P$, so $c\wedge d\notin P$. But $c\wedge d$ belongs to $C\cap D$ by convexity, showing $C\cap D\ne P$.

If $P$ is not prime, choose disjoint positive $a,b\notin P$. The [principal convex lattice subgroups](../../../../../../principal-convex-lattice-subgroup.md) $A=\langle a\rangle_c$ and $B=\langle b\rangle_c$ have $A\cap B=\{1\}$. Indeed, disjoint positive elements commute, since $a\vee b=a(a\wedge b)^{-1}b=ab=ba$, and [Riesz decomposition in a lattice-ordered group](../../../../../../riesz-decomposition-in-a-lattice-ordered-group.md) shows $a^r\wedge b^s=1$ for every positive $r,s$. Now the distributivity of the [lattice of convex lattice subgroups](../../../../../../lattice-of-convex-lattice-subgroups.md) gives

$$
(P\vee A)\cap(P\vee B)=P\vee(A\cap B)=P.
$$

Both joins properly contain $P$, violating the intersection condition. This proves the requested equivalence.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
