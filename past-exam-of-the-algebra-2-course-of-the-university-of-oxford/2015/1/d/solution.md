<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

By the [first isomorphism theorem for rings](../../../../first-isomorphism-theorem-for-rings.md), the given surjection identifies $S$ with $R/\ker\phi$. Since $R$ is a [principal ideal domain](../../../../principal-ideal-domain.md), write $\ker\phi=(a)$.

If $a=0$, the [quotient ring](../../../../quotient-ring.md) is $R$, an [integral domain](../../../../integral-domain.md), so part (a)(ii) applies. If $a$ is a [unit](../../../../unit-in-a-ring.md), the [quotient ring](../../../../quotient-ring.md) is the [zero ring](../../../../zero-ring.md); its unique element is associate to itself by multiplication by its identity, so it too is an [associator ring](../../../../associator-ring.md).

In the remaining case, [unique factorization](../../../../unique-factorization-in-an-integral-domain.md) gives

$$
a=\varepsilon p_1^{k_1}\cdots p_r^{k_r},
$$

where $\varepsilon$ is a [unit](../../../../unit-in-a-ring.md), the $p_i$ are pairwise nonassociate [prime elements](../../../../prime-element.md), and $k_i\geq1$. The [principal ideals](../../../../principal-ideal.md) $(p_i^{k_i})$ are pairwise comaximal: different prime factors have [greatest common divisor](../../../../greatest-common-divisor.md) $1$, and [Bézout's identity](../../../../bezout-s-identity.md) gives a linear combination equal to $1$. The [Chinese remainder theorem](../../../../chinese-remainder-theorem.md) therefore gives a [ring isomorphism](../../../../ring-isomorphism.md)

$$
R/(a)\ \cong\ \prod_{i=1}^r R/(p_i^{k_i}).
$$

Every factor is an [associator ring](../../../../associator-ring.md) by part (c), and their finite [direct product of rings](../../../../direct-product-of-rings.md) is an [associator ring](../../../../associator-ring.md) by part (b). A [ring isomorphism](../../../../ring-isomorphism.md) preserves [units](../../../../unit-in-a-ring.md) and [principal ideals](../../../../principal-ideal.md), so the property transfers to $S$. Hence

$$
\boxed{S\text{ is an associator ring}.}
$$

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
