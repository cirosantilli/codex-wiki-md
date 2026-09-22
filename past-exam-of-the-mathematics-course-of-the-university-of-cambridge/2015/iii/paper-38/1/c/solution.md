<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For minimization, the [optimization Lagrangian](../../../../../../optimization-lagrangian.md) is

$$
L=3y-z+\lambda(2x-y-z-2)+\mu(x^2+y^2-5),\qquad \lambda\geq0.
$$

Its coefficient of $z$ is $-1-\lambda<0$, so its infimum over unrestricted $z$ is $-\infty$ for every allowable [Lagrange multiplier](../../../../../../lagrange-multiplier.md). There is no finite global minimizer of the [optimization Lagrangian](../../../../../../optimization-lagrangian.md) to which the [Lagrangian sufficiency theorem](../../../../../../lagrange-sufficiency-theorem.md) could apply.

The primal [minimization problem](../../../../../../minimization-problem.md) is also unbounded: set $x=0$, $y=\sqrt5$ and $z=t\geq0$. These points are feasible, and $3y-z=3\sqrt5-t\to-\infty$. Hence

$$
\boxed{\inf(3y-z)=-\infty.}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
