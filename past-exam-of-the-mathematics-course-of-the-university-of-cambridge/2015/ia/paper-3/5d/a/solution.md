<h1 id="5d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The identity [permutation](../../../../../../permutation.md) fixes every [multivariate polynomial](../../../../../../multivariate-polynomial.md). With permutation composition $(\sigma\tau)(i)=\sigma(\tau(i))$, substitution gives

$$
[\sigma\cdot(\tau\cdot f)](x_1,\ldots,x_n)
=f(x_{\sigma(\tau(1))},\ldots,x_{\sigma(\tau(n))})
=[(\sigma\tau)\cdot f](x_1,\ldots,x_n).
$$

Thus this is a left [variable-permutation action on polynomials](../../../../../../variable-permutation-action-on-polynomials.md). The substitution acts on variable names; using the displayed definition avoids reversing the composition order.

For the given [multivariate polynomial](../../../../../../multivariate-polynomial.md), the [group orbit](../../../../../../orbit-of-a-group-action.md) corresponds to the three partitions of four indices into two unordered pairs:

$$
\boxed{\operatorname{Orb}(f)=\{x_1x_2+x_3x_4,\ x_1x_3+x_2x_4,\ x_1x_4+x_2x_3\}.}
$$

These three [polynomials](../../../../../../polynomial-split.md) are distinct, and every pairing occurs under a [permutation](../../../../../../permutation.md). The [orbit-stabilizer theorem](../../../../../../orbit-stabilizer-theorem.md) gives

$$
\boxed{|(S_4)_f|=24/3=8.}
$$

The eight elements of the [stabiliser subgroup](../../../../../../stabilizer-subgroup.md) independently interchange the members of each pair, and may also interchange the two pairs.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5D](../../5d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
