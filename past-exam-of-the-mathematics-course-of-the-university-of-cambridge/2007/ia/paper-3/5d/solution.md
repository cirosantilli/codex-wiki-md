<h1 id="5d/solution">Solution</h1>

↑ **Parent:** [5D](../5d.md)

The [order of a group element](../../../../../order-of-a-group-element.md) $x$ is the least positive integer $r$ with $x^r=e$, or infinity if none exists. In a [finite group](../../../../../finite-group.md), some two powers among $e,x,\ldots,x^{|G|}$ coincide; cancellation then gives a positive power equal to $e$, so $r$ exists. The generated [cyclic group](../../../../../cyclic-group.md) $H=\langle x\rangle$ consists of the distinct elements $e,x,\ldots,x^{r-1}$ and has size $r$.

We now prove the needed divisibility directly by [cosets](../../../../../coset.md). Multiplication by $g$ bijects $H$ with the left [coset](../../../../../coset.md) $gH$, so every left [coset](../../../../../coset.md) has $r$ elements. If $gH$ and $hH$ intersect, write $ga=hb$ with $a,b\in H$. Then $h^{-1}g=ba^{-1}\in H$, which implies $gH=hH$. Thus distinct left [cosets](../../../../../coset.md) are disjoint, and every element of $G$ belongs to its own left [coset](../../../../../coset.md). The finite set $G$ is partitioned into, say, $k$ such [cosets](../../../../../coset.md). Hence $|G|=kr$ and

$$
\boxed{\operatorname{ord}(x)\mid |G|.}
$$

This supplies the counting argument underlying [Lagrange's theorem](../../../../../lagrange-s-theorem.md), rather than appealing to it or to an unproved orbit formula.

A divisor of $|G|$ need not occur as an element order. Use $G=C_2\times C_2\times C_2$, of order eight, and $d=4<8$. Every element has square equal to the identity, so there is no element of order four. Thus **the proposed converse is false, even for an abelian group**.

For the [direct product of groups](../../../../../direct-product-of-groups.md) $C_m\times C_n$, let $a,b$ generate the factors. The least $k>0$ for which $(a,b)^k=(e,e)$ is the [least common multiple](../../../../../least-common-multiple.md) of $m,n$. If $m,n$ are [coprime](../../../../../coprime-integers.md), this is $mn$, the size of the whole product, so $(a,b)$ generates every element. Conversely, for any pair $(u,v)$ its order is $\operatorname{lcm}(\operatorname{ord}u,\operatorname{ord}v)$ and divides $\operatorname{lcm}(m,n)$. If $\gcd(m,n)>1$, that bound is $mn/\gcd(m,n)<mn$, so no element can generate the product. Therefore

$$
\boxed{C_m\times C_n\text{ is cyclic exactly when }\gcd(m,n)=1.}
$$

This is the [cyclicity of a product of two finite cyclic groups](../../../../../cyclicity-of-a-product-of-two-finite-cyclic-groups.md); the general pair-order criterion is the [order of a direct-product element](../../../../../order-of-a-direct-product-element.md).

## ↑ Ancestors (10)

1. [5D](../5d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
