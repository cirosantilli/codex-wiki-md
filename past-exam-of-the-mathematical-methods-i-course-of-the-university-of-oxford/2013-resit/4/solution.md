<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use [parametric equations](../../../parametric-equation.md) for the two lines,

$$
\mathbf r=\mathbf p+t\mathbf u,\quad \mathbf p=(2,3,-1),\quad\mathbf u=(2,1,2),
\qquad
\mathbf r=\mathbf q+s\mathbf v,\quad\mathbf q=(-2,-1,1),\quad\mathbf v=(1,2,1).
$$

Their [cross product](../../../cross-product.md) is $\mathbf u\times\mathbf v=(-3,0,3)\ne0$. Projection of the separation of the base points onto this common normal gives the [shortest distance between skew lines](../../../shortest-distance-between-skew-lines.md):

$$
\boxed{d=\frac{|(\mathbf q-\mathbf p)\cdot(\mathbf u\times\mathbf v)|}{|\mathbf u\times\mathbf v|}
=\frac{18}{3\sqrt2}=3\sqrt2.}
$$

This projection is a lower bound on every connecting segment because adding either line's direction leaves its normal component unchanged. It is attained: imposing perpendicularity of $\mathbf p+t\mathbf u-\mathbf q-s\mathbf v$ to both directions gives $t=2/3$ and $s=7/3$. The corresponding points are $(10/3,11/3,1/3)$ and $(1/3,11/3,10/3)$; their difference is $(3,0,-3)$, perpendicular to both lines and of length $3\sqrt2$.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2013 resit](../../2013-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
