<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $a=|A|$ and $b=|B|$, so $p\geq a>b\geq1$. To cover both the unsaturated and saturated cases with the same [coefficient](../../../../../../coefficient.md) calculation, set

$$
b'=\min\{b,p+2-a\},\qquad r=a+b'-2=\min\{p,a+b-2\}.
$$

Choose $B'\subseteq B$ of size $b'$. These parameters satisfy $1\leq b'<a\leq p$ and $1\leq r\leq p$.

Assume, for a contradiction, that the restricted sumset $C$ has fewer than $r$ elements. Extend it to a [subset](../../../../../../subset.md) $D\subseteq\mathbb F_p$ of size $r-1$, and form

$$
F(x,y)=(x-y)\prod_{z\in D}(x+y-z).
$$

On $A\times B'$, this [polynomial](../../../../../../polynomial-split.md) vanishes: when $x=y$ the first factor vanishes, and when $x\ne y$ the sum belongs to $C\subseteq D$. Its total degree is $r=(a-1)+(b'-1)$. Only the leading homogeneous part $(x-y)(x+y)^{r-1}$ contributes to the [coefficient](../../../../../../coefficient.md) of $x^{a-1}y^{b'-1}$. That [coefficient](../../../../../../coefficient.md) is

$$
\binom{r-1}{a-2}-\binom{r-1}{a-1}
=(a-b')\frac{(r-1)!}{(a-1)!(b'-1)!}.
$$

The equality includes $b'=1$, with an out-of-range binomial [coefficient](../../../../../../coefficient.md) interpreted as zero. All factorial arguments are between zero and $p-1$, and $0<a-b'<p$, so this [coefficient](../../../../../../coefficient.md) is nonzero in $\mathbb F_p$. The [Combinatorial Nullstellensatz](../../../../../../combinatorial-nullstellensatz.md) applied to $A\times B'$ forces a nonzero value, contradicting the vanishing just proved. Hence the [restricted sumset bound for unequal subsets of a prime field](../../../../../../restricted-sumset-bound-for-unequal-subsets-of-a-prime-field.md) is

$$
\boxed{|C|\geq\min\{p,|A|+|B|-2\}.}
$$

The strict size inequality is used precisely in the nonzero factor $a-b'$. The argument includes $r=p$ without dividing by $p!$, so no separate saturation assumption is hidden.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
