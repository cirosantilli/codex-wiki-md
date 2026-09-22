<h1 id="3e/solution">Solution</h1>

↑ **Parent:** [3E](../3e.md)

The local [maximum modulus principle](../../../../../maximum-modulus-principle.md) says that if $|f|$ has a local maximum at an interior point of a connected domain, then $f$ is constant. On a small circle about the maximum, the mean-value property and

$$
|f(z_0)|\le\frac1{2\pi}\int|f(z_0+re^{it})|dt\le|f(z_0)|
$$

force equality everywhere. Equality in the triangle inequality makes the boundary values identical; Cauchy's formula then makes $f$ constant locally, and the identity theorem makes it constant on the domain.

Write $f=u+iv$. The hypothesis gives $u-v\le0$. Therefore

$$
|e^{(1+i)f(z)}|=e^{u-v}\le1,
$$

with equality at zero. The local maximum [modulus](../../../../../modulus.md) principle makes the exponential constant. [Differentiation](../../../../../differentiation.md) then gives $f'=0$, so $f$ is constant; since $f(0)=0$, it is identically zero.

## ↑ Ancestors (10)

1. [3E](../3e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
