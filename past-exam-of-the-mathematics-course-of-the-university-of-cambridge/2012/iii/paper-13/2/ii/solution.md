<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the dense standard [affine charts](../../../../../../affine-chart-of-a-variety.md). Their product is

$$
\mathbb A^n\times\mathbb A^m\cong\mathbb A^{n+m},
$$

which is also a dense [affine chart](../../../../../../affine-chart-of-a-variety.md) of $\mathbb P^{n+m}$. The identification of these charts gives **a birational isomorphism** between the two [projective varieties](../../../../../../projective-variety.md).

To distinguish them, calculate their [divisor class groups](../../../../../../divisor-class-group.md) explicitly. Let $H\subset\mathbb P^r$ be a coordinate [hyperplane](../../../../../../hyperplane.md). Its complement is $\mathbb A^r$, whose [coordinate ring](../../../../../../coordinate-ring.md) is a [unique factorization domain](../../../../../../unique-factorization-domain.md). Any [Weil divisor](../../../../../../weil-divisor.md) on $\mathbb P^r$ restricts on this chart to a [principal Weil divisor](../../../../../../principal-weil-divisor.md); subtract that [principal Weil divisor](../../../../../../principal-weil-divisor.md) on $\mathbb P^r$, leaving a [Weil divisor](../../../../../../weil-divisor.md) supported on $H$. Thus $[H]$ generates $\operatorname{Cl}(\mathbb P^r)$. If $aH=\operatorname{div}(q)$, then $q$ has zero [Weil divisor](../../../../../../weil-divisor.md) on $\mathbb A^r$. A reduced fraction in a [unique factorization domain](../../../../../../unique-factorization-domain.md) with zero orders at every [prime Weil divisor](../../../../../../prime-weil-divisor.md) must be a [unit](../../../../../../unit-in-a-ring.md), so $q\in k^*$. It follows that $a=0$. We have proved

$$
\boxed{\operatorname{Cl}(\mathbb P^r)\cong\mathbb Z\quad(r>0).}
$$

In the product, let $H_1$ and $H_2$ be coordinate [hyperplanes](../../../../../../hyperplane.md) in the factors and put

$$
D_1=H_1\times\mathbb P^m,\qquad D_2=\mathbb P^n\times H_2.
$$

The complement of $D_1\cup D_2$ is $\mathbb A^{n+m}$, again with a [unique factorization domain](../../../../../../unique-factorization-domain.md) as its [coordinate ring](../../../../../../coordinate-ring.md). The same restriction-and-subtraction argument says that $[D_1],[D_2]$ generate the [divisor class group](../../../../../../divisor-class-group.md). If

$$
aD_1+bD_2=\operatorname{div}(q),
$$

then on that [affine chart](../../../../../../affine-chart-of-a-variety.md) $q$ has neither zeros nor poles along any [prime Weil divisor](../../../../../../prime-weil-divisor.md). [Unique factorization](../../../../../../unique-factorization-in-an-integral-domain.md) makes $q$ a [unit](../../../../../../unit-in-a-ring.md) of $k[s_1,\ldots,s_n,t_1,\ldots,t_m]$, hence a constant. It follows that $a=b=0$. Therefore

$$
\boxed{\operatorname{Cl}(\mathbb P^n\times\mathbb P^m)\cong\mathbb Z^2.}
$$

Both spaces are [smooth varieties](../../../../../../smooth-algebraic-variety.md), so their [divisor class groups](../../../../../../divisor-class-group.md) also equal their [Picard groups](../../../../../../picard-group.md). An [isomorphism](../../../../../../isomorphism.md) preserves the [divisor class group](../../../../../../divisor-class-group.md); $\mathbb Z^2$ and $\mathbb Z$ are not [isomorphic](../../../../../../isomorphism.md). Thus **the spaces are birational but not isomorphic**. The assumptions $n,m>0$ ensure that both boundary [prime Weil divisors](../../../../../../prime-weil-divisor.md) actually occur.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
