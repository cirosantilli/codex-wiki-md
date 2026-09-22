<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Insert the complete [orthonormal basis](../../../../orthonormal-basis.md) of [energy eigenstates](../../../../energy-eigenstate.md) on either side of the [Boltzmann factor](../../../../boltzmann-factor.md). The [spectral theorem](../../../../spectral-theorem.md) gives

$$
e^{-\beta H}=\sum_{n=0}^{\infty}e^{-\beta\hbar\omega(n+1/2)}|n\rangle\langle n|,
\qquad
\boxed{\langle x|e^{-\beta H}|x\rangle
=\sum_{n=0}^{\infty}e^{-\beta\hbar\omega(n+1/2)}|\varphi_n(x)|^2.}
$$

At low [temperature](../../../../temperature-split.md), the gap $\hbar\omega$ suppresses excited [energy eigenstates](../../../../energy-eigenstate.md). The [harmonic oscillator eigenfunction](../../../../harmonic-oscillator-eigenfunction.md) of the [ground state](../../../../ground-state.md) is

$$
\varphi_0(x)=\left(\frac{m\omega}{\pi\hbar}\right)^{1/4}
e^{-m\omega x^2/(2\hbar)}.
$$

Therefore

$$
\langle x|e^{-\beta H}|x\rangle
\sim e^{-\beta\hbar\omega/2}|\varphi_0(x)|^2,
\qquad
\boxed{R\longrightarrow\frac{|\varphi_0(x)|^2}{|\varphi_0(0)|^2}
=e^{-m\omega x^2/\hbar}.}
$$

The common [zero-point energy](../../../../zero-point-energy.md) factor cancels. Dividing the kernel by its [trace](../../../../matrix-trace.md) would give the position [probability density](../../../../probability-density.md) of the [canonical ensemble](../../../../canonical-ensemble-split.md); at zero [temperature](../../../../temperature-split.md) this tends to $|\varphi_0(x)|^2$, whose [variance](../../../../variance-split.md) is $\hbar/(2m\omega)$. Thus zero [temperature](../../../../temperature-split.md) projects onto the [ground state](../../../../ground-state.md) and retains its quantum spread, rather than concentrating at the minimum of the classical [potential energy](../../../../potential-energy.md).

There is also a check on the first correction. With $q=\sqrt{m\omega/\hbar}\,x$, the first excited [harmonic oscillator eigenfunction](../../../../harmonic-oscillator-eigenfunction.md) satisfies $|\varphi_1(x)|^2=2q^2|\varphi_0(x)|^2$ and $\varphi_1(0)=0$. Hence the [spectral theorem](../../../../spectral-theorem.md) gives $R=e^{-q^2}[1+2q^2e^{-z}+O(e^{-2z})]$, in agreement with part (c).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [1](../../1.md)
3. [2024](../../../2024-split.md)
4. [Past exam of the advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum theory: path integrals and many-particle physics course of the University of Oxford](../../../../advanced-quantum-theory-path-integrals-and-many-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
