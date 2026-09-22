<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Assume first $1\le t\le n$, and write $d=n-t$. The sharp [nonuniform t-intersecting family bound](../../../../../nonuniform-t-intersecting-family-bound.md) is

$$
\boxed{|\mathcal A|\le
\begin{cases}
\displaystyle\sum_{i=0}^q\binom ni,&d=2q,\\[3pt]
\displaystyle2\sum_{i=0}^q\binom{n-1}i,&d=2q+1.
\end{cases}}
$$

We prove the bound by deriving the needed [Kleitman diametric theorem](../../../../../kleitman-diametric-theorem.md). Identify [subsets](../../../../../subset.md) with binary words, with [Hamming distance](../../../../../hamming-distance.md) $|A\triangle B|$. Let $D(n,d)$ be the two expressions above. A [set family](../../../../../set-family.md) of [Hamming diameter](../../../../../diameter-of-a-set-family.md) at most $d<n$ has size at most $D(n,d)$, as follows.

First apply [downward coordinate compression](../../../../../downward-coordinate-compression.md): delete coordinate $i$ from a member only when its deletion is not already present. This preserves size and cannot increase the [Hamming diameter](../../../../../diameter-of-a-set-family.md). The only possible increased distance would be between a newly lowered member $A\setminus\{i\}$ and a retained member $B$ containing $i$. The deletion $B\setminus\{i\}$ must have belonged to the old [set family](../../../../../set-family.md), or $B$ would have been lowered too. The old pair $A,B\setminus\{i\}$ has precisely that increased distance, proving it was already allowed. Repeated downward compressions terminate in a [down-set](../../../../../down-set.md).

Next apply all [elementary set shifts](../../../../../elementary-set-shift.md) $S_{ij}$ with $i<j$. They preserve size and [Hamming diameter](../../../../../diameter-of-a-set-family.md). If shifting one member but retaining the other increased their distance, the retained member must contain $j$ but not $i$; its shifted partner was already present, and the old pair with that partner has the same distance. These shifts preserve the [down-set](../../../../../down-set.md) property: a [subset](../../../../../subset.md) of a shifted member either was already present or is obtained by shifting its corresponding old [subset](../../../../../subset.md). For a retained member, a [subset](../../../../../subset.md) cannot disappear, because the shifted partner of that [subset](../../../../../subset.md) is also a [subset](../../../../../subset.md) of the member or of its retained shifted partner. Repeated shifts terminate, since the sum of the selected coordinate labels decreases whenever a change occurs. We now have a shifted [down-set](../../../../../down-set.md) $\mathcal F$ of the same size and [Hamming diameter](../../../../../diameter-of-a-set-family.md).

Split it into sections on $[n-1]$:

$$
\mathcal F_0=\{A:n\notin A,\ A\in\mathcal F\},\qquad
\mathcal F_1=\{A:A\cup\{n\}\in\mathcal F\}.
$$

The first section has [Hamming diameter](../../../../../diameter-of-a-set-family.md) at most $d$. We claim the second has [Hamming diameter](../../../../../diameter-of-a-set-family.md) at most $d-2$. For $X,Y\in\mathcal F_1$, downward closure gives $X\setminus Y,Y\in\mathcal F_1$. Compare $(X\setminus Y)\cup\{n\}$ with $Y\in\mathcal F_0$. Their distance is $|X\cup Y|+1$, so $|X\cup Y|\le d-1<n-1$. Choose $i<n$ outside their union. Shiftedness puts $X\cup\{i\}$ in $\mathcal F_0$, while $Y\cup\{n\}$ is a member of $\mathcal F$. Their distance is $|X\triangle Y|+2$, proving the claim. For $d<2$ this argument forces $\mathcal F_1$ to be empty.

The induction now gives

$$
|\mathcal F|\le D(n-1,d)+D(n-1,d-2)=D(n,d),
$$

where negative-diameter [set families](../../../../../set-family.md) are empty. The equality of the numerical expressions is Pascal's identity. The base case $d=0$ has at most one member. At the boundary $d=n-1$, at most one member of each complementary pair is allowed, giving $2^{n-1}$, which equals $D(n,n-1)$ by binomial symmetry. For the remaining cases $1\le d\le n-2$, both section bounds belong to smaller-dimensional induction cases. This completes the diametric proof.

For a $t$-intersecting [set family](../../../../../set-family.md),

$$
|A\triangle B|=|A\cup B|-|A\cap B|\le n-t=d,
$$

so the theorem applies. For $d=2q$, equality is attained by all [sets](../../../../../set-split.md) of size at least $n-q$, since two such [sets](../../../../../set-split.md) intersect in at least $n-2q=t$ elements. For $d=2q+1$, take all [sets](../../../../../set-split.md) of size at least $n-q$, and also all $(n-q-1)$-sets avoiding one fixed point. Two of these smaller [sets](../../../../../set-split.md) intersect in at least $2(n-q-1)-(n-1)=t$ points; a smaller and a larger [set](../../../../../set-split.md) intersect in at least $t$; two larger [sets](../../../../../set-split.md) intersect in at least $t+1$. The size of this [set family](../../../../../set-family.md) is

$$
\sum_{i=0}^q\binom ni+\binom{n-1}q
=2\sum_{i=0}^q\binom{n-1}i,
$$

so it attains the odd bound. If $t=0$, the full power [set](../../../../../set-split.md) is admissible; if $t>n$, the only admissible [set family](../../../../../set-family.md) is empty.

**Every maximal 1-intersecting [set family](../../../../../set-family.md) attains $2^{n-1}$, for $n\ge1$.** Such a [set family](../../../../../set-family.md) is an [up-set](../../../../../up-set.md), since adding a superset preserves [set intersections](../../../../../set-intersection.md). It contains $[n]$ and omits the empty [set](../../../../../set-split.md). It contains at most one member of any complementary pair. If neither of two nonempty complements $A,A^c$ were present, maximality would give a member $B$ disjoint from $A$; upward closure would then include $A^c$, a contradiction. Thus it chooses precisely one member of each complementary pair, as in [maximal intersecting families choose one member of every complementary pair](../../../../../maximal-intersecting-families-choose-one-member-of-every-complementary-pair.md).

**Not every maximal 2-intersecting [set family](../../../../../set-family.md) attains the bound.** On four points, let $\mathcal A=\{A:\{1,2\}\subseteq A\}$. This [set family](../../../../../set-family.md) has four members and is maximal: every missing [set](../../../../../set-split.md) meets its member $\{1,2\}$ in at most one point. The sharp bound is $1+4=5$, attained by all [sets](../../../../../set-split.md) of size at least three. This proves [maximal intersection does not imply maximum size](../../../../../maximal-intersection-does-not-imply-maximum-size.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 14](../../paper-14-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
