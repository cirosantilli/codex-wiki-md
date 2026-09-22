<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [c](../c.md)

On the slit [domain](../../../../domain-mathematical-analysis.md) $D$, choose the [complex argument](../../../../argument-complex-analysis.md) $\theta=\operatorname{Arg}_{(0,2\pi)}z$. The resulting [holomorphic logarithm](../../../../holomorphic-logarithm.md) is $L(z)=\log|z|+i\theta$, with $L'(z)=1/z$. Define

$$
\boxed{f(z)=\exp\bigl(\tfrac12L(z)\bigr)=\sqrt{|z|}\,e^{i\theta/2}.}
$$

It is [holomorphic](../../../../holomorphic-function-split.md) as a composition of [holomorphic functions](../../../../holomorphic-function-split.md), and $f(z)^2=e^{L(z)}=z$. At $z=-1$ the chosen [argument](../../../../argument-complex-analysis.md) is $\pi$, so $f(-1)=i$.

Suppose a [holomorphic square root](../../../../holomorphic-square-root.md) $g$ existed on the whole [punctured complex plane](../../../../punctured-complex-plane.md). It would be nonzero, and differentiating $g^2=z$ would give $2gg'=1$. There are several ways to express the resulting obstruction; a direct one uses the [unit circle](../../../../complex-unit-circle.md). Set

$$
q(t)=e^{-it/2}g(e^{it}),\qquad 0\leq t\leq2\pi.
$$

The [chain rule](../../../../chain-rule.md) and $g'(z)=g(z)/(2z)$ imply $q'(t)=0$, so $q$ is constant. But

$$
q(0)=g(1),\qquad q(2\pi)=-g(1).
$$

These cannot agree because $g(1)^2=1$. Thus no such global [holomorphic square root](../../../../holomorphic-square-root.md) exists. Going once around zero changes the sign of the locally chosen root.

## ↑ Ancestors (12)

1. [c](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the metric spaces and complex analysis course of the University of Oxford](../../../split.md)
5. [Metric spaces and complex analysis course of the University of Oxford](../../../../metric-spaces-and-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
