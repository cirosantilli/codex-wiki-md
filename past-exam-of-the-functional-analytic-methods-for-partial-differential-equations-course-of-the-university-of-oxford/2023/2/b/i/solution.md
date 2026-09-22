<h1 id="2/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Interpret the paper's unspecified $\Omega$ as containing $B_1$, the domain on which the coefficients are used. Write $A(x)=(a_{ij}(x))$, a real [symmetric matrix](../../../../../symmetric-matrix.md). The [strict ellipticity](../../../../../strict-ellipticity.md) condition is pointwise positive definiteness:

$$
\boxed{\xi^TA(x)\xi>0\qquad(x\in B_1,\ \xi\in\mathbb R^n\setminus\{0\}).}
$$

The lower bound may depend on $x$. By continuity, [strict ellipticity](../../../../../strict-ellipticity.md) gives a positive lower bound on each [compact subset](../../../../../compact-space.md) of $B_1$, but does not require one bound throughout the whole open ball.

With the two-constant convention used in the next part, [uniform ellipticity](../../../../../uniformly-elliptic-operator.md) means

$$
\boxed{\lambda|\xi|^2\leq\xi^TA(x)\xi\leq\Lambda|\xi|^2
\qquad(x\in B_1,\ \xi\in\mathbb R^n),\quad0<\lambda\leq\Lambda<\infty.}
$$

Both constants are independent of $x$. Some terminology uses [uniform ellipticity](../../../../../uniformly-elliptic-operator.md) for just the lower bound and states coefficient boundedness separately; here the paper supplies both constants. The [spectral theorem](../../../../../spectral-theorem.md) for the [symmetric matrix](../../../../../symmetric-matrix.md) gives $|A(x)\xi|\leq\Lambda|\xi|$. For example, $A(x)=(1-|x|^2)I$ satisfies [strict ellipticity](../../../../../strict-ellipticity.md) in $B_1$ but has no uniform positive lower bound as $|x|\uparrow1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the functional analytic methods for partial differential equations course of the University of Oxford](../../../../split.md)
6. [Functional analytic methods for partial differential equations course of the University of Oxford](../../../../../functional-analytic-methods-for-partial-differential-equations-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
