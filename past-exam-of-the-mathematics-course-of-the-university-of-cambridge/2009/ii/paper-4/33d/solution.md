<h1 id="33d/solution">Solution</h1>

↑ **Parent:** [33D](../33d.md)

For potential period $a$, a [Bloch state](../../../../../bloch-state.md) has the form $\psi_k(x)=e^{ikx}u_k(x)$, with $u_k(x+a)=u_k(x)$, or equivalently $\psi_k(x+a)=e^{ika}\psi_k(x)$. Quasimomentum is defined modulo the reciprocal-lattice vector $2\pi/a$. A [Brillouin zone](../../../../../brillouin-zone.md) is one fundamental interval for that identification, usually $[-\pi/a,\pi/a)$. Here $a=2\pi$, so it is $[-1/2,1/2)$.

For small $V_0>0$, the first free-particle degeneracy occurs at the zone edge $k=1/2$, between [plane waves](../../../../../plane-wave.md) $e^{ix/2}$ and $e^{-ix/2}$ of energy $1/4$. In this two-dimensional subspace, the diagonal [matrix](../../../../../matrix.md) elements of the potential vanish. Its [Fourier coefficient](../../../../../fourier-coefficient.md) at wave number one is $-V_0/2$; the $\cos2x$ term cannot connect these two waves at first order. Thus [degenerate perturbation theory](../../../../../degenerate-perturbation-theory.md) gives the [matrix](../../../../../matrix.md)

$$
\begin{pmatrix}1/4&-V_0/2\\-V_0/2&1/4\end{pmatrix},
$$

with energies $1/4\pm V_0/2+O(V_0^2)$. Near the edge the two uncoupled energies have opposite slopes, and diagonalization gives the avoided crossing, so the lowest [band gap](../../../../../band-gap.md) is

$$
\boxed{\Delta E=V_0+O(V_0^2),\qquad V_0\downarrow0.}
$$

For large $V_0$, expand about each deepest minimum $x=2\pi j$:

$$
-V_0(\cos x+\cos2x)=-2V_0+\frac52V_0x^2+O(V_0x^4).
$$

The local [quantum harmonic oscillator](../../../../../quantum-harmonic-oscillator.md) $-d^2/dx^2+(5V_0/2)x^2$ has levels $(2n+1)\sqrt{5V_0/2}$. Its localization width is $O(V_0^{-1/4})$, so the quartic term changes these low levels by $O(1)$. Tunnelling between successive deep wells gives exponentially narrow [energy bands](../../../../../energy-band.md). The secondary minima at $x=(2j+1)\pi$ have potential zero, and their levels lie far above the first two deep-well levels, whose energies are $-2V_0+O(\sqrt{V_0})$. Therefore the gap between the first and second bands is the first oscillator spacing to leading order:

$$
\boxed{\Delta E\sim2\sqrt{\frac{5V_0}{2}}=\sqrt{10V_0},\qquad V_0\to\infty.}
$$

The $O(1)$ anharmonic shifts and exponentially small bandwidths do not change this leading estimate.

## ↑ Ancestors (10)

1. [33D](../33d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
