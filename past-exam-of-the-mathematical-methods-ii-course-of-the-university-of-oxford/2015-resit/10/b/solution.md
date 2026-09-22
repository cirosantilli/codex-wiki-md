<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write the fixed point as $\mathbf a=(a_1,a_2,a_3)$ and the variable point as $\mathbf r=(x_1,x_2,x_3)$. Then $\mathbf R=\mathbf r-\mathbf a$ and

$$
R=\left[\sum_{j=1}^3(x_j-a_j)^2\right]^{1/2}.
$$

Since the fixed point is not on the surface, $R>0$ at every point being considered. Componentwise differentiation gives $\partial R/\partial x_j=(x_j-a_j)/R$, hence

$$
\boxed{\nabla R=\frac{\mathbf R}{R},\qquad|\nabla R|=1}.
$$

Thus the [gradient](../../../../gradient.md) points from the fixed point towards the variable point and is a [unit vector](../../../../unit-vector.md). Keeping the fixed point fixed is important: differentiating a distance between two simultaneously moving points would include both endpoint derivatives.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2015 resit](../../../2015-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
