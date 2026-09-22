<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

**Equation and boundary conditions.** The [delta potential](../../../../../delta-potential.md) has strength $V_0$ with units of [energy](../../../../../energy-split.md) times length, because the [Dirac delta function](../../../../../dirac-delta-function.md) has units of inverse length. The [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) is

$$
-\frac{\hbar^2}{2m}\psi''(x)-V_0\delta(x)\psi(x)=E\psi(x).
$$

The [wavefunction](../../../../../wave-function-split.md) is continuous at the origin. A finite jump in $\psi$ would produce a [derivative](../../../../../derivative.md) of a [Dirac delta function](../../../../../dirac-delta-function.md) in $\psi''$, with no corresponding term in this potential. A jump in $\psi'$ does produce a delta contribution and is allowed. Integrate through a symmetric interval:

$$
-\frac{\hbar^2}{2m}[\psi'(\epsilon)-\psi'(-\epsilon)]
-V_0\psi(0)=E\int_{-\epsilon}^{\epsilon}\psi(x)\,dx.
$$

For continuous finite $\psi$, the right-hand side vanishes as $\epsilon\to0$. Consequently

$$
\boxed{\psi'(0^+)-\psi'(0^-)=-\frac{2mV_0}{\hbar^2}\psi(0).}
$$

This [derivative](../../../../../derivative.md) jump is the boundary condition associated with the attractive [delta potential](../../../../../delta-potential.md).

**Unique [bound state](../../../../../bound-state.md).** For $E<0$, write $\kappa=\sqrt{-2mE}/\hbar>0$. Away from the origin, $\psi''=\kappa^2\psi$. Normalizability excludes exponentials growing at either infinity, leaving

$$
\psi(x)=\begin{cases}A e^{\kappa x},&x<0,\\B e^{-\kappa x},&x>0.\end{cases}
$$

[Continuity](../../../../../continuous-function.md) gives $A=B=C$. The [derivative](../../../../../derivative.md) jump then becomes $-2\kappa C=-2mV_0C/\hbar^2$. For a nonzero state,

$$
\kappa=\frac{mV_0}{\hbar^2},\qquad
\boxed{E=-\frac{\hbar^2\kappa^2}{2m}=-\frac{mV_0^2}{2\hbar^2}.}
$$

There is exactly one positive value of $\kappa$, so exactly one negative-energy [bound state](../../../../../bound-state.md). An odd solution would have $\psi(0)=0$; the allowed decaying exponentials would then both vanish identically. Normalize the even solution using

$$
1=2|C|^2\int_0^\infty e^{-2\kappa x}\,dx=\frac{|C|^2}{\kappa}.
$$

Choosing the overall phase real and positive gives the [bound state in a delta potential](../../../../../bound-state-in-a-delta-potential.md):

$$
\boxed{\psi_0(x)=\sqrt\kappa\,e^{-\kappa|x|},\qquad\kappa=\frac{mV_0}{\hbar^2}.}
$$

It peaks at the origin, has a downward cusp there, and decays exponentially on both sides. Its value, but not its slope, is continuous.

**Scattering amplitudes and fluxes.** For $E>0$, put $k=\sqrt{2mE}/\hbar$ and retain $\kappa=mV_0/\hbar^2$ as a strength parameter. A unit-amplitude wave incident from the left has

$$
\psi_L=e^{ikx}+r e^{-ikx},\qquad\psi_R=t e^{ikx}.
$$

[Continuity](../../../../../continuous-function.md) gives $t=1+r$. The jump condition gives

$$
ik t-ik(1-r)=-2\kappa t,\qquad ikr=-\kappa(1+r).
$$

Solving,

$$
r=-\frac{\kappa}{\kappa+ik},\qquad t=\frac{ik}{\kappa+ik}.
$$

The [probability current](../../../../../probability-current.md) of a [plane wave](../../../../../plane-wave.md) of amplitude $A$ is $\hbar k|A|^2/m$ in its propagation direction. Since the asymptotic [wavenumber](../../../../../wavenumber.md) is the same on both sides, [reflection probability](../../../../../quantum-reflection-probability.md) and [transmission probability](../../../../../transmission-probability.md) are just $|r|^2$ and $|t|^2$:

$$
\boxed{R=\frac{\kappa^2}{k^2+\kappa^2}
=\frac{mV_0^2/\hbar^2}{2E+mV_0^2/\hbar^2},\qquad
T=\frac{k^2}{k^2+\kappa^2}
=\frac{2E}{2E+mV_0^2/\hbar^2}.}
$$

They satisfy $R+T=1$, expressing conserved [probability current](../../../../../probability-current.md) in this real potential.

<a id="section-b/b6/image-the-normalized-delta-well-bound-state-and-reflection-transmission-probabilities-as-attraction-increases"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2017/paper-1-b6-delta-well.png)

**[Figure 3](#section-b/b6/image-the-normalized-delta-well-bound-state-and-reflection-transmission-probabilities-as-attraction-increases). The normalized delta-well bound state and reflection/transmission probabilities as attraction increases**.

The right-hand plot uses $\eta=\kappa/k=V_0\sqrt{m/(2E)}/\hbar$, proportional to $V_0$ at fixed incident [energy](../../../../../energy-split.md). Then $R=\eta^2/(1+\eta^2)$ rises monotonically from zero to one, while $T=1/(1+\eta^2)$ falls from one to zero; they are equal at $\eta=1$. Despite the absence of a classical forbidden barrier, an abrupt attractive interaction reflects a quantum wave. Increasing attraction strengthens the [derivative](../../../../../derivative.md) mismatch and can approach complete reflection at fixed positive [energy](../../../../../energy-split.md). At fixed $V_0$, increasing incident [energy](../../../../../energy-split.md) instead makes the well increasingly transparent. The negative-energy [bound state](../../../../../bound-state.md) and the positive-energy scattering states are different stationary solutions, not an absorptive loss channel.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
