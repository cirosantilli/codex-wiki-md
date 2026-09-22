<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The [characteristic polynomial](../../../characteristic-polynomial.md) of the homogeneous equation factors as $(r-1)(r-3)$, giving the [complementary function](../../../homogeneous-solution.md) $C_1e^x+C_2e^{3x}$. For a particular solution take $A\cos x+B\sin x$. Comparing cosine and sine coefficients gives $2A-4B=10$ and $4A+2B=0$, hence $A=1,B=-2$. Therefore

$$
y=C_1e^x+C_2e^{3x}+\cos x-2\sin x.
$$

The initial conditions imply $C_1+C_2=2$ and $C_1+3C_2=2$, so $C_1=2,C_2=0$. The required solution is

$$
\boxed{y=2e^x+\cos x-2\sin x.}
$$

It has $y(0)=3$ and $y'(0)=0$, and direct [differentiation](../../../differentiation.md) verifies $y''-4y'+3y=10\cos x$.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2013](../../2013-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
