<h1 id="6/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Choose a [normal subgroup](../../../../../../../normal-subgroup.md) $N$ of prime order $p\in\{5,7\}$ as in [ii](../ii.md), and choose a [subgroup](../../../../../../../subgroup.md) $H$ of the other prime order $q$. Their intersection is trivial by [Lagrange's theorem](../../../../../../../lagrange-s-theorem.md). Both are [cyclic groups](../../../../../../../cyclic-group.md), and [ii](../../b/ii.md) gives $|\operatorname{Aut}(N)|=p-1$.

The [image of a group homomorphism](../../../../../../../image-of-a-group-homomorphism.md) $\pi:H\to\operatorname{Aut}(N)$ from [iii](../../b/iii.md) has order dividing $q$, because its [kernel of a group homomorphism](../../../../../../../kernel-of-a-group-homomorphism.md) partitions $H$ into equally sized [cosets](../../../../../../../coset.md). Its order also divides $p-1$ by [Lagrange's theorem](../../../../../../../lagrange-s-theorem.md). But

$$
\gcd(7,4)=\gcd(5,6)=1,
$$

so $\pi$ is trivial in either case. By [iii](../../b/iii.md), $\langle N,H\rangle\cong C_p\times C_q$ has order $pq=35$ and therefore equals $G$.

If $n$ and $h$ generate $N$ and $H$, the element $(n,h)$ has order $\operatorname{lcm}(p,q)=pq=35$, since its $k$th power is the identity exactly when both $p$ and $q$ divide $k$. Thus this [direct product of groups](../../../../../../../direct-product-of-groups.md) is cyclic, and

$$
\boxed{G\cong C_{35}.}
$$

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Mathematics I](../../../../mathematics-i-split.md)
5. [Prelims](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
