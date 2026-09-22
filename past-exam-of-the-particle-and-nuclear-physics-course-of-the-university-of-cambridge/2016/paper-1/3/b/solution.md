<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Assume [allowed beta decay](../../../../../allowed-beta-decay.md), so the leading [matrix element](../../../../../matrix-element.md) has negligible lepton-momentum dependence. Neglect [nuclear recoil](../../../../../nuclear-recoil.md) and [neutrino mass](../../../../../neutrino-mass.md). Let $Q$ be the [kinetic energy](../../../../../kinetic-energy.md) available to the [electron](../../../../../electron.md) and [antineutrino](../../../../../antineutrino.md), $E_0=m_e+Q$, and $E=\sqrt{p^2+m_e^2}$. The [neutrino](../../../../../neutrino.md) [energy](../../../../../energy-split.md) and [momentum](../../../../../momentum-split.md) magnitude are $k=E_0-E$.

[Fermi's golden rule](../../../../../fermi-s-golden-rule.md) weights accessible final states. After angular integration, the momentum-space factors are $p^2\,dp$ and $k^2\,dk$. The energy-conserving [Dirac delta function](../../../../../dirac-delta-function.md) removes the [neutrino](../../../../../neutrino.md) integral:

$$
d\Gamma=Cp^2\,dp\int_0^\infty k^2\,dk\,\delta(E_0-E-k).
$$

The constant includes the allowed nuclear [matrix element](../../../../../matrix-element.md), weak-coupling and angular factors. Including the usual [Fermi function](../../../../../fermi-function.md) for electron-nucleus Coulomb distortion gives

$$
\boxed{\frac{d\Gamma}{dp}=C F(Z,E)\,p^2(E_0-\sqrt{p^2+m_e^2})^2,\quad
0\leq p\leq\sqrt{Q(Q+2m_e)}.}
$$

For the kinetic-energy spectrum, $dp/dT=E/p$ instead yields

$$
\frac{d\Gamma}{dT}=C F(Z,E)\,pE(Q-T)^2.
$$

The two distributions differ by a Jacobian; forgetting it changes the shape.

A pure fifth-power law additionally neglects [electron](../../../../../electron.md) [mass](../../../../../mass.md) and Coulomb distortion and keeps the nuclear [matrix element](../../../../../matrix-element.md) fixed. Then $E=p$, $E_0\simeq Q$, and

$$
\Gamma=C\int_0^Q p^2(Q-p)^2\,dp
=CQ^5\int_0^1x^2(1-x)^2\,dx
=\boxed{\frac{C}{30}Q^5.}
$$

Two [momentum](../../../../../momentum-split.md) powers come from each final particle and one from the remaining integration. This is the origin of the [Sargent rule](../../../../../sargent-rule.md). **Exact $Q^5$ dependence requires the relativistic-electron, constant-matrix-element limit.** For $Q\ll m_e$, the same approximation without Coulomb distortion has $pE\simeq m_e\sqrt{2m_eT}$ and instead scales as $m_e^{3/2}Q^{7/2}$. Forbidden-transition factors, nuclear-structure changes and Coulomb distortion also modify the simple law.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2016](../../../split.md)
5. [Past exam of the particle and nuclear physics course of the University of Cambridge](../../../../split.md)
6. [Particle and Nuclear Physics course of the University of Cambridge](../../../../../particle-and-nuclear-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
