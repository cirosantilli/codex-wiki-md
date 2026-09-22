<h1 id="b/5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a fixed observation point $(\xi,\tau)$, use the backward [adjoint Green function](../../../../../adjoint-green-function.md) with $L^*=-\partial_t-\partial_x^2+1$. It satisfies $L^*G=0$ for $t<\tau$, decays with its spatial derivative as $|x|\to\infty$, and has terminal [distribution](../../../../../distribution-mathematical-analysis.md) $G(x,\tau^-;\xi,\tau)=\delta(x-\xi)$. Extending it by zero for $t>\tau$ gives $L^*G=\delta(x-\xi)\delta(t-\tau)$.

For $0<t<\tau$, [integration by parts](../../../../../integration-by-parts.md) proves

$$
\frac d{dt}\int_{\mathbb R}Gu\,dx=\int_{\mathbb R}[(-G_{xx}+G)u+G(u_{xx}-u)]\,dx=[Gu_x-G_xu]_{-\infty}^{\infty}=0.
$$

Evaluating this constant pairing at the initial and terminal times yields

$$
\boxed{u(\xi,\tau)=\int_{\mathbb R}G(x,0;\xi,\tau)f(x)\,dx.}
$$

By translating the [heat kernel with constant absorption](../../../../../heat-kernel-with-constant-absorption.md) and reversing the time difference,

$$
\boxed{G(x,t;\xi,\tau)=\frac{\exp[-(\tau-t)-(x-\xi)^2/(4(\tau-t))]}{\sqrt{4\pi(\tau-t)}},\qquad t<\tau.}
$$

The terminal singularity is understood as a [distribution](../../../../../distribution-mathematical-analysis.md); the representation follows for smooth decaying data and extends to standard integrable data by the heat-kernel approximation argument.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the differential equations and applications course of the University of Oxford](../../../../split.md)
6. [Differential equations and applications course of the University of Oxford](../../../../../differential-equations-and-applications-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
