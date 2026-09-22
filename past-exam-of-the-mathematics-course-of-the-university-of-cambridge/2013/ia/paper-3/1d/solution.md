<h1 id="1d/solution">Solution</h1>

↑ **Parent:** [1D](../1d.md)

[Lagrange's theorem](../../../../../lagrange-s-theorem.md) states that for a [subgroup](../../../../../subgroup.md) $L$ of a [finite group](../../../../../finite-group.md) $G$, $|G|=[G:L]|L|$. In particular $|L|$ divides $|G|$; the equal-sized [cosets](../../../../../coset.md) partition $G$.

Apply the theorem to $H\cap K$ inside both [subgroups](../../../../../subgroup.md). Its order divides both coprime orders, so **$H\cap K=\{1\}$**. For $h\in H$ and $k\in K$, the [group commutator](../../../../../group-commutator.md) $hkh^{-1}k^{-1}$ lies in $K$ by $K$ being a [normal subgroup](../../../../../normal-subgroup.md), and in $H$ because $kh^{-1}k^{-1}\in H$. It is therefore the identity. Thus **every element of $H$ commutes with every element of $K$**.

Define $\theta:H\times K\to G$ by $\theta(h,k)=hk$. The cross-commutation just proved gives $\theta(h,k)\theta(h',k')=hh'kk'=\theta(hh',kk')$, so this is a [group homomorphism](../../../../../group-homomorphism.md) from the [direct product of groups](../../../../../direct-product-of-groups.md). The product assumption makes it surjective. If $hk=1$, then $h=k^{-1}\in H\cap K$, so both entries are the identity and the [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) is trivial. Hence

$$
\boxed{G\cong H\times K,\qquad(h,k)\longmapsto hk.}
$$

This proves the [internal direct product theorem](../../../../../internal-direct-product-theorem.md) in the present coprime-order setting, rather than merely matching the numbers of elements.

## ↑ Ancestors (10)

1. [1D](../1d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
