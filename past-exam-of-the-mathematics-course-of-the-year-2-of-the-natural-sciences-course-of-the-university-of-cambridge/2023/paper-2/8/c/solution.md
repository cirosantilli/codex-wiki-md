<h1 id="8/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a [normal subgroup](../../../../../normal-subgroup.md) $H$, the [quotient group](../../../../../quotient-group.md) consists of its [cosets](../../../../../coset.md) with multiplication

$$
\boxed{G/H=\{gH:g\in G\},\qquad(gH)(kH)=(gk)H.}
$$

To check that this is well-defined, replace $g,k$ by $gh_1,kh_2$ with $h_1,h_2\in H$. Their product is

$$
gh_1kh_2=gk(k^{-1}h_1k)h_2\in gkH,
$$

since normality puts $k^{-1}h_1k$ in $H$. Hence the product does not depend on representatives. [Associativity](../../../../../associative-property.md) follows from that in $G$, the [identity element](../../../../../identity-element.md) is $H=eH$, and $(gH)^{-1}=g^{-1}H$. These verify the [group axioms](../../../../../group-axioms.md).

[Lagrange's theorem](../../../../../lagrange-s-theorem.md) counts the equal-sized cosets:

$$
\boxed{|G|=|G/H|\,|H|,\qquad |H|\mid |G|.}
$$

Finally, if $|G|=p$ is [prime](../../../../../prime-number-split.md), choose $g\ne e$. Its [cyclic subgroup](../../../../../cyclic-subgroup.md) has order greater than one dividing $p$, hence equals $G$. All elements are powers of $g$, so $g^jg^k=g^{j+k}=g^kg^j$. Thus

$$
\boxed{G\cong C_p\text{ and }G\text{ is abelian}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [8](../../8.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2023](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
