<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a [Lagrangian density](../../../../lagrangian-density.md) depending on $\phi$, $\partial_t\phi$, $\partial_i\phi$ and $\partial_i\partial_j\phi$, direct variation gives

$$
\delta S=\int dt\,d^3x\left[
\mathcal L_\phi\delta\phi+
\mathcal L_{\dot\phi}\partial_t\delta\phi+
\mathcal L_{\partial_i\phi}\partial_i\delta\phi+
\mathcal L_{\partial_i\partial_j\phi}\partial_i\partial_j\delta\phi\right].
$$

Take $\delta\phi$ to have compact support, so every boundary term vanishes. One [integration by parts](../../../../integration-by-parts.md) for the first-derivative terms and two for the second-derivative term yield the [Euler-Lagrange field equation with second derivatives](../../../../euler-lagrange-field-equation-with-second-derivatives.md)

$$
\mathcal L_\phi-\partial_t\mathcal L_{\dot\phi}
-\partial_i\mathcal L_{\partial_i\phi}
+\partial_i\partial_j\mathcal L_{\partial_i\partial_j\phi}=0.
$$

The plus sign on the last term is essential. For the [action](../../../../action.md) in [a](../a.md), it is particularly transparent to vary the [Laplacian](../../../../laplacian.md) directly:

$$
\delta S=\int dt\,d^3x\left[
\dot\phi\,\partial_t\delta\phi-\kappa^2\nabla^2\phi\,\nabla^2\delta\phi-m^2\phi\,\delta\phi\right]
=-\int dt\,d^3x\left[\ddot\phi+\kappa^2\nabla^4\phi+m^2\phi\right]\delta\phi.
$$

Thus the classical [equation of motion](../../../../equation-of-motion.md) is

$$
\boxed{\partial_t^2\phi+\kappa^2\nabla^4\phi+m^2\phi=0.}
$$

Here $\nabla^4=(\nabla^2)^2$ is the [biharmonic operator](../../../../biharmonic-operator.md). Substitution of the [plane wave](../../../../plane-wave.md) $\phi=Ae^{-i\omega t+i\mathbf p\cdot\mathbf x}$ gives

$$
[-\omega^2+\kappa^2|\mathbf p|^4+m^2]A=0,
\qquad
\boxed{\omega=\pm\sqrt{\kappa^2|\mathbf p|^4+m^2}.}
$$

A real classical solution combines complex-conjugate [plane waves](../../../../plane-wave.md). Quantization assigns the positive branch to the excitation [energy](../../../../energy-split.md), giving the required [dispersion relation](../../../../dispersion-relation-split.md). The negative-frequency branch supplies the [creation operator](../../../../creation-operator.md) part of the field, rather than negative excitation [energy](../../../../energy-split.md). Independently, the [Hamiltonian](../../../../hamiltonian.md) in [a](../a.md) gives $\dot\phi=\pi$, $\dot\pi=-\kappa^2\nabla^4\phi-m^2\phi$, confirming the same sign.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
