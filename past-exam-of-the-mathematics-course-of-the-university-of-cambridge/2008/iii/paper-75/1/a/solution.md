<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume $a<b$. A [Chebyshev system](../../../../../../chebyshev-system.md) of dimension $n+1$ is a family of real [continuous functions](../../../../../../continuous-function.md) $u_0,\ldots,u_n$ for which every [linear combination](../../../../../../linear-combination.md) $u=\sum_{j=0}^n c_ju_j$ with coefficients not all zero has at most $n$ distinct zeros in the interval. In particular the [functions](../../../../../../function-split.md) are [linearly independent](../../../../../../linear-independence.md): an identically zero nontrivial combination would violate that bound. Multiplicities are not counted in this definition.

For distinct points $x_0,\ldots,x_n$, form the evaluation [matrix](../../../../../../matrix.md) $A=(u_j(x_i))_{i,j=0}^n$. If its [determinant](../../../../../../determinant.md) vanished, a nonzero vector $c$ would satisfy $Ac=0$. Its associated combination would vanish at all $n+1$ points, contradicting the [Chebyshev system](../../../../../../chebyshev-system.md) property. Conversely, if the property failed, some nonzero coefficient vector would give a combination vanishing at $n+1$ distinct points. At those points $Ac=0$, so the evaluation [matrix](../../../../../../matrix.md) would be singular. We have proved the [determinant criterion for a Chebyshev system](../../../../../../determinant-criterion-for-a-chebyshev-system.md):

$$
\boxed{\Phi\text{ is a Chebyshev system}\iff
\det(u_j(x_i))_{i,j=0}^n\ne0\text{ for every set of distinct }x_i.}
$$

This is also the existence-and-uniqueness condition for interpolation from the span of the [functions](../../../../../../function-split.md): any prescribed $n+1$ data values give a uniquely solvable linear system.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 75](../../../paper-75-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
