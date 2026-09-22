<h1 id="6f/solution">Solution</h1>

↑ **Parent:** [6F](../6f.md)

For a [linear map](../../../../../linear-map.md) $T:U\to V$, its [rank of a linear map](../../../../../rank-of-a-linear-map.md) is $\dim\operatorname{im}T$, and its [nullity](../../../../../nullity-of-a-linear-map.md) is $\dim\ker T$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) states $\dim U=\operatorname{rank}T+\operatorname{nullity}T$. One obtains it by extending a [basis](../../../../../basis.md) of the kernel to a [basis](../../../../../basis.md) of $U$; the images of the added vectors form a [basis](../../../../../basis.md) of the image.

Restrict $\beta$ to $A=\operatorname{im}\alpha$. Its image is $\operatorname{im}(\beta\alpha)$ and its kernel is $A\cap\ker\beta$. Thus

$$
\operatorname{rank}(\beta\alpha)=\operatorname{rank}\alpha-\dim(A\cap\ker\beta).
$$

The intersection dimension is at most $\dim\ker\beta=\dim V-\operatorname{rank}\beta$, proving the lower bound. It is nonnegative, proving the upper bound by $\operatorname{rank}\alpha$, while $\operatorname{im}(\beta\alpha)\subseteq\operatorname{im}\beta$ proves the other upper bound. Consequently the [rank inequality for a composition](../../../../../rank-inequality-for-a-composition.md) is

$$
\boxed{\operatorname{rank}\alpha+\operatorname{rank}\beta-\dim V\le\operatorname{rank}(\beta\alpha)\le\min(\operatorname{rank}\alpha,\operatorname{rank}\beta).}
$$

## ↑ Ancestors (10)

1. [6F](../6f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
