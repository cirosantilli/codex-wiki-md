<h1 id="31b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A [Lyapunov function](../../../../../../lyapunov-function.md) for an equilibrium is a continuously differentiable function that is positive definite there and whose derivative along nonconstant trajectories is negative definite in a neighbourhood.

For $V=x^2+ky^2$, positivity requires $k>0$, and

$$
\dot V
=-2ax^2-2aky^2+2(3-k)xy
+2(x^2+y^2)(x^2+ky^2).
$$

The quartic term is negligible sufficiently close to the origin, so $V$ is a local Lyapunov function exactly when

$$
ax^2+aky^2-(3-k)xy
$$

is positive definite. Its determinant condition is

$$
4a^2k>(3-k)^2.
$$

The two roots of equality are

$$
k_{1,2}(a)=3+2a^2\mp2a\sqrt{a^2+3}
=\left(\sqrt{a^2+3}\mp a\right)^2.
$$

Therefore

$$
\boxed{
(\sqrt{a^2+3}-a)^2<k<(\sqrt{a^2+3}+a)^2
}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31B](../../31b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
