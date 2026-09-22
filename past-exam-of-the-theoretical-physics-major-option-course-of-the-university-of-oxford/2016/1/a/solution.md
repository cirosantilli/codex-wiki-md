<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\beta=(k_BT)^{-1}$ and sum over all $2^{2L}$ configurations of the [Ising spins](../../../../ising-spin-variable.md). The [canonical partition function](../../../../canonical-partition-function.md) and [Helmholtz free energy](../../../../helmholtz-free-energy.md) per site are

$$
Z_L=\sum_{\{\sigma,\tau\}}e^{-\beta E(\sigma,\tau)},
\qquad \boxed{f_L=-\frac{k_BT}{2L}\log Z_L.}
$$

Both [spins](../../../../spin.md) in each cell count as sites. In particular the denominator is $2L$, rather than $L$.

The mean [spin magnetization](../../../../spin-magnetization.md) per site is the [Boltzmann distribution](../../../../boltzmann-distribution.md) average

$$
\boxed{\langle m\rangle=\frac1{2LZ_L}\sum_{\{\sigma,\tau\}}\left[\sum_{j=1}^L(\sigma_j+\tau_j)\right]e^{-\beta E}.}
$$

Equivalently introduce a uniform [magnetic field](../../../../magnetic-field-split.md) through $E_h=E-h\sum_j(\sigma_j+\tau_j)$ and differentiate:

$$
\langle m\rangle=\left.\frac1{2L\beta}\frac{\partial\log Z_L(h)}{\partial h}\right|_{h=0}.
$$

This convention absorbs the microscopic [magnetic moment](../../../../magnetic-dipole-moment.md) into $h$. Simultaneous reversal of every [spin](../../../../spin.md) leaves $E$ invariant and changes the sign of the numerator, so $\langle m\rangle=0$ at zero field for finite $L$.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
