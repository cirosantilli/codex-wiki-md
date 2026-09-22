<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [Steiner system](../../../../../../steiner-system.md) $S(l,m,n)$ is an $n$-point set together with $m$-element blocks such that every $l$-element subset is contained in exactly one block. On $X=H\cup H'$, define the following six-element blocks using the incidence extensions of $\Theta$.

Take the two blocks $H$ and $H'$. For each [duad](../../../../../../duad.md) $d$ of $H$ and each [duad](../../../../../../duad.md) $d'$ in the [syntheme](../../../../../../syntheme.md) $\Theta(d)$, take

$$
B(d,d')=d\cup(H'\setminus d'),\qquad
X\setminus B(d,d')=(H\setminus d)\cup d'.
$$

These give forty-five blocks of type $(2,4)$ and forty-five of type $(4,2)$. Finally, for every corresponding partition pair $A\mid A^c$ and $B\mid B^c$, take all four unions

$$
A\cup B,\quad A\cup B^c,\quad A^c\cup B,\quad A^c\cup B^c.
$$

There are ten partition pairs and forty blocks of type $(3,3)$. Distinct indexing data give distinct blocks within each family, and different types have different intersection sizes with $H$. Thus the total is

$$
\boxed{2+45+45+40=132\text{ distinct blocks}.}
$$

To prove the defining property, fix a five-element subset $Y$ and set $r=|Y\cap H|$.

If $r=5$ or $0$, only $H$ or $H'$ can contain it. If $r=1$, write $Y\cap H=\{a\}$ and $Y\cap H'=C'$ with $|C'|=4$. A containing block must have type $(2,4)$ and its omitted [duad](../../../../../../duad.md) is $d'=H'\setminus C'$. The total $T_a$ has exactly one [syntheme](../../../../../../syntheme.md) containing $d'$; the other total containing that [syntheme](../../../../../../syntheme.md) determines a unique second point $b$. Thus the unique block is $B(\{a,b\},d')$.

If $r=4$, write $Y\cap H=C$ and $Y\cap H'=\{a'\}$. A containing block must have type $(4,2)$, with omitted [duad](../../../../../../duad.md) $d=H\setminus C$. Exactly one [duad](../../../../../../duad.md) $d'\in\Theta(d)$ contains $a'$, so $(H\setminus d)\cup d'$ is the unique block.

If $r=2$, write $Y\cap H=d$ and $Y\cap H'=C'$, where $|C'|=3$. There are only two possible types. A $(2,4)$ block exists exactly when the matching $\Theta(d)$ has a [duad](../../../../../../duad.md) contained in $H'\setminus C'$. There is then exactly one such [duad](../../../../../../duad.md), since two disjoint [duads](../../../../../../duad.md) cannot fit inside a triple. For a perfect matching on two triples, either all three pairs are cross, or there is one internal pair in each triple and one cross pair. Thus a $(2,4)$ block exists precisely when $\Theta(d)$ is not entirely cross for $C'\mid(H'\setminus C')$.

On the other hand, a $(3,3)$ block containing $Y$ must use the unique partition of $H$ corresponding to $C'\mid(H'\setminus C')$. It exists precisely when $d$ is contained in one of that partition's triples, and is then unique. By the partition incidence rule in part (b), this happens precisely when $\Theta(d)$ is entirely cross. Hence exactly one of the two possible block types exists, always uniquely.

For $r=3$, interchange the roles of $H$ and $H'$ and use the inverse partition incidence rule proved in part (b). More explicitly, the [duad](../../../../../../duad.md) $Y\cap H'$ either has an inverse [syntheme](../../../../../../syntheme.md) with an internal pair in the complement of the triple $Y\cap H$, yielding a unique $(4,2)$ block, or its inverse [syntheme](../../../../../../syntheme.md) is entirely cross, yielding the unique $(3,3)$ block. These alternatives are exclusive and exhaustive for the same matching-on-two-triples reason.

Every split $r=0,\ldots,5$ therefore gives exactly one containing block. We have constructed

$$
\boxed{S(5,6,12),\text{ the small Witt design}.}
$$

As an independent count, each block contains six five-subsets and $132\cdot6=792=\binom{12}{5}$. The case proof establishes uniqueness and existence; the count alone would not have done so.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
