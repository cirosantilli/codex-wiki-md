<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

If $x\in\operatorname{Null}(A)$, the $i$th entry of $Ax=0$ says $r_i\cdot x=0$. Any $y\in\operatorname{Row}(A)$ is a [linear combination](../../../../../linear-combination.md) $y=\sum_i\alpha_i r_i$, so bilinearity of the [dot product](../../../../../dot-product.md) gives

$$
y\cdot x=\sum_i\alpha_i(r_i\cdot x)=0.
$$

Hence

$$
\boxed{\operatorname{Row}(A)\perp\operatorname{Null}(A).}
$$

This proves the [orthogonality](../../../../../orthogonal-vectors.md) for every pair of [vectors](../../../../../vector.md) in the two [vector subspaces](../../../../../vector-subspace.md). In fact the [null space](../../../../../kernel-of-a-linear-map-split.md) equals the [orthogonal complement](../../../../../orthogonal-complement.md) of the [row space](../../../../../row-space.md), since being [orthogonal](../../../../../orthogonal-vectors.md) to every row is exactly the system $Ax=0$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Digital systems, linear algebra, introduction to formal proof](../../../digital-systems-linear-algebra-introduction-to-formal-proof-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
