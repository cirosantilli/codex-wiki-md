<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Differentiating the logarithm gives

$$
\frac d{dt}\log(\sec t+\tan t)=\frac{\sec t\tan t+\sec^2t}{\sec t+\tan t}=\sec t.
$$

The real logarithm is valid where its argument is positive; $\log|\sec t+\tan t|$ gives the same derivative on the other nonsingular intervals.

For the [first-order linear differential equation](../../../first-order-linear-differential-equation.md), an [integrating factor](../../../integrating-factor.md) on the interval containing $t=0$ is

$$
\mu(t)=\exp\left(\int3\tan t\,dt\right)=\sec^3t.
$$

Multiplying the equation by it yields $(x\sec^3t)'=\sec t$. Integration and $x(0)=2$ therefore give

$$
\boxed{x(t)=\cos^3t\left[2+\log(\sec t+\tan t)\right],\qquad-\frac\pi2<t<\frac\pi2.}
$$

The interval ends at singularities of the differential equation's coefficient $\tan t$; a finite limiting value of the expression would not remove those coefficient singularities.

## ↑ Ancestors (11)

1. [6](../6.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the mathematical methods I course of the University of Oxford](../../split.md)
4. [Mathematical methods I course of the University of Oxford](../../../mathematical-methods-i-course-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
