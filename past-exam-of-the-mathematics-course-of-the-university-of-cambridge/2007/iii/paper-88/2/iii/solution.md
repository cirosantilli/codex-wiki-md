<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Fix $C$ and write $m=|A|$. Choose the permitted [prime](../../../../../../prime-number.md) $N$ with $Cm<N<2Cm$. Part (ii) gives a [subset](../../../../../../subset.md) $A'$ of size at least $m/2$ and its [cyclic group](../../../../../../cyclic-group.md) model $B\subseteq\mathbb Z_N$. Thus

$$
\frac{|B|}{N}>\frac1{4C}.
$$

To apply the interval form of [Roth theorem on three-term arithmetic progressions](../../../../../../roth-theorem-on-three-term-arithmetic-progressions.md), represent $B$ in $\{0,\ldots,N-1\}$ and split this interval into two consecutive intervals of length at most $\lceil N/2\rceil$. One has at least $|B|/2\geq m/4$ points. After translation, this is an [integer](../../../../../../integer.md) [subset](../../../../../../subset.md) $B_0$ of an interval of length at most $Cm+1$ and [subset density](../../../../../../density-of-a-finite-subset.md) bounded below in terms of $C$ only. Pad the interval to length $L=\lceil N/2\rceil$ if necessary. If $B_0$ had no nonconstant three-term [arithmetic progression](../../../../../../arithmetic-progression.md), part (i) would give

$$
\frac m4\leq|B_0|\leq\frac{C_0L}{\log\log L}\leq\frac{C_0(Cm+1)}{\log\log L}.
$$

Since $L\to\infty$ with $m$, this is impossible once $m$ is sufficiently large depending only on $C$.

Thus $B$ contains distinct elements $b_1,b_2,b_3$ with $b_1+b_3=2b_2$ modulo $N$. Their distinct preimages $a_1,a_2,a_3\in A'$ satisfy $a_1+a_3=2a_2$ in the [integers](../../../../../../integer.md) by the [Freiman 2-isomorphism](../../../../../../freiman-2-isomorphism.md). Reordering the endpoints if necessary gives

$$
\boxed{a_1,a_2,a_3\text{ form a nonconstant three-term arithmetic progression in }A.}
$$

The required size threshold depends on the fixed constant $C$; it is not a claim uniform in an arbitrarily growing $C$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 88](../../../paper-88-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
