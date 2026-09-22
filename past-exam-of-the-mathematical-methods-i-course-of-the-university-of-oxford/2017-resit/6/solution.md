<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For nonparallel lines, $\mathbf n=\mathbf m_1\times\mathbf m_2$ is perpendicular to both direction vectors. Every displacement between the lines differs from $\mathbf a_2-\mathbf a_1$ by a vector in their span, so its component along $\mathbf n$ is fixed. Varying the two parameters cancels the component in that span. The [shortest distance between skew lines](../../../shortest-distance-between-skew-lines.md) is therefore

$$
\boxed{d=\frac{|(\mathbf a_2-\mathbf a_1)\cdot(\mathbf m_1\times\mathbf m_2)|}{|\mathbf m_1\times\mathbf m_2|}.}
$$

This also gives zero for intersecting nonparallel lines. For parallel lines the denominator vanishes and the correct separate formula is $| (\mathbf a_2-\mathbf a_1)\times\mathbf m_1|/|\mathbf m_1|$.

The given lines have vector forms

$$
\mathbf r_1=(2,3,-1)+t(2,1,2),\qquad
\mathbf r_2=(-2,-1,1)+u(1,2,1).
$$

Here $\mathbf m_1\times\mathbf m_2=(-3,0,3)$ and $\mathbf a_2-\mathbf a_1=(-4,-4,2)$. Their [scalar triple product](../../../scalar-triple-product.md) is $18$, giving

$$
\boxed{d=\frac{18}{3\sqrt2}=3\sqrt2.}
$$

As a constructive check, the closest parameters are $t=2/3$ and $u=7/3$, where the connecting vector is $(3,0,-3)$ and is perpendicular to both lines.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2017 resit](../../2017-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
