<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [normal vector](../../../normal-vector.md) to the [plane](../../../plane.md) is $n=(3,4,12)^T$, with [Euclidean norm](../../../euclidean-norm.md) $\|n\|=\sqrt{9+16+144}=13$. For $p=(1,1,1)^T$, $n\cdot p=19$, so the [distance from a point to a plane](../../../distance-from-a-point-to-a-plane.md) is

$$
\boxed{d=\frac{|n\cdot p-26|}{\|n\|}=\frac7{13}.}
$$

To verify that this is the minimum, the displacement to the [closest point on a plane](../../../closest-point-on-a-plane.md) is parallel to $n$. Put $q=p+tn$ and require $n\cdot q=26$. This gives $t=7/169$ and

$$
q=\frac1{169}(190,197,253)^T.
$$

For every other point $r$ on the [plane](../../../plane.md), the displacement $r-q$ is orthogonal to $q-p$. The [Pythagorean theorem](../../../pythagorean-theorem.md) gives $\|r-p\|^2=\|q-p\|^2+\|r-q\|^2\geq(7/13)^2$, proving minimality.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2019](../../2019-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
