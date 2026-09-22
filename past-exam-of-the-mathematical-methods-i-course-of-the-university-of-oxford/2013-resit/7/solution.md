<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For this [homogeneous tangent differential equation](../../../homogeneous-tangent-differential-equation.md), set $u=y/x$ on an interval not containing $x=0$. Since $y'=u+xu'$, cancellation gives $xu'=2\tan u$. Away from zeros of $\tan u$, separation and [integration](../../../integral-split.md) give

$$
\int\cot u\,du=2\int\frac{dx}{x},\qquad
\log|\sin u|=2\log|x|+C_0.
$$

Restoring a signed constant yields the compact implicit solution

$$
\boxed{\sin(y/x)=Cx^2.}
$$

A complete real branch description is

$$
\boxed{y=x\left[k\pi+(-1)^k\arcsin(Cx^2)\right],\qquad k\in\mathbb Z.}
$$

Here $C$ is real and the interval must satisfy $x\ne0$ and $|Cx^2|<1$. The strict inequality excludes points with $\cos(y/x)=0$, where the original [tangent function](../../../tangent-function.md) is undefined. Separating divided by $\tan u$, so its zeros must be checked separately: $u=k\pi$ gives $y=k\pi x$. These are exactly the $C=0$ branches already included. The branch integer is fixed on each connected solution interval; it cannot be changed arbitrarily at a regular point.

## ↑ Ancestors (11)

1. [7](../7.md)
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
