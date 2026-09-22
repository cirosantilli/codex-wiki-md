<h1 id="32d/solution">Solution</h1>

↑ **Parent:** [32D](../32d.md)

Generalized [position eigenstates](../../../../../position-eigenstate.md) satisfy $\langle x|x'\rangle=\delta(x-x')$ and $\int|x\rangle\langle x|dx=I$. Define the position-space [wavefunction](../../../../../wave-function.md) $\psi(x)=\langle x|\psi\rangle$. Completeness then gives $\langle\psi|\psi\rangle=\int|\psi(x)|^2dx$. Position acts by multiplication, $\langle x|\widehat x|\psi\rangle=x\psi(x)$. Using $\langle x|p\rangle=(2\pi\hbar)^{-1/2}e^{ipx/\hbar}$ and [momentum](../../../../../momentum.md) completeness, differentiating the Fourier integral gives $\langle x|\widehat p|\psi\rangle=-i\hbar\psi'(x)$ on the [momentum operator](../../../../../momentum-operator.md)'s domain.

For the unit-mass, unit-frequency oscillator define

$$
a=\frac{\widehat x+i\widehat p}{\sqrt{2\hbar}},\quad a^\dagger=\frac{\widehat x-i\widehat p}{\sqrt{2\hbar}},\quad[a,a^\dagger]=1,\quad H=\hbar(a^\dagger a+1/2).
$$

Since $[H,a]=-\hbar a$, a simultaneous [energy eigenstate](../../../../../energy-eigenstate.md) and $a$-eigenstate would satisfy $[H,a]|\psi_\alpha\rangle=0=-\hbar\alpha|\psi_\alpha\rangle$, forcing $\alpha=0$. For $\alpha=0$, the energy is $\hbar/2$, the smallest possible because $\langle a^\dagger a\rangle=\|a\psi\|^2\geq0$.

The position-space equation is $(x+\hbar\partial_x)\psi_\alpha=\sqrt{2\hbar}\alpha\psi_\alpha$. Solving and normalizing, with $\alpha=u+iv$, gives up to a constant phase

$$
\boxed{\psi_\alpha(x)=(\pi\hbar)^{-1/4}\exp\left[-\frac{(x-\sqrt{2\hbar}\,u)^2}{2\hbar}+i\sqrt{\frac2\hbar}\,v x\right].}
$$

Its squared modulus is a normalized Gaussian, so every complex $\alpha$ gives a normalizable [coherent state](../../../../../coherent-state.md).

For a creation eigenstate, $(x-\hbar\partial_x)\psi=\sqrt{2\hbar}\beta\psi$ instead gives $\psi=C\exp[x^2/(2\hbar)-\sqrt{2/\hbar}\,\beta x]$. Every nonzero such function grows quadratically exponentially at infinity and fails square integrability. Hence **there are no nonzero normalizable eigenstates of $a^\dagger$**. This last symbol is $a^\dagger$ in the original PDF, although the converted TeX drops its dagger.

## ↑ Ancestors (10)

1. [32D](../32d.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
