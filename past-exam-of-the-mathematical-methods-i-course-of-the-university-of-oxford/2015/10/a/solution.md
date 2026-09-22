<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the remaining distance calculation with $b=c$, every point on the line is $a+tb$. The nearest point to $p$ is found by [orthogonal projection](../../../../orthogonal-projection.md) onto $b$:

$$
t_* =\frac{(p-a)\cdot b}{|b|^2},\qquad
\boxed{d(p,S)=\left|(p-a)-\frac{(p-a)\cdot b}{|b|^2}b\right|=\frac{|(p-a)\times b|}{|b|}.}
$$

Indeed, differentiating $|a+tb-p|^2$ sets its component along $b$ to zero. Its second derivative is $2|b|^2>0$, proving this is the minimum.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the mathematical methods I course of the University of Oxford](../../../split.md)
5. [Mathematical methods I course of the University of Oxford](../../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
