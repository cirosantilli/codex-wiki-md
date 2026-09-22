<h1 id="section-b/b8/solution">Solution</h1>

↑ **Parent:** [B8](../b8.md)

The stationary equation is

$$
-\frac{\hbar^2}{2m}\psi''-U\delta(x)\psi=E\psi.
$$

The second [derivative](../../../../../derivative.md) represents [kinetic energy](../../../../../kinetic-energy.md); the delta term is an attractive point interaction, with $U$ having dimensions [energy](../../../../../energy-split.md) times length. A jump in $\psi$ would produce a delta [derivative](../../../../../derivative.md) in $\psi''$, with no matching term in this potential, so $\psi$ is continuous. Integrating through the origin gives

$$
\psi'(0^+)-\psi'(0^-)=-\frac{2mU}{\hbar^2}\psi(0).
$$

For $E<0$ define $\kappa=\sqrt{-2mE}/\hbar$. Each side has general solution $c_+e^{\kappa x}+c_-e^{-\kappa x}$ with independent constants. Square integrability retains $Ce^{\kappa x}$ on the left and $Ce^{-\kappa x}$ on the right. The jump requires $\kappa=mU/\hbar^2$, and [wavefunction normalization](../../../../../wavefunction-normalization.md) gives

$$
\boxed{E_b=-\frac{mU^2}{2\hbar^2},\qquad
\psi_b(x)=\sqrt{\frac{mU}{\hbar^2}}\,e^{-mU|x|/\hbar^2}}.
$$

There is one [bound state](../../../../../bound-state.md) for every $U>0$.

For $E>0$ write $k=\sqrt{2mE}/\hbar$. General solutions are independent combinations of $e^{ikx}$ and $e^{-ikx}$ on each side. For incidence from the left choose $\psi_L=e^{ikx}+r e^{-ikx}$ and $\psi_R=t e^{ikx}$. Continuity gives $t=1+r$ and the jump gives $2ikr=-2(mU/\hbar^2)t$. With $g=mU/(\hbar^2k)$,

$$
r=\frac{ig}{1-ig},\qquad t=\frac1{1-ig},\qquad
\boxed{R=\frac{g^2}{1+g^2},\quad T=\frac1{1+g^2},\quad R+T=1}.
$$

The incident and transmitted velocities are equal, so squared amplitude ratios are current ratios here. At fixed positive [energy](../../../../../energy-split.md), $U\to0$ gives full transmission and increasing $U$ gives increasing reflection, approaching unity. Even an attractive point well reflects quantum waves; [energy](../../../../../energy-split.md) is conserved, and the static potential does not irreversibly capture the incident particle into its [bound state](../../../../../bound-state.md).

<a id="section-b/b8/image-original-reflection-and-transmission-curves-versus-dimensionless-attractive-well-strength-at-fixed-incident-energy"></a>
![](../../../../../past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2013/paper-1-delta-scattering.png)

**[Figure 2](#section-b/b8/image-original-reflection-and-transmission-curves-versus-dimensionless-attractive-well-strength-at-fixed-incident-energy). Original reflection and transmission curves versus dimensionless attractive-well strength at fixed incident energy**.

## ↑ Ancestors (14)

1. [B8](../b8.md)
2. [Section B](../../section-b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
