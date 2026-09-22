<h1 id="4/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Put $k_Z=Ze^2/(4\pi\epsilon_0)$. [Gauss's law](../../../../gauss-s-law.md) for a uniform spherical [nuclear charge distribution](../../../../nuclear-charge-distribution.md), with the [electrostatic potential](../../../../electric-potential.md) matched at $R$, gives the electronic [potential energy](../../../../potential-energy.md)

$$
V_{\rm sph}(r)=\begin{cases}
-\dfrac{k_Z}{2R}(3-r^2/R^2),&r<R,\\
-k_Z/r,&r\geq R.
\end{cases}
$$

Subtracting the point-nucleus [Coulomb potential](../../../../coulomb-potential-energy.md) leaves the nonnegative perturbation

$$
\delta V(r)=k_Z\left(\frac1r-\frac3{2R}+\frac{r^2}{2R^3}\right)\quad(r<R),\qquad
\delta V=0\quad(r\geq R).
$$

The normalized nonrelativistic [hydrogen-like ion](../../../../hydrogen-like-ion.md) $1s$ [wavefunction](../../../../wave-function-split.md) has $|\psi(r)|^2=Z^3e^{-2Zr/a_0}/(\pi a_0^3)$. Since $ZR/a_0\ll1$, approximate it inside the [atomic nucleus](../../../../atomic-nucleus-split.md) by $|\psi(0)|^2$. First-order [time-independent perturbation theory](../../../../time-independent-perturbation-theory.md) then gives

$$
\begin{aligned}
\Delta E_{1s}&\simeq4\pi|\psi(0)|^2 k_Z\int_0^R\left(r-\frac{3r^2}{2R}+\frac{r^4}{2R^3}\right)dr\\
&=4\pi|\psi(0)|^2 k_Z\frac{R^2}{10}
=\frac25\frac{Z^4e^2}{4\pi\epsilon_0a_0}\left(\frac R{a_0}\right)^2.
\end{aligned}
$$

Define $E_H=-Z^2\mathrm{Ry}$, as the paper specifies for the [hydrogen-like ion](../../../../hydrogen-like-ion.md), rather than the neutral-[hydrogen](../../../../hydrogen.md) value. Using $\mathrm{Ry}=e^2/(8\pi\epsilon_0a_0)$ gives

$$
\boxed{\Delta E_{1s}=\frac45Z^2|E_H|\left(\frac R{a_0}\right)^2
=\frac45 Z^4\mathrm{Ry}\left(\frac R{a_0}\right)^2}
$$

to leading order in $ZR/a_0$. For $A=208$, $R\simeq7.11\,\mathrm{fm}$, $ZR/a_0\simeq0.0110$, and

$$
\boxed{\Delta E_{1s}\simeq+8.88\,\mathrm{eV},\qquad
\Delta E_{1s}/h\simeq+2.15\times10^{15}\,\mathrm{Hz}.}
$$

The finite [nuclear charge radius](../../../../nuclear-charge-radius.md) makes the [energy level](../../../../energy-level.md) less bound. The quoted [frequency](../../../../frequency.md) is a level shift divided by $h$: a line frequency shifts by $(\Delta E_u-\Delta E_l)/h$, so a decay into this shifted $1s$ level alone has the opposite sign.

The formula is a nonrelativistic, small-[nuclear charge radius](../../../../nuclear-charge-radius.md) estimate. Keeping the exponential in the first-order integral gives $\Delta E_{1s}=\Delta E_{\rm leading}[1-5ZR/(6a_0)+O((ZR/a_0)^2)]$, about a one-percent correction here. More seriously, $Z\alpha_{\rm fs}\simeq0.598$ for [lead](../../../../lead.md), so relativistic contraction is substantial. A precise physical prediction needs a finite-nucleus [Dirac equation](../../../../dirac-equation.md) calculation; the boxed estimate is the model requested, not precision heavy-ion spectroscopy.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
