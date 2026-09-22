<h1 id="12f/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

**A [Hausdorff](../../../../../../hausdorff-space.md), noncompact [topology](../../../../../../topology-split.md).** The condition says precisely that each point of $U$ lies in a [residue class](../../../../../../residue-class.md) $n+k\mathbb Z$ contained in $U$. These classes form a basis: the intersection of two classes containing a common point contains the class through that point with modulus equal to the least common multiple of their moduli. Thus arbitrary unions obey the condition, and so do finite intersections. Also $\varnothing$ and $\mathbb Z$ obey it. This is the [profinite topology](../../../../../../profinite-topology.md) on $\mathbb Z$.

If $a\ne b$, choose $k>|a-b|$. Then $a+k\mathbb Z$ and $b+k\mathbb Z$ are disjoint open neighbourhoods, proving the [Hausdorff](../../../../../../hausdorff-space.md) property. To test [compactness](../../../../../../compact-space.md), define

$$
a_n=\frac{4^n-1}{3},\qquad F_n=a_n+4^n\mathbb Z\quad(n\geq1).
$$

Every $F_n$ is nonempty and both open and closed: its complement is a finite union of other [residue classes](../../../../../../residue-class.md). Since $a_{n+1}-a_n=4^n$, $F_{n+1}\subseteq F_n$. If $x$ belonged to their intersection, then $3x+1$ would be divisible by $4^n$ for every $n$, forcing $3x+1=0$, impossible for an integer. Therefore $U_n=\mathbb Z\setminus F_n$ is an increasing [open cover](../../../../../../open-cover.md) of $\mathbb Z$. Any finite subcollection has union $U_N$ for its largest index and misses the nonempty $F_N$. This proves that the [profinite topology on the integers is not compact](../../../../../../profinite-topology-on-the-integers-is-not-compact.md).

## ↑ Ancestors (11)

1. [D](../d.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
