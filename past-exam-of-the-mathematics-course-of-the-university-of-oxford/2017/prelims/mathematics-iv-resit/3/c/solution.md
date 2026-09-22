<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [polar radius](../../../../../../polar-radius.md) $r=at\in[0,1]$ as the parameter of the [Archimedean spiral](../../../../../../archimedean-spiral.md). Its [angle](../../../../../../angle.md) in [polar coordinates](../../../../../../polar-coordinates.md) is $r/a$. The radial and angular contributions to its [arc length](../../../../../../arc-length.md) are [orthogonal](../../../../../../orthogonal-vectors.md), so

$$
aL_a=\int_0^1\sqrt{a^2+r^2}\,dr.
$$

There is no need to evaluate this [integral](../../../../../../integral-split.md). The simple bounds $r\leq\sqrt{a^2+r^2}\leq r+a$ imply

$$
\frac12\leq aL_a\leq\frac12+a.
$$

The [squeeze theorem](../../../../../../squeeze-theorem.md) therefore gives the [scaled length of an Archimedean spiral](../../../../../../scaled-length-of-an-archimedean-spiral.md):

$$
\boxed{\ell=\lim_{a\to0^+}aL_a=\frac12.}
$$

Geometrically, the radial contribution becomes negligible after multiplying the [arc length](../../../../../../arc-length.md) by $a$; the remaining contribution is the area under the [function graph](../../../../../../graph-of-a-function.md) $r\mapsto r$ on $[0,1]$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Mathematics IV resit](../../../mathematics-iv-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
