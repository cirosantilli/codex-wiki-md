<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [multiplicative group of a field](../../../../multiplicative-group-of-a-field.md) is abelian, so its finite [subgroup](../../../../subgroup.md) $G$ is a [finite abelian group](../../../../finite-abelian-group.md). Let $d\mid|G|$, and suppose $H$ is a subgroup of order $d$. By [Lagrange's theorem](../../../../lagrange-s-theorem.md), the order of each $h\in H$ divides $d$, hence $h^d=1$. Thus $H$ is contained in the set of roots in $k$ of $t^d-1$.

This nonzero [polynomial](../../../../polynomial-split.md) has degree $d$, so it has at most $d$ roots. Since the $d$ distinct elements of $H$ are already roots, they comprise the whole root set. Any second subgroup $K$ of order $d$ would also consist of $d$ roots of the same polynomial, forcing $K=H$. Therefore there is at most one [subgroup](../../../../subgroup.md) of each order dividing $|G|$.

Part (c) now applies to give

$$
\boxed{G\text{ is cyclic}.}
$$

The root bound remains valid in positive [characteristic](../../../../characteristic-of-a-field.md), even if the formal [derivative](../../../../derivative.md) of $t^d-1$ vanishes: the argument counts distinct roots, so no separability assumption is needed.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the algebra 2 course of the University of Oxford](../../../split.md)
5. [Algebra 2 course of the University of Oxford](../../../../algebra-2-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
