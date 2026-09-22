<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [surface area of a tricylinder](../../../../../../surface-area-of-a-tricylinder.md), permutation [symmetry](../../../../../../symmetry-physics.md) shows that each of the three [cylindrical surfaces](../../../../../../cylindrical-surface.md) contributes the same [surface area](../../../../../../surface-area.md) to the [boundary](../../../../../../boundary-of-a-set.md). On the face $x^2+y^2=1$, put $x=\cos\theta$, $y=\sin\theta$. The remaining two inequalities require

$$
z^2\leq1-y^2=\cos^2\theta,\qquad
z^2\leq1-x^2=\sin^2\theta,
$$

so $|z|\leq\min(|\sin\theta|,|\cos\theta|)$. The [surface area element](../../../../../../surface-area-element.md) on this unit [circular cylinder](../../../../../../circular-cylinder.md) is $d\theta\,dz$. There are eight congruent angular sectors, with the minimum equal to $\sin\theta$ for $0\leq\theta\leq\pi/4$. Thus the [area](../../../../../../surface-area.md) of this face is

$$
A_1=\int_0^{2\pi}2\min(|\sin\theta|,|\cos\theta|)\,d\theta
=16\int_0^{\pi/4}\sin\theta\,d\theta
=8(2-\sqrt2).
$$

Every [boundary point](../../../../../../boundary-point.md) lies on at least one of these three [cylindrical surfaces](../../../../../../cylindrical-surface.md); their pairwise intersections are [curves](../../../../../../curve.md) of zero [surface area](../../../../../../surface-area.md). Adding the three faces therefore gives

$$
\boxed{\operatorname{Area}(\partial R_2)=24(2-\sqrt2).}
$$

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [Mathematics V](../../../mathematics-v-split.md)
4. [Prelims](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
