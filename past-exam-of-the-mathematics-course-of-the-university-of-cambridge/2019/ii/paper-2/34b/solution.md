<h1 id="34b/solution">Solution</h1>

↑ **Parent:** [34B](../34b.md)

For a normalized trial state $\psi$, expand it in an orthonormal basis of [energy eigenstates](../../../../../energy-eigenstate.md), $\psi=\sum_nc_n\psi_n$. The [Rayleigh quotient](../../../../../rayleigh-quotient.md) is then

$$
\langle H\rangle_\psi
=\sum_n|c_n|^2E_n\geq E_0\sum_n|c_n|^2=E_0.
$$

This is the [quantum variational principle](../../../../../quantum-variational-principle.md): minimizing the expectation of the [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md) over any trial family gives an upper bound on the [ground-state energy](../../../../../ground-state-energy.md).

Let $\psi$ be the normalized ground-state wavefunction and form the normalized dilation $\psi_\lambda(x)=\lambda^{1/2}\psi(\lambda x)$. Its kinetic and potential expectations are

$$
T(\lambda)=\lambda^2T,
\qquad
V(\lambda)=\lambda^{-n}V.
$$

The true ground state makes the energy stationary at $\lambda=1$, so

$$
0=\left.\frac d{d\lambda}\bigl(\lambda^2T+\lambda^{-n}V\bigr)\right|_{\lambda=1}
=2T-nV.
$$

Thus the [power-law quantum virial theorem](../../../../../power-law-quantum-virial-theorem.md) gives

$$
\boxed{2\langle T\rangle_0=n\langle V\rangle_0.}
$$

If $n\leq-3$ and $A>0$, the two sides have opposite signs, because $T>0$ and $V>0$. If $A<0$, the scaled energy $\lambda^2T+\lambda^{-n}V$ tends to $-\infty$ as $\lambda\to\infty$, since $-n>2$, so the Hamiltonian is not bounded below. If $A=0$, the [free particle](../../../../../free-particle.md) has no normalizable ground state. Hence there is no normalizable ground state for $n\leq-3$.

For $n=1$ take the normalized [Gaussian function](../../../../../gaussian-function.md)

$$
\psi_\alpha(x)=\left(\frac{2\alpha^2}{\pi}\right)^{1/4}e^{-\alpha^2x^2}.
$$

The [Gaussian integral](../../../../../gaussian-integral.md) gives

$$
\langle T\rangle_\alpha=\frac{\hbar^2\alpha^2}{2m},
\qquad
\langle |x|\rangle_\alpha=\frac1{\sqrt{2\pi}\alpha},
$$

and therefore

$$
E(\alpha)=\frac{\hbar^2\alpha^2}{2m}
+\frac{A}{\sqrt{2\pi}\alpha}.
$$

Its unique minimum satisfies

$$
\alpha^3=\frac{mA}{\sqrt{2\pi}\hbar^2}.
$$

At this point $\langle V\rangle=2\langle T\rangle$, consistently with the virial theorem, and the resulting variational estimate is

$$
\boxed{E_0\leq
\frac32\left(\frac{A^2\hbar^2}{2\pi m}\right)^{1/3}.}
$$

## ↑ Ancestors (10)

1. [34B](../34b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
