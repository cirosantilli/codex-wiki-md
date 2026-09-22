<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Rigid walls require zero normal [velocity](../../../../velocity.md), so $\phi_x=0$ at $x=0,L$ and $\phi_y=0$ at $y=0,b$. [Separation of variables](../../../../separation-of-variables.md) gives spatial modes $\cos(m\pi x/L)\cos(n\pi y/b)$, for nonnegative integers $m,n$. The [wave equation](../../../../wave-equation-split.md) therefore gives

$$
\boxed{\omega_{m,n}^2=\pi^2c_0^2(m^2/L^2+n^2/b^2).}
$$

The $(0,0)$ spatially constant mode has zero frequency and is not an ordinary positive-frequency [acoustic oscillation](../../../../acoustic-wave.md).

A spatially uniform boundary forcing excites the $n=0$ transverse mode. Put $\phi=X(x)\cos\omega t$. Then $X''+(\omega/c_0)^2X=0$ and $X'(L)=0$, hence $X=C\cos[\omega(L-x)/c_0]$. The condition $X'(0)=a$ fixes $C$ and gives

$$
\boxed{\phi=\frac{ac_0\cos[\omega(L-x)/c_0]}{\omega\sin(\omega L/c_0)}\cos\omega t.}
$$

Arbitrary free oscillations can be superposed. The denominator vanishes at longitudinal [resonances](../../../../resonance.md). Near them the lossless steady harmonic response ceases to be a uniformly small-amplitude approximation; [damping](../../../../damping.md) from [viscosity](../../../../dynamic-viscosity-split.md), heat transfer or wall losses regularizes the response, and large amplitudes can require nonlinear [equations of motion](../../../../equation-of-motion.md) or a more accurate moving-boundary model. At exact [resonance](../../../../resonance.md) a switched-on ideal forcing produces secular growth rather than a bounded harmonic particular solution.

For the semi-infinite duct expand $F(y)=\sum_{n\geq0}F_n\cos(n\pi y/b)$. Each axial mode has

$$
\boxed{k_n^2=\omega^2/c_0^2-(n\pi/b)^2.}
$$

For a propagating mode a particular solution is $\phi_n=(F_n/k_n)\cos(n\pi y/b)\cos(k_nx-\omega t)$; differentiating at zero gives the prescribed $F_n\cos(n\pi y/b)\sin\omega t$. A nonzero higher transverse coefficient propagates when $|\omega|>n\pi c_0/b$.

The outgoing [radiation condition](../../../../radiation-condition.md) selects $c_0^2k_n/\omega>0$, its positive axial [group velocity](../../../../group-velocity.md). Thus $\boxed{\omega k_n>0}$. This sign is selected by the absence of waves incident from infinity, not by the differential equation alone. If $F$ has a nonzero mean, its $n=0$ component can propagate even below every higher-mode cutoff.

For $F=\cos(\pi y/b)$ and $0<|\omega|<\pi c_0/b$, put $\kappa=\sqrt{(\pi/b)^2-\omega^2/c_0^2}$. The decaying solution is

$$
\boxed{\phi=-\frac1\kappa e^{-\kappa x}\cos(\pi y/b)\sin\omega t.}
$$

It is evanescent and carries no mean [energy](../../../../energy-split.md) to infinity. These mode and sign conditions are summarized by the [radiation condition for a waveguide mode](../../../../radiation-condition-for-a-waveguide-mode.md).

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the theoretical mechanics course of the University of Oxford](../../../split.md)
5. [Theoretical mechanics course of the University of Oxford](../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
