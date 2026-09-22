<h1 id="6/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For fixed frequency $\omega$, the [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) gives $\widehat{u_{xx}}=-\omega^2\widehat u$. The transformed [initial value problem](../../../../../initial-value-problem.md) is therefore

$$
\partial_t\widehat u(t,\omega)=-\omega^2\widehat u(t,\omega),\qquad
\widehat u(0,\omega)=\widehat T(\omega).
$$

Solving this scalar [ordinary differential equation](../../../../../ordinary-differential-equation.md) yields

$$
\boxed{\widehat u(t,\omega)=e^{-t\omega^2}\widehat T(\omega)
=2e^{-t\omega^2}\frac{\sin^2\omega}{\omega^2},}
$$

where the value at $\omega=0$ is interpreted by continuity and equals two. Thus diffusion suppresses high frequencies by the Gaussian multiplier while preserving the zero-frequency mass.

The differentiation and transform steps are justified for the [heat kernel](../../../../../heat-kernel.md) solution $u=q_t*T$: for positive time its spatial derivatives are integrable, since Gaussian derivatives are integrable and $T$ is bounded with compact support. Alternatively, the transformed calculation first suggests the formula, and the next part verifies the resulting solution directly.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [6](../../../6.md)
4. [2014](../../../../2014-split.md)
5. [Past exam of the algebra 1 and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra 1 and differential equations 1 course of the University of Oxford](../../../../../algebra-1-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
