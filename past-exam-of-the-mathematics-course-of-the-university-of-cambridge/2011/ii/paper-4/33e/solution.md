<h1 id="33e/solution">Solution</h1>

↑ **Parent:** [33E](../33e.md)

For charge $-e$, the required [gauge transformation](../../../../../gauge-transformation.md) of the wavefunction is

$$
\boxed{\Psi' = e^{-ief/\hbar}\Psi.}
$$

Define $D_t=\partial_t-ie\phi/\hbar$ and $\mathbf D=\nabla+ie\mathbf A/\hbar$. With the stated transformed potentials, differentiating the phase gives $D'_t\Psi'=e^{-ief/\hbar}D_t\Psi$ and $\mathbf D'\Psi'=e^{-ief/\hbar}\mathbf D\Psi$. Applying the spatial identity twice shows that both sides of the Schrödinger equation acquire the same phase, proving invariance. The magnetic field and electric field are unchanged because mixed derivatives commute.

Take $B>0$, as in the stated energy formula. In the specified gauge, the time-independent [Hamiltonian](../../../../../hamiltonian.md) is

$$
H=\frac1{2m}\left[(-i\hbar\partial_x-eBy)^2-\hbar^2\partial_y^2\right].
$$

It commutes with $-i\hbar\partial_x$, so choose simultaneous generalized eigenstates $\psi_k=e^{ikx}\chi_k(y)$ and attach $e^{-iEt/\hbar}$. The remaining equation is

$$
\left[-\frac{\hbar^2}{2m}\frac{d^2}{dy^2}+\frac{e^2B^2}{2m}\left(y-\frac{\hbar k}{eB}\right)^2\right]\chi_k=E\chi_k.
$$

It is a [harmonic oscillator](../../../../../simple-harmonic-motion.md) of frequency $\omega_c=eB/m$, centred at $y_0=\hbar k/(eB)$. Therefore the [Landau levels](../../../../../landau-level.md) are

$$
\boxed{E_n=(n+\tfrac12)\hbar\omega_c=(2n+1)\frac{\hbar eB}{2m}.}
$$

They are independent of the continuously variable $k$ on the infinite plane, giving infinite degeneracy. Plane waves may be normalized in a finite box and the infinite-area limit then taken. For signed $B$, replace the oscillator frequency by $e|B|/m$.

With $\phi=-Ey$, the additional potential energy is $+eEy$. Completing the square preserves the oscillator frequency but shifts its centre to

$$
\boxed{y_0=\frac1{eB}\left(\hbar k-\frac{mE}{B}\right).}
$$

The constant term after completing the square gives

$$
\boxed{E_{n,k}=(2n+1)\frac{\hbar eB}{2m}+eEy_0+\frac{mE^2}{2B^2}
=(2n+1)\frac{\hbar eB}{2m}+\frac{\hbar kE}{B}-\frac{mE^2}{2B^2}.}
$$

When $E\ne0$, different $k$ at fixed $n$ have different energies: the guiding-centre degeneracy of each [Landau level](../../../../../landau-level.md) is lifted. Accidental coincidences between different $n,k$ are not excluded; what disappears is the flat $k$-independent level.

## ↑ Ancestors (10)

1. [33E](../33e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2011](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
