<h1 id="2d/solution">Solution</h1>

↑ **Parent:** [2D](../2d.md)

[Lagrange's theorem](../../../../../lagrange-s-theorem.md) says that for a [subgroup](../../../../../subgroup.md) $H$ of a [finite group](../../../../../finite-group.md) $G$,

$$
\boxed{|G|=[G:H]|H|,\qquad |H|\mid|G|.}
$$

To prove it, the left [cosets](../../../../../coset.md) $gH$ partition $G$. Indeed every element lies in its own [coset](../../../../../coset.md); if $gH$ and $kH$ intersect, write $gh=kh'$ and deduce $g=k h'h^{-1}$, so $gH=kH$. Multiplication by $g$ is a bijection from $H$ to $gH$, and each [coset](../../../../../coset.md) therefore has $|H|$ elements. Summing over the $[G:H]$ distinct [cosets](../../../../../coset.md) proves the formula.

For the [failure of the converse to Lagrange's theorem](../../../../../failure-of-the-converse-to-lagrange-s-theorem.md), take the [alternating group](../../../../../alternating-group.md) $A_4$, of order $4!/2=12$, and the divisor $6$. Suppose it had a [subgroup](../../../../../subgroup.md) $H$ of order six. Its index would be two. An index-two [subgroup](../../../../../subgroup.md) is normal: for $g\notin H$, both $gH$ and $Hg$ are the complement of $H$, while for $g\in H$ they are $H$. Hence $A_4/H$ would be a [group](../../../../../group-split.md) of order two.

Every three-cycle in $A_4$ has order three. Its image in the quotient has cube equal to the identity and, since the quotient has order two, must itself be the identity. Thus all three-cycles lie in $H$. There are eight of them: choose the omitted point in four ways and one of two cyclic orders on the other three points. Together with the identity this would give at least nine elements of $H$, contradicting $|H|=6$. Therefore **$A_4$ has no [subgroup](../../../../../subgroup.md) of order six, although six divides its order**.

## ↑ Ancestors (10)

1. [2D](../2d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
