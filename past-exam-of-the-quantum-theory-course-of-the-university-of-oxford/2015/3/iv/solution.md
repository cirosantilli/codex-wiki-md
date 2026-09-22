<h1 id="3/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The smallest [energy eigenvalue](../../../../energy-eigenvalue-split.md) in part (iii) occurs at the smallest possible [principal quantum number](../../../../principal-quantum-number.md), $N_{\rm p}=1$. Since $n,\ell\geq0$, this forces $n=0$ and $\ell=0$. Therefore $f=a_0r$, and

$$
\boxed{\psi_0(r)=a_0e^{-\alpha_0r},\qquad \alpha_0=\frac{mKZ}{\hbar^2},\qquad E_0=-\frac{mK^2Z^2}{2\hbar^2}.}
$$

For the spherically symmetric [ground state](../../../../ground-state.md), the full three-dimensional [wavefunction normalization](../../../../wavefunction-normalization.md) uses $d^3x=r^2dr\,d\Omega$. Integrating over the [solid angle](../../../../solid-angle.md) gives

$$
1=4\pi|a_0|^2\int_0^\infty r^2e^{-2\alpha_0r}\,dr.
$$

Put $R=2\alpha_0r$ and use the supplied [factorial](../../../../factorial.md) integral:

$$
\int_0^\infty r^2e^{-2\alpha_0r}\,dr=\frac1{(2\alpha_0)^3}\int_0^\infty R^2e^{-R}\,dR=\frac{2!}{8\alpha_0^3}=\frac1{4\alpha_0^3}.
$$

Thus $|a_0|^2=\alpha_0^3/\pi$. Choosing the positive [global phase](../../../../global-phase.md) convention gives

$$
\boxed{a_0=\left(\frac{\alpha_0^3}{\pi}\right)^{1/2}.}
$$

This is the [radial normalization of the hydrogen ground state](../../../../radial-normalization-of-the-hydrogen-ground-state.md) convention in which the angular factor is absorbed into the spherically symmetric function. If instead one writes $\Psi=R(r)Y_{00}$ with the normalized [spherical harmonic](../../../../spherical-harmonic.md) $Y_{00}=1/\sqrt{4\pi}$, then $R(r)=2\alpha_0^{3/2}e^{-\alpha_0r}$. Both conventions describe the same normalized three-dimensional [quantum state](../../../../quantum-state.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [3](../../3.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
