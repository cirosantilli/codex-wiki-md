<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $\Psi_3=A^3\psi_3$ and $\Theta_3=A^3\theta_3$ denote the full third-order coefficients. This notation keeps the detuning term, proportional to $A$, and the slow-time term, proportional to $A_T$, visible. Define

$$
B=J(\psi_1,\theta_2)+J(\psi_2,\theta_1).
$$

The equations at order $\epsilon^3$ are

$$
\nabla^2\Psi_3+R_c\Theta_{3x}=-A\theta_{1x},\qquad
\nabla^2\Theta_3-\Psi_{3x}=A_T\theta_1+A^3B.
$$

Equivalently, where $A\ne0$, the question's coefficients satisfy $\nabla^2\psi_3+R_c\theta_{3x}=-A^{-2}\theta_{1x}$ and $\nabla^2\theta_3-\psi_{3x}=(A_T/A^3)\theta_1+B$. Eliminate $\Theta_3$ from the full coefficients:

$$
(\nabla^4+R_c\partial_x^2)\Psi_3=-A\partial_x\nabla^2\theta_1-R_cA_T\theta_{1x}-R_cA^3\partial_xB.
$$

Use the [Fredholm solvability condition for a self-adjoint operator](../../../../../../fredholm-solvability-condition-for-a-self-adjoint-operator.md). With $\langle f,g\rangle=\int_0^1\int_0^2fg\,dx\,dz$, projection onto the critical [eigenfunction](../../../../../../eigenfunction.md) $\psi_1$ makes the left side vanish. Therefore the [Landau amplitude equation](../../../../../../landau-amplitude-equation.md) is

$$
\boxed{A_T=\alpha A-\beta A^3,\qquad
\alpha=-\frac{\langle\psi_1,\partial_x\nabla^2\theta_1\rangle}{R_c\langle\psi_1,\theta_{1x}\rangle},\qquad
\beta=\frac{\langle\psi_1,\partial_x\{J(\psi_1,\theta_2)+J(\psi_2,\theta_1)\}\rangle}{\langle\psi_1,\theta_{1x}\rangle}.}
$$

These integrals already answer the requested coefficient calculation. Evaluating them gives $\langle\psi_1,\theta_{1x}\rangle=1/4$, $\langle\psi_1,\partial_x\nabla^2\theta_1\rangle=-\pi^2/2$, and $\langle\psi_1,\partial_xB\rangle=\pi^2/32$. Hence, for the prescribed normalization,

$$
\boxed{A_T=\frac12A-\frac{\pi^2}{8}A^3.}
$$

The cubic term opposes growth, so the nonzero steady amplitudes $A=\pm2/\pi$ are [stable equilibria](../../../../../../stable-equilibrium.md) within the chosen roll phase. The conductive state $A=0$ is unstable for this positive detuning. This is [supercritical saturation of Darcy convection rolls](../../../../../../supercritical-saturation-of-darcy-convection-rolls.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [4](../../4.md)
3. [Paper 331](../../../paper-331-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
