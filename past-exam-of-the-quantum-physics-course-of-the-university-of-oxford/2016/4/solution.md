<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Use the [orthonormal](../../../orthonormal-set.md) [energy eigenstates](../../../energy-eigenstate.md) of the [infinite square well](../../../infinite-square-well.md),

$$
\phi_n(x)=\sqrt{\frac2a}\sin\frac{n\pi x}{a},\qquad E_n=n^2E_1,\qquad E_1=\frac{\pi^2\hbar^2}{2ma^2}.
$$

The identity $\sin u\cos u=\tfrac12\sin2u$ resolves the initial [wavefunction](../../../wave-function-split.md) into $\Psi(0)=(2\phi_1+\phi_2)/\sqrt5$. Each [energy eigenstate](../../../energy-eigenstate.md) acquires its own [dynamical phase](../../../dynamical-phase.md), so

$$
\boxed{\Psi(x,t_0)=\frac{2\phi_1(x)e^{-iE_1t_0/\hbar}+\phi_2(x)e^{-4iE_1t_0/\hbar}}{\sqrt5}}
$$

inside the well, and the [wavefunction](../../../wave-function-split.md) vanishes outside. The [energy](../../../energy-split.md) probabilities are $4/5$ and $1/5$ at every time. Consequently

$$
\boxed{\langle H\rangle_0=\langle H\rangle_{t_0}=\frac85E_1=\frac{4\pi^2\hbar^2}{5ma^2}.}
$$

For the left half, each diagonal [integral](../../../integral-split.md) $\int_0^{a/2}|\phi_n|^2dx$ is $1/2$, while

$$
\int_0^{a/2}\phi_1\phi_2\,dx=\frac4{3\pi}.
$$

The [interference](../../../interference-wave-propagation.md) term therefore yields

$$
\boxed{P_{\mathrm{left}}(t_0)=\frac12+\frac{16}{15\pi}\cos\frac{3E_1t_0}{\hbar}.}
$$

This [probability](../../../probability.md) lies between approximately $0.1605$ and $0.8395$, with [period](../../../period-of-a-function.md) $2\pi\hbar/(3E_1)$. A conserved [energy](../../../energy-split.md) distribution is compatible with time-dependent position probabilities because the relative [quantum phase](../../../quantum-phase.md) keeps evolving.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2016](../../2016-split.md)
3. [Past exam of the quantum physics course of the University of Oxford](../../split.md)
4. [Quantum physics course of the University of Oxford](../../../quantum-physics-course-of-the-university-of-oxford.md)
5. [Year 2 of the physics course of the University of Oxford](../../../year-2-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
