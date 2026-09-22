<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $G=x^3e^{-x^2-y^2}$ and $a=\sqrt{3/2}$. Its [partial derivatives](../../../../partial-derivative.md) are

$$
G_x=x^2(3-2x^2)e^{-x^2-y^2},\qquad G_y=-2yx^3e^{-x^2-y^2},
$$

so both vanish at $(a,0)$ and $(-a,0)$. Evaluating the second derivatives at a point $(x,0)$ with $x^2=3/2$ gives

$$
G_{xx}=-6xe^{-3/2},\qquad G_{xy}=0,\qquad G_{yy}=-3xe^{-3/2}.
$$

Therefore the [Hessian determinant](../../../../hessian-determinant.md) is $18x^2e^{-3}=27e^{-3}>0$. Its two diagonal entries are negative at $x=a$ and positive at $x=-a$. Hence

$$
\boxed{\begin{aligned}
(a,0)&:\ \text{strict local maximum},&G&=\left(\frac{3}{2e}\right)^{3/2},\\
(-a,0)&:\ \text{strict local minimum},&G&=-\left(\frac{3}{2e}\right)^{3/2}.
\end{aligned}}
$$

These are also global extrema: for positive $x$, the factor $e^{-y^2}\le1$ maximizes the positive value at $y=0$, and differentiating $x^3e^{-x^2}$ fixes its positive maximum at $a$. Oddness in $x$ supplies the corresponding global minimum.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [5](../../5.md)
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
