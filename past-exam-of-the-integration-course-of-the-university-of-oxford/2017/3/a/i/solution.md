<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A sufficient theorem is [dominated differentiation under the integral sign](../../../../../dominated-differentiation-under-the-integral-sign.md). Let $t_0$ be interior to a parameter interval, suppose $u(\cdot,t)$ is measurable for each $t$, and suppose $u(\cdot,t_0)$ is integrable. Assume $u(x,\cdot)$ is differentiable near $t_0$ for $x$ outside one fixed [null set](../../../../../null-set.md), and that throughout this neighborhood

$$
|\partial_tu(x,t)|\leq H(x)
$$

for one nonnegative [Lebesgue integrable function](../../../../../lebesgue-integrable-function.md) $H$. Then $F(t)=\int_Eu(x,t)\,dx$ is defined near $t_0$, is differentiable at $t_0$, and

$$
\boxed{F'(t_0)=\int_E\partial_tu(x,t_0)\,dx.}
$$

Indeed the [mean value theorem](../../../../../mean-value-theorem.md) bounds both $|u(x,t)-u(x,t_0)|$ by $|t-t_0|H(x)$ and the difference quotient by $H(x)$. The first bound proves local integrability; the second lets the [dominated convergence theorem](../../../../../dominated-convergence-theorem.md) pass the limit of difference quotients through the integral.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the integration course of the University of Oxford](../../../../split.md)
6. [Integration course of the University of Oxford](../../../../../integration-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
