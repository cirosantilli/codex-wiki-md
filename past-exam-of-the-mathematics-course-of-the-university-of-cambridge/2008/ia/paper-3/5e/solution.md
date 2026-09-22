<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

For a [normal subgroup](../../../../../normal-subgroup.md) $H\trianglelefteq G$, define multiplication of left [cosets](../../../../../coset.md) by

$$
\boxed{(gH)(kH)=(gk)H.}
$$

To check that this is well-defined, replace $g,k$ by $gh_1,kh_2$ with $h_1,h_2\in H$. Their product is $gh_1kh_2=gk(k^{-1}h_1k)h_2$, and normality puts $(k^{-1}h_1k)h_2$ in $H$. Thus the product [coset](../../../../../coset.md) is independent of the representatives. [Associativity](../../../../../associative-property.md) follows from multiplication in $G$, the identity is $H$, and the inverse of $gH$ is $g^{-1}H$. These operations form the [quotient group](../../../../../quotient-group.md) $G/H$.

For the unheaded finite-index conclusion, let $G$ act on the $n$ left [cosets](../../../../../coset.md) of its proper [subgroup](../../../../../subgroup.md) $H$ by $g\cdot(xH)=gxH$. This is well-defined even if $H$ is not normal: replacing $x$ by $xh$ leaves $gxH$ unchanged. The maps are bijections with inverses supplied by $g^{-1}$, and their compositions give a [group homomorphism](../../../../../group-homomorphism.md) $\varphi:G\to S_n$. Its [kernel of a group homomorphism](../../../../../kernel-of-a-group-homomorphism.md) $N$ is normal, by the calculation in part (ii).

The action is not trivial, because some $g\notin H$ sends the [coset](../../../../../coset.md) $H$ to $gH\ne H$; hence $N\ne G$. If $N$ were trivial, $\varphi$ would be [injective](../../../../../injective-function.md), implying $|G|\leq|S_n|=n!$. Under the given strict inequality this is impossible. Thus $N$ is a nontrivial proper [normal subgroup](../../../../../normal-subgroup.md), and

$$
\boxed{|G|>n!\ \Longrightarrow\ G\text{ is not simple}.}
$$

More precisely, $N=\bigcap_{x\in G}xHx^{-1}$ is the [subgroup core](../../../../../core-group-theory.md): $g$ fixes every [coset](../../../../../coset.md) if and only if $x^{-1}gx\in H$ for every $x$. This identifies the [normal subgroup](../../../../../normal-subgroup.md) produced by the [coset action](../../../../../coset-action.md).

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
