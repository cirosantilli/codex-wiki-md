<h1 id="s18/2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Multiply the expression for $\psi$ by $F^*(x)$ and integrate. Cancelling the nonzero $C$ gives

$$
1=\frac{\alpha m}{\kappa\hbar^2}\int\!\int F^*(x)F(y)e^{-\kappa|x-y|}\,dx\,dy.
$$

The kernel is real and symmetric, so relabelling the integration variables puts the expression in the printed order:

$$
\boxed{\kappa=\frac{\alpha m}{\hbar^2}\int\!\int F(x)F^*(y)e^{-\kappa|x-y|}\,dx\,dy,
\qquad E=-\frac{\hbar^2\kappa^2}{2m},\quad\kappa>0.}
$$

This is the scalar consistency condition for the rank-one potential, rather than an independent [normalization](../../../../../normalization.md) equation. The double [integral](../../../../../integral-split.md) is real and nonnegative because the [Fourier transform](../../../../../fourier-transform-split.md) of $e^{-\kappa|x|}$ is $2\kappa/(q^2+\kappa^2)>0$. Thus attractive $\alpha>0$ is needed for a nontrivial solution. Under the usual integrability assumptions the corresponding free [resolvent](../../../../../resolvent-of-an-operator.md) expectation decreases with $\kappa$, giving at most one [bound state](../../../../../bound-state.md) for this rank-one attraction.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [S18](../../../s18.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
