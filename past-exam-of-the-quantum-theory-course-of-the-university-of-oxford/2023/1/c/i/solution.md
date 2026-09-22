<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $\tau=t-T$ and retain the [global phase](../../../../../global-phase.md) from the preceding [Lüders rule](../../../../../luders-rule.md) update. Since $P\phi_n=(\hbar n/R)\phi_n$, the same [orthonormal basis](../../../../../orthonormal-basis.md) diagonalizes the new [Hamiltonian operator](../../../../../hamiltonian-quantum-mechanics.md), with

$$
H_{\mathrm{new}}=\frac{(P-ms)^2}{2m},\qquad
\widetilde E_n=\frac1{2m}\left(\frac{\hbar n}{R}-ms\right)^2.
$$

In particular, $\widetilde E_{\pm2}=E_\star+ms^2/2\mp2\hbar s/R$. Applying [unitary time evolution](../../../../../unitary-time-evolution.md) from $T$ therefore gives

$$
\boxed{\begin{aligned}
\Psi(t,x)&=-\frac{e^{-iE_\star T/\hbar}}{\sqrt2}
\left(e^{-i\widetilde E_2\tau/\hbar}\phi_2(x)+e^{-i\widetilde E_{-2}\tau/\hbar}\phi_{-2}(x)\right)\\
&=-\frac{e^{-iE_\star T/\hbar}e^{-i(E_\star+ms^2/2)\tau/\hbar}}{\sqrt{\pi R}}
\cos\!\left(\frac{2(x+s\tau)}R\right).
\end{aligned}}
$$

This is [rigid translation from a momentum term in the Hamiltonian](../../../../../rigid-translation-from-a-momentum-term-in-the-hamiltonian.md): the position [probability density](../../../../../probability-density.md) moves with velocity $-s$. The plus sign in $x+s\tau$ follows directly from the negative sign of $-sP$. At $\tau=0$ the expression agrees exactly with the preceding [post-measurement state](../../../../../post-measurement-state.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the quantum theory course of the University of Oxford](../../../../split.md)
6. [Quantum theory course of the University of Oxford](../../../../../quantum-theory-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
