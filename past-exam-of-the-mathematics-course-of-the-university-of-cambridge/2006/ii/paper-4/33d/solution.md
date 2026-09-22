<h1 id="33d/solution">Solution</h1>

↑ **Parent:** [33D](../33d.md)

Assume $\lambda>0$ for the attractive wells. Write $E=-\hbar^2\kappa^2/(2m)$ with $\kappa>0$. Between wells the solution is a linear combination of $e^{\kappa x}$ and $e^{-\kappa x}$. Across a well it is continuous and its derivative jumps by $-2\lambda\psi$. Free propagation by $a$ and the jump have matrices

$$
P_a=\begin{pmatrix}\cosh\kappa a&\kappa^{-1}\sinh\kappa a\\
\kappa\sinh\kappa a&\cosh\kappa a\end{pmatrix},\qquad
D=\begin{pmatrix}1&0\\-2\lambda&1\end{pmatrix}.
$$

Their product has [determinant](../../../../../determinant.md) one and [trace](../../../../../matrix-trace.md) $2[\cosh\kappa a-(\lambda/\kappa)\sinh\kappa a]$. [Bloch theorem](../../../../../bloch-s-theorem.md) $e^{\pm ika}$ therefore give the [negative-energy band of an attractive delta comb](../../../../../negative-energy-band-of-an-attractive-delta-comb.md) equation

$$
\boxed{\cos ka=\cosh\kappa a-\frac\lambda\kappa\sinh\kappa a}.
$$

Negative energies are allowed precisely where the right side lies in $[-1,1]$. A cell [wavefunction](../../../../../wave-function.md) can be written explicitly as

$$
\psi(x)=\psi(0)\frac{\sinh\kappa(a-x)+e^{ika}\sinh\kappa x}{\sinh\kappa a},\quad 0<x<a,
$$

continued by [Bloch theorem](../../../../../bloch-s-theorem.md); the band equation enforces its derivative jump.

For $\lambda a\gg1$, the isolated well has $\kappa=\lambda$ and energy $E_0=-\hbar^2\lambda^2/(2m)$. Writing $\kappa=\lambda+\delta$, the band equation gives $\delta\sim2\lambda e^{-\lambda a}\cos ka$. Hence

$$
\boxed{E(k)\simeq E_0-2t\cos ka,\qquad t=\frac{\hbar^2\lambda^2}{m}e^{-\lambda a}}.
$$

This is the nearest-neighbour [tight-binding model](../../../../../tight-binding.md). Its hopping magnitude follows independently from isolated wavefunctions $\phi_n=\sqrt\lambda e^{-\lambda|x-na|}$: the neighbouring delta well contributes $\langle\phi_0,(H-E_0)\phi_1\rangle\simeq-(\hbar^2\lambda/m)\phi_0(0)\phi_1(0)=-t$. The subtraction removes the overlap contribution of $E_0$. More distant contributions are exponentially smaller. For repulsive or absent wells, $\lambda\le0$, the quadratic form is nonnegative and there are no negative-energy bands.

## ↑ Ancestors (10)

1. [33D](../33d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
