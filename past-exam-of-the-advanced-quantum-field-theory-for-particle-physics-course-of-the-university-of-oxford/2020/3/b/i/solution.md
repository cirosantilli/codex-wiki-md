<h1 id="3/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [gauge-invariant](../../../../../gauge-invariance.md) [path integral](../../../../../path-integral.md) counts all representatives of each [gauge orbit](../../../../../gauge-orbit.md). In a perturbative region with a regular [gauge fixing](../../../../../gauge-fixing.md) slice, insert the [Faddeev-Popov gauge-orbit identity](../../../../../faddeev-popov-gauge-orbit-identity.md)

$$
1=\Delta_{\mathrm{FP}}[A]\int\mathcal D\omega\,\delta(F[A^\omega]-\sigma),\qquad
F[A]=\partial_\mu A^\mu+\lambda A_\mu A^\mu.
$$

The [Faddeev-Popov determinant](../../../../../faddeev-popov-determinant.md) is the [functional Jacobian](../../../../../functional-jacobian.md) converting integration over the [gauge transformation](../../../../../gauge-transformation.md) parameter into integration over the condition. The redundant [gauge group](../../../../../gauge-group.md) volume then factors out of normalized [correlation functions](../../../../../correlation-function.md).

Choose $A_\mu^\omega=A_\mu+\partial_\mu\omega$. Its infinitesimal variation gives

$$
\delta F=\partial^2\omega+2\lambda A^\mu\partial_\mu\omega,\qquad
\boxed{\mathcal M(x,y)=[\partial_x^2+2\lambda A^\mu(x)\partial_{x\mu}]\delta^{(4)}(x-y),\quad\Delta_{\mathrm{FP}}[A]=\det\mathcal M.}
$$

There is no derivative of $A$ in this expression: only $A_\mu$ is varied in $A^2$. For $\lambda=0$, the determinant is field independent and can be absorbed into normalization. For $\lambda\ne0$, it is a functional of the [gauge field](../../../../../gauge-field.md), so dropping it changes the [path integral](../../../../../path-integral.md), even though the [gauge group](../../../../../gauge-group.md) is Abelian. Constant residual [gauge transformations](../../../../../gauge-transformation.md) are removed by boundary conditions or by dividing out their volume, as usual in perturbative [gauge fixing](../../../../../gauge-fixing.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2020](../../../../2020-split.md)
5. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../../split.md)
6. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Mathematical and theoretical physics course of the University of Oxford](../../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
