<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The identity $\cos^2x=\tfrac12+\tfrac14e^{2ix}+\tfrac14e^{-2ix}$ gives the [momentum eigenstate](../../../../momentum-eigenstate.md) expansion

$$
\Psi(x,0)=A\sqrt{2\pi}\left(\frac12\psi_0+\frac14\psi_2+\frac14\psi_{-2}\right).
$$

Using the [orthonormal basis](../../../../orthonormal-basis.md) from part (a), the [wavefunction normalization](../../../../wavefunction-normalization.md) is

$$
1=|A|^2(2\pi)\left(\frac14+\frac1{16}+\frac1{16}\right)=|A|^2\frac{3\pi}{4}.
$$

Hence $|A|=2/\sqrt{3\pi}$. The [wavefunction normalization](../../../../wavefunction-normalization.md) leaves a [global phase](../../../../global-phase.md) free; the positive real choice used in the requested expansion gives

$$
\boxed{A=\frac2{\sqrt{3\pi}},\qquad \Psi(x,0)=\sqrt{\frac23}\left(\psi_0(x)+\frac12\psi_2(x)+\frac12\psi_{-2}(x)\right).}
$$

The two nonzero [eigenvalues](../../../../eigenvalue.md) of the [momentum operator](../../../../momentum-operator.md) have the same [energy eigenvalue](../../../../energy-eigenvalue-split.md) $E_\star=2\hbar^2/m$. Under [unitary time evolution](../../../../unitary-time-evolution.md), their coefficients acquire the same [dynamical phase](../../../../dynamical-phase.md). With $\Omega=E_\star/\hbar=2\hbar/m$,

$$
\boxed{\begin{aligned}
\Psi(x,t)&=\sqrt{\frac23}\left(\psi_0(x)+\frac{e^{-i\Omega t}}2\psi_2(x)+\frac{e^{-i\Omega t}}2\psi_{-2}(x)\right)\\
&=\frac{1+e^{-i\Omega t}\cos(2x)}{\sqrt{3\pi}}.
\end{aligned}}
$$

At $t=0$, $1+\cos(2x)=2\cos^2x$ recovers the initial [wavefunction](../../../../wave-function-split.md). Its [probability density](../../../../probability-density.md), useful below, is

$$
|\Psi(x,t)|^2=\frac{1+\cos^2(2x)+2\cos(2x)\cos(\Omega t)}{3\pi}.
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [1](../../1.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the quantum theory course of the University of Oxford](../../../split.md)
5. [Quantum theory course of the University of Oxford](../../../../quantum-theory-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
