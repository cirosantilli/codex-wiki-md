<h1 id="a/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In the position representation the [Time-dependent Schrödinger equation](../../../../time-dependent-schrodinger-equation.md) is

$$
\boxed{i\hbar\partial_t\psi=-\frac{\hbar^2}{2m}\partial_x^2\psi+V(x)\psi.}
$$

For a normalized state define [probability density](../../../../probability-density.md) and [probability current](../../../../probability-current.md) by

$$
\rho=|\psi|^2,\qquad
j=\frac{\hbar}{2mi}(\overline\psi\psi_x-\psi\overline{\psi_x})
=\frac\hbar m\operatorname{Im}(\overline\psi\psi_x).
$$

Multiplying the equation by $\overline\psi$ and its [complex conjugate](../../../../complex-conjugate.md) by $\psi$, then subtracting, cancels the real potential. The resulting identity is

$$
\partial_t|\psi|^2=\frac{i\hbar}{2m}
(\overline\psi\psi_{xx}-\psi\overline{\psi_{xx}})=-\partial_xj.
$$

Thus $\boxed{\partial_t\rho+\partial_xj=0}$. Integrating over an interval gives $d\int_b^c\rho\,dx/dt=j(b)-j(c)$: probability changes only through flux across the endpoints. This is local [conservation of quantum probability](../../../../conservation-of-quantum-probability.md).

Continuity with the zero exterior imposes zero endpoint values on the [infinite square well](../../../../infinite-square-well.md). Solving the stationary equation with these [boundary conditions](../../../../boundary-condition.md) gives

$$
\boxed{E_n=\frac{n^2\pi^2\hbar^2}{2ma^2},\qquad
\Psi_n(x)=\sqrt{\frac2a}\sin\frac{n\pi x}a,\quad n\geq1,}
$$

with zero extension outside. The [integral](../../../../integral-split.md) of $\sin^2(n\pi x/a)$ is $a/2$, which fixes the [normalization](../../../../normalization.md). The initial coefficients are $3/5$ and $4/5$, whose squared moduli sum to one. Each energy component acquires its stationary phase:

$$
\boxed{\psi(x,t)=\frac35\Psi_1(x)e^{-iE_1t/\hbar}
+\frac45\Psi_2(x)e^{-iE_2t/\hbar}.}
$$

At the midpoint, $\Psi_1=\sqrt{2/a}$, $\Psi_1'=0$, $\Psi_2=0$, $\Psi_2'=-(2\pi/a)\sqrt{2/a}$. Hence

$$
\overline\psi\psi_x=-\frac{48\pi}{25a^2}e^{-i(E_2-E_1)t/\hbar}.
$$

Taking its imaginary part proves

$$
\boxed{j(a/2,t)=\frac{48\pi\hbar}{25ma^2}
\sin\left(\frac{3\pi^2\hbar}{2ma^2}t\right),\qquad
A=\frac{48\pi\hbar}{25ma^2},\quad\omega=\frac{3\pi^2\hbar}{2ma^2}.}
$$

## ↑ Ancestors (12)

1. [1](../1.md)
2. [A](../../a.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../split.md)
5. [Quantum mechanics quantum theory and quantum computers course of the University of Oxford](../../../../quantum-mechanics-quantum-theory-and-quantum-computers-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
