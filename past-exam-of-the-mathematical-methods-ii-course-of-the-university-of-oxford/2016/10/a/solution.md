<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Parametrize the graph by $\mathbf r(x,y)=(x,y,f(x,y))$ over its projection $D$ onto the $xy$ plane. The tangent vectors are $(1,0,f_x)$ and $(0,1,f_y)$, so their [cross product](../../../../cross-product.md) is $(-f_x,-f_y,1)$. Hence the scalar [surface element](../../../../area-element-of-a-surface.md) is

$$
dS=|\mathbf r_x\times\mathbf r_y|\,dx\,dy=\sqrt{1+f_x^2+f_y^2}\,dx\,dy,
$$

and

$$
\boxed{\operatorname{area}(S)=\iint_D\sqrt{1+f_x^2+f_y^2}\,dx\,dy.}
$$

The printed subscript $S$ is shorthand for integrating over the projected parameter region: $dx\,dy$ belongs to $D$, while the square-root factor converts projected area into actual surface area. The corresponding upward [vector surface element of a graph](../../../../vector-surface-element-of-a-graph.md) is $(-f_x,-f_y,1)\,dx\,dy$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
