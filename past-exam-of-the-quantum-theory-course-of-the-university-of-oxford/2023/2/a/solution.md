<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Hamiltonian operator](../../../../hamiltonian-quantum-mechanics.md) separates into two commuting one-dimensional [quantum harmonic oscillators](../../../../quantum-harmonic-oscillator-split.md). Write

$$
\xi_j=\sqrt{\frac{m\omega_j}{\hbar}}x_j,\qquad
G=e^{-(\xi_1^2+\xi_2^2)/2},\qquad E_{00}=\frac{\hbar}{2}(\omega_1+\omega_2).
$$

Products of [harmonic oscillator eigenfunctions](../../../../harmonic-oscillator-eigenfunction.md) give

$$
\psi_{n_1,n_2}\propto H_{n_1}(\xi_1)H_{n_2}(\xi_2)G,\qquad
E_{n_1,n_2}=E_{00}+\hbar(n_1\omega_1+n_2\omega_2).
$$

Here $H_n$ is the physicists' [Hermite polynomial](../../../../hermite-polynomial.md), so $H_0=1$, $H_1(u)=2u$ and $H_2(u)=4u^2-2$. The first six [energy eigenstates](../../../../energy-eigenstate.md), ordered with multiplicity, are

$$
\boxed{\begin{array}{c|c|c}
(n_1,n_2)&E_{n_1,n_2}&\psi_{n_1,n_2}\ \text{up to a nonzero constant}\\\hline
(0,0)&E_{00}&G\\
(1,0)&E_{00}+\hbar\omega_1&\xi_1G\\
(0,1)&E_{00}+\hbar\omega_2&\xi_2G\\
(2,0)&E_{00}+2\hbar\omega_1&(4\xi_1^2-2)G\\
(1,1)&E_{00}+\hbar(\omega_1+\omega_2)&\xi_1\xi_2G\\
(0,2)&E_{00}+2\hbar\omega_2&(4\xi_2^2-2)G
\end{array}}
$$

For this [two-dimensional oscillator level ordering](../../../../two-dimensional-oscillator-level-ordering.md), the excitation [energies](../../../../energy-split.md) obey

$$
0<\omega_1\leq\omega_2<2\omega_1\leq\omega_1+\omega_2\leq2\omega_2<3\omega_1.
$$

Every state with $n_1+n_2\geq3$ costs at least $3\hbar\omega_1$, so none has been missed. Equalities within the list occur when $\omega_2=\omega_1=\omega$. Then the [two-dimensional isotropic harmonic oscillator](../../../../two-dimensional-isotropic-harmonic-oscillator.md) has

$$
\boxed{E_N=\hbar\omega(N+1),\qquad g_N=N+1,\qquad N=0,1,2,\ldots.}
$$

The [quantum degeneracy](../../../../degenerate-energy-levels.md) counts $n_1=0,\ldots,N$ with $n_2=N-n_1$. The six listed states occupy three distinct [energy levels](../../../../energy-level.md), of [quantum degeneracies](../../../../degenerate-energy-levels.md) one, two and three.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
