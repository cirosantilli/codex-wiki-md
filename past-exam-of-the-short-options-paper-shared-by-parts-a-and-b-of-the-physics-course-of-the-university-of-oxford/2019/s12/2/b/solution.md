<h1 id="s12/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take an overdamped particle with [viscous drag coefficient](../../../../../viscous-drag-coefficient.md) $\gamma$, so its deterministic drift in the [harmonic potential](../../../../../harmonic-potential.md) $U=kx^2/2$ is $\dot x=-kx/\gamma$. The one-dimensional [Fokker-Planck equation](../../../../../fokker-planck-equation.md) has [probability current](../../../../../probability-current.md)

$$
J=-\frac{kx}{\gamma}p-D\frac{dp}{dx}.
$$

At thermal [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md), $J=0$ and the [Boltzmann distribution](../../../../../boltzmann-distribution.md) is $p(x)=Z^{-1}e^{-kx^2/(2k_BT)}$, with $p'/p=-kx/(k_BT)$. Inserting this into the zero-current condition gives

$$
0=kxp\left(-\frac1\gamma+\frac{D}{k_BT}\right),\qquad
\boxed{D=\frac{k_BT}{\gamma}.}
$$

The result is the [Einstein diffusion relation](../../../../../einstein-diffusion-relation.md) between [diffusion](../../../../../diffusion.md) and mobility. It assumes a bath at one [temperature](../../../../../temperature-split.md), linear drag and thermal [equilibrium](../../../../../equilibrium-point-of-a-dynamical-system.md). The same Gaussian [probability density](../../../../../probability-density.md) gives $\langle x^2\rangle=k_BT/k$, providing an independent calibration of trap stiffness.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [S12](../../../s12.md)
4. [2019](../../../../2019-split.md)
5. [Past exam of the short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../split.md)
6. [Short options paper shared by Parts A and B of the physics course of the University of Oxford](../../../../../short-options-paper-shared-by-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
