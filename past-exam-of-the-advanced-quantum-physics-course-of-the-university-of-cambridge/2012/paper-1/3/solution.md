<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a spinless particle, [minimal coupling](../../../../minimal-coupling.md) gives $H=(\mathbf p-q\mathbf A)^2/(2m)+q\phi$. Choose the [vector potential](../../../../vector-potential.md) $\mathbf A=(0,\alpha x^2/2,0)$ and $\phi=0$. Its [curl](../../../../curl.md) is $\mathbf B=\alpha x\hat{\mathbf z}$ and $[p_y,A_y]=0$, so

$$
\boxed{H=\frac1{2m}\left[p_x^2+\left(p_y-\frac{q\alpha x^2}{2}\right)^2\right].}
$$

The [translation separation in a magnetic field gradient](../../../../translation-separation-in-a-magnetic-field-gradient.md) follows from $[H,p_y]=0$: a simultaneous [energy eigenstate](../../../../energy-eigenstate.md) can be written $\Psi=L_y^{-1/2}e^{iky}\Phi_k(x)$. The [periodic boundary condition](../../../../periodic-boundary-conditions.md) requires $e^{ikL_y}=1$, hence **$k=2\pi n/L_y$**, $n\in\mathbb Z$. The remaining [Schrödinger equation](../../../../schrodinger-equation.md) is

$$
\left[-\frac{\hbar^2}{2m}\frac{d^2}{dx^2}+V_k(x)\right]\Phi_k=E_k\Phi_k,\qquad
\boxed{V_k(x)=\frac1{2m}\left(\hbar k-\frac{g x^2}{2}\right)^2,\quad g=q\alpha.}
$$

This [magnetic-gradient quartic confinement](../../../../magnetic-gradient-quartic-confinement.md) has a positive quartic coefficient for $g\ne0$. If $k/g<0$, it is a single well at zero, with $V_k(0)=\hbar^2k^2/(2m)$. Its harmonic curvature gives

$$
\omega_s=\frac{\sqrt{-\hbar gk}}m,\qquad
\Phi_0\propto e^{-x^2/(2a_s^2)},\quad\Phi_1\propto x e^{-x^2/(2a_s^2)},\quad a_s=\sqrt{\frac\hbar{m\omega_s}}.
$$

Thus the two lowest states are respectively even and odd, with one central peak or two opposite-sign lobes, and approximately $E_j=V_k(0)+(j+1/2)\hbar\omega_s$. They are not a nearly degenerate pair.

If $k/g>0$, the two minima are $x=\pm x_0$, $x_0=\sqrt{2\hbar k/g}$, with zero potential there and a central barrier $\hbar^2k^2/(2m)$. For well-separated minima the [lowest parity states of a symmetric double well](../../../../lowest-parity-states-of-a-symmetric-double-well.md) are

$$
\boxed{\Phi_0\simeq\frac{\phi_L+\phi_R}{\sqrt{2(1+s)}},\qquad
\Phi_1\simeq\frac{\phi_L-\phi_R}{\sqrt{2(1-s)}},\qquad s=\langle\phi_L|\phi_R\rangle\ll1.}
$$

Here $\phi_L,\phi_R$ are the localized ground-state Gaussians. Their even combination is the lower state; the odd combination has a node at the origin. Weak [quantum tunnelling](../../../../quantum-tunnelling.md) gives an exponentially small [double-well tunneling splitting](../../../../double-well-tunneling-splitting.md).

To obtain their common leading energy, put $x=x_0+\delta x$. Since $\hbar k=gx_0^2/2$,

$$
V_k(x_0+\delta x)=\frac{g^2x_0^2}{2m}(\delta x)^2+O((\delta x)^3),\qquad
\omega_d=\frac{|g|x_0}{m}=\frac{\sqrt{2\hbar gk}}m.
$$

The [double-well oscillator scale in a linear magnetic field](../../../../double-well-oscillator-scale-in-a-linear-magnetic-field.md) therefore gives

$$
\boxed{E_{k,0}\simeq E_{k,1}\simeq\frac{\hbar\omega_d}{2}=\frac1m\sqrt{\frac{\hbar^3q\alpha k}{2}}.}
$$

The asymptotic condition is $x_0\gg\sqrt{\hbar/(m\omega_d)}$, so the barrier separates narrow local oscillator states. It is this scale comparison that makes the source's “large” ratio meaningful.

The [signed group velocity of a magnetic-gradient doublet](../../../../signed-group-velocity-of-a-magnetic-gradient-doublet.md) follows by differentiating the band energy with respect to the conserved wavevector:

$$
\boxed{v_y=\frac1\hbar\frac{dE_k}{dk}\simeq\frac{E_k}{2\hbar k}=\frac{\hbar q\alpha}{2m\sqrt{2\hbar q\alpha k}}.}
$$

For $q\alpha>0$ the double-well branch has $k>0$ and moves along $+y$; reversing both signs reverses its velocity. To this order the two parity states have the same velocity. Corrections include local anharmonicity and the exponentially small splitting. The spinless Hamiltonian specified here has no extra [Zeeman effect](../../../../zeeman-splitting.md) term.

<a id="3/image-original-quartic-magnetic-gradient-potentials-and-numerical-lowest-even-odd-wavefunctions-for-opposite-wavevector-signs"></a>
![](../../../../past-exam-of-the-advanced-quantum-physics-course-of-the-university-of-cambridge/2012/paper-1-aqp2012-magnetic-gradient-wells.png)

**[Figure 4](#3/image-original-quartic-magnetic-gradient-potentials-and-numerical-lowest-even-odd-wavefunctions-for-opposite-wavevector-signs). Original quartic magnetic-gradient potentials and numerical lowest even/odd wavefunctions for opposite wavevector signs**. [Source](paper-1-aqp2012-magnetic-gradient-wells.py).

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2012](../../split.md)
4. [Past exam of the advanced quantum physics course of the University of Cambridge](../../../split.md)
5. [Advanced Quantum Physics course of the University of Cambridge](../../../../advanced-quantum-physics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
