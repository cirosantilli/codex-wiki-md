<h1 id="2f/solution">Solution</h1>

↑ **Parent:** [2F](../2f.md)

Put $I=\int_0^1f(t)\,dt$. If $I\ne0$, take the [inner product](../../../../../inner-product.md) with the [unit vector](../../../../../unit-vector.md) $u=I/\|I\|_2$. Then

$$
\|I\|_2=u\mathbin{\cdot}I=\int_0^1u\mathbin{\cdot}f(t)\,dt\leq\int_0^1\|f(t)\|_2\,dt
$$

by the [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md); the case $I=0$ is immediate. This is the [triangle inequality for a vector-valued integral](../../../../../triangle-inequality-for-a-vector-valued-integral.md).

Equality in the Euclidean argument requires $u\mathbin{\cdot}f(t)=\|f(t)\|_2$ for every $t$: the nonnegative continuous difference has integral zero. Equality in [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) then says $f(t)=\lambda(t)u$ with $\lambda(t)\geq0$. Conversely, if $f(t)=\lambda(t)v$ for one fixed $v\in\mathbb R^m$ and a continuous $\lambda\geq0$, then for **every** [norm](../../../../../norm.md),

$$
\left\|\int_0^1f\right\|=\left(\int_0^1\lambda\right)\|v\|=\int_0^1\|f(t)\|\,dt.
$$

Thus these nonnegative-ray functions, including $f\equiv0$, are exactly the required functions.

## ↑ Ancestors (10)

1. [2F](../2f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
