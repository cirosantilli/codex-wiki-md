<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Euler-Lagrange equation](../../../../euler-lagrange-equation.md) for the [real scalar field](../../../../real-scalar-field.md) gives

$$
\partial_\mu\frac{\partial\mathcal L}{\partial(\partial_\mu\phi)}-\frac{\partial\mathcal L}{\partial\phi}=0
\quad\Longrightarrow\quad
\boxed{(\Box+m^2)\phi=0.}
$$

Thus the [conjugate momentum](../../../../canonical-momentum.md) and [Hamiltonian density](../../../../hamiltonian-density.md) are

$$
\boxed{\pi=\frac{\partial\mathcal L}{\partial\dot\phi}=\dot\phi,\qquad
\mathcal H=\pi\dot\phi-\mathcal L=\frac12\bigl[\pi^2+(\nabla\phi)^2+m^2\phi^2\bigr],\qquad H=\int d^3x\,\mathcal H.}
$$

The spatial [Fourier transform](../../../../fourier-transform-split.md) reduces the [Klein-Gordon equation](../../../../klein-gordon-equation.md) to $\ddot\phi_{\mathbf p}+\omega_{\mathbf p}^2\phi_{\mathbf p}=0$, with positive [frequency](../../../../frequency.md) $\omega_{\mathbf p}=\sqrt{\mathbf p^2+m^2}$. Hence a general real solution is the [mode expansion of a free field](../../../../mode-expansion-of-a-free-field.md)

$$
\boxed{\phi(t,\mathbf x)=\int\frac{d^3p}{(2\pi)^3\sqrt{2\omega_{\mathbf p}}}
\left[a_{\mathbf p}e^{-i\omega_{\mathbf p}t+i\mathbf p\cdot\mathbf x}
+a_{\mathbf p}^*e^{i\omega_{\mathbf p}t-i\mathbf p\cdot\mathbf x}\right].}
$$

The two coefficients are complex conjugates because the [field](../../../../field.md) is real. Each pair of initial data $\phi(0,\mathbf x),\pi(0,\mathbf x)$ fixes these coefficients. The normalization anticipates [canonical quantization](../../../../canonical-quantization.md) and the relativistic normalization of one-particle states.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
