<h1 id="1f/solution">Solution</h1>

↑ **Parent:** [1F](../1f.md)

Put $q=(1,1,1,1)^{\mathsf T}$ and arrange the four vectors as the columns of $A=(x-1)I+qq^{\mathsf T}$. On the one-dimensional [vector subspace](../../../../../vector-subspace.md) spanned by $q$, the [eigenvalue](../../../../../eigenvalue.md) is $x+3$. On the three-dimensional [orthogonal complement](../../../../../orthogonal-complement.md) $q^\perp=\{v:\sum_i v_i=0\}$, the [eigenvalue](../../../../../eigenvalue.md) is $x-1$. Thus

$$
\det A=(x+3)(x-1)^3,
$$

and **the vectors fail to be a basis exactly when $x=1$ or $x=-3$.**

For $x=1$, all four columns equal $q$. The [matrix rank](../../../../../matrix-rank.md) is $1$, a [basis](../../../../../basis.md) of their [span](../../../../../linear-span.md) is $\{q\}$, and an extension to a [basis](../../../../../basis.md) of $\mathbb R^4$ is

$$
\boxed{\{q,e_1,e_2,e_3\}.}
$$

The last coordinate first forces the coefficient of $q$ to vanish in any [linear dependence](../../../../../linear-dependence.md), after which the other coefficients vanish.

For $x=-3$, the [matrix rank](../../../../../matrix-rank.md) is $3$ and the [span](../../../../../linear-span.md) is exactly $q^\perp$. A [basis](../../../../../basis.md) consists of the first three original columns,

$$
\boxed{\{(-3,1,1,1),(1,-3,1,1),(1,1,-3,1)\}.}
$$

Indeed, writing them as $q-4e_i$, a vanishing linear combination has coefficient sum zero by its fourth coordinate, and then each coefficient is zero by the first three coordinates. Adjoin $q$ to extend this [basis](../../../../../basis.md) to $\mathbb R^4$, since $q\notin q^\perp$.

## ↑ Ancestors (10)

1. [1F](../1f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
