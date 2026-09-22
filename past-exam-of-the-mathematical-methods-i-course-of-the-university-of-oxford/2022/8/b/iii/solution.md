<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $\mathbf w=\mathbf a-\mathbf c$, $B=\mathbf b\cdot\mathbf b$, $D=\mathbf d\cdot\mathbf d$ and $E=\mathbf b\cdot\mathbf d$. Differentiating $|\mathbf w+\lambda\mathbf b-\mu\mathbf d|^2$ with respect to the two parameters gives

$$
B\lambda-E\mu=-\mathbf w\cdot\mathbf b,\qquad
E\lambda-D\mu=-\mathbf w\cdot\mathbf d.
$$

For nonparallel directions, $BD-E^2=|\mathbf b\times\mathbf d|^2>0$. Solving this [linear system](../../../../../system-of-linear-equations.md) yields

$$
\boxed{\lambda=\frac{(\mathbf b\cdot\mathbf d)[(\mathbf a-\mathbf c)\cdot\mathbf d]-|\mathbf d|^2[(\mathbf a-\mathbf c)\cdot\mathbf b]}{|\mathbf b|^2|\mathbf d|^2-(\mathbf b\cdot\mathbf d)^2}.}
$$

The quadratic being minimized is strictly convex in the two parameters under this nonparallel assumption, so the critical point gives the unique pair of closest points. Parallel lines do not select a unique value of $\lambda$.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [2022](../../../../2022-split.md)
5. [Past exam of the mathematical methods I course of the University of Oxford](../../../../split.md)
6. [Mathematical methods I course of the University of Oxford](../../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
