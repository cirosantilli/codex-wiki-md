<h1 id="9h/solution">Solution</h1>

↑ **Parent:** [9H](../9h.md)

For a [linear map](../../../../../linear-map.md) $\theta:U\to V$, its [rank of a linear map](../../../../../rank-of-a-linear-map.md) is $r(\theta)=\dim\operatorname{im}\theta$, and its [nullity](../../../../../nullity-of-a-linear-map.md) is $n(\theta)=\dim\ker\theta$. Choose a [basis](../../../../../basis.md) $e_1,\ldots,e_s$ of its [kernel](../../../../../kernel-of-a-linear-map.md) and extend it to a [basis](../../../../../basis.md) $e_1,\ldots,e_d$ of $U$. Then $\theta e_{s+1},\ldots,\theta e_d$ span its image. They are linearly independent: a linear combination mapped to zero would belong to the [kernel](../../../../../kernel-of-a-linear-map.md), contradicting independence of the extended [basis](../../../../../basis.md) unless all its coefficients vanish. Hence $r(\theta)=d-s$, proving

$$
\boxed{r(\theta)+n(\theta)=\dim U.}
$$

For [endomorphisms](../../../../../endomorphism.md) of $U$, define $(\theta+\phi)(u)=\theta(u)+\phi(u)$ and $(\theta\phi)(u)=\theta(\phi(u))$. The image of the sum lies in the sum of the two images. Thus

$$
r(\theta+\phi)\le\dim(\operatorname{im}\theta+\operatorname{im}\phi)
\le r(\theta)+r(\phi).
$$

To prove the product inequality, restrict $\phi$ to $K=\ker(\theta\phi)$. This map has [kernel](../../../../../kernel-of-a-linear-map.md) $\ker\phi$ and image $\operatorname{im}\phi\cap\ker\theta$: every vector in the intersection has a preimage in $K$. Applying the [rank-nullity theorem](../../../../../rank-nullity-theorem.md) to the restricted map gives

$$
n(\theta\phi)=n(\phi)+\dim(\operatorname{im}\phi\cap\ker\theta)
\le n(\phi)+n(\theta).
$$

Now put $d=\dim U$ and $s=r(\theta)+r(\phi)$. If both equalities hold, $r(\theta+\phi)=s\le d$, while $n(\theta\phi)=2d-s\le d$ forces $s\ge d$. Therefore $s=d$, the sum has full [rank](../../../../../rank-one-quadratic-form.md), and the product has [nullity](../../../../../nullity-of-a-linear-map.md) $d$. The sum is an [isomorphism](../../../../../isomorphism.md) and the product is zero.

Conversely, if $\theta\phi=0$, then $\operatorname{im}\phi\subseteq\ker\theta$, giving $s\le d$. If the sum is also an [isomorphism](../../../../../isomorphism.md), its [rank](../../../../../rank-one-quadratic-form.md) is $d\le s$. Thus $s=d$, and the two inequalities become equalities. This proves the [equality in the rank-sum and nullity-product inequalities](../../../../../equality-in-the-rank-sum-and-nullity-product-inequalities.md) in both directions.

## ↑ Ancestors (10)

1. [9H](../9h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
