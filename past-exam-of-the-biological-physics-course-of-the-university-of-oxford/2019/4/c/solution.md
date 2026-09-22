<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take forward as increasing $x$, and specify the sinusoidal amplitude convention by

$$
U(x)=A[1-\cos(2\pi x/d)]-Fx.
$$

Thus the unforced barrier is $2A$, not $A$. Let $s=Fd/(2\pi A)=0.7051$ and $\theta=\arcsin s$. Stationary points exist because $F<2\pi A/d=7.09\,\mathrm{pN}$. A minimum is at $x_m=d\theta/(2\pi)$ and its forward saddle at $x_+=d(\pi-\theta)/(2\pi)$. The distances and activation barriers are

$$
\ell_+=\frac d2-\frac{d\theta}\pi=1.756\,\mathrm{nm},\quad
\ell_-=d-\ell_+=5.244\,\mathrm{nm},
$$



$$
\Delta U_+=2A\sqrt{1-s^2}-F\ell_+=2.422\,\mathrm{pN\,nm},\qquad
\Delta U_-=2A\sqrt{1-s^2}+F\ell_-=37.422\,\mathrm{pN\,nm}.
$$

Use an [Arrhenius estimate](../../../../arrhenius-equation.md) with the supplied distance-squared waiting-time scaling, $\tau\propto\ell^2e^{\Delta U/(k_BT)}$. Calibrate at $F=0$ with $\ell_0=d/2$ and rate $k_0=1\,\mathrm{s^{-1}}$ in each direction. At the explicit room-[temperature](../../../../temperature-split.md) estimate $T=300\,\mathrm K$, $k_BT=4.142\,\mathrm{pN\,nm}$, giving

$$
\boxed{k_+\simeq k_0\left(\frac{d/2}{\ell_+}\right)^2e^{(2A-\Delta U_+)/(k_BT)}\simeq100\,\mathrm{s^{-1}}.}
$$

Applying the same distance rule separately backwards gives $k_-\simeq0.00241\,\mathrm{s^{-1}}$ and hence the literal scaling-model estimate

$$
\boxed{f_-^{\rm distance\ rule}=\frac{k_-}{k_++k_-}\simeq2.4\times10^{-5}.}
$$

**Thermodynamic qualification:** for isothermal [diffusion](../../../../diffusion.md) in this translated tilted potential, adjacent wells differ by $Fd=35\,\mathrm{pN\,nm}$, so [local detailed balance](../../../../local-detailed-balance.md) instead requires $k_+/k_-=e^{Fd/(k_BT)}$. The two separate distance prefactors introduce an extra factor $(\ell_-/\ell_+)^2\simeq8.91$, inconsistent with that requirement. Keeping the forward estimate while enforcing the proper ratio gives

$$
\boxed{k_-^{\rm DB}\simeq0.0215\,\mathrm{s^{-1}},\qquad
f_-^{\rm DB}=\frac1{1+e^{Fd/(k_BT)}}\simeq2.14\times10^{-4}.}
$$

Both interpretations are shown because the supplied distance heuristic is not, by itself, a thermodynamically consistent prescription for both directional prefactors. Additional hidden chemical driving would require its own affinity, not an unexplained prefactor asymmetry. A common transition-state prefactor, as in a consistent [Kramers model](../../../../kramers-escape-rate.md), preserves the [Boltzmann rate ratio](../../../../local-detailed-balance.md). Moreover the forward barrier is only about $0.58k_BT$, so rare-escape exponential dwell kinetics and the numerical rate should be regarded as rough estimates. If “amplitude” meant the entire unforced barrier height, the maximum restoring [force](../../../../force-split.md) would be only $\pi A/d=3.55\,\mathrm{pN}$ and no dwell wells would survive at $5\,\mathrm{pN}$; the amplitude convention is therefore essential.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
