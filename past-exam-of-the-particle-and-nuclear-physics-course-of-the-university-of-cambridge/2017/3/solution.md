<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**Alpha lifetimes and competing beta decays.** The [Geiger-Nuttall law](../../../geiger-nuttall-law.md) follows approximately from [quantum tunnelling](../../../quantum-tunnelling.md) through the daughter’s [Coulomb barrier](../../../coulomb-barrier.md). Increasing $Q_\alpha$ shortens the barrier and greatly increases the decay rate; increasing the daughter charge makes the barrier harder to penetrate. A useful local parametrization is

$$
\log_{10}\frac{T_\alpha}{\mathrm y}\simeq a\frac{Z_d}{\sqrt{Q_\alpha/\mathrm{MeV}}}+b,\qquad Z_d=Z-2.
$$

Using the supplied _nuclear_ masses, no electron-mass subtraction is needed for [alpha decay](../../../alpha-decay.md). The calculated [Q values](../../../q-value.md) are

$$
\begin{array}{c|rrrr}
\text{parent}&{}^{232}\mathrm{Th}&{}^{228}\mathrm{Th}&{}^{228}\mathrm{Ra}&{}^{228}\mathrm{Ac}\\\hline
Q_\alpha/\mathrm{MeV}&4.07063&5.51445&4.07063&4.67610
\end{array}.
$$

Calibrate the two constants to the two supplied even-even thorium [half-lives](../../../half-life.md). Their daughter charges are both 88, so

$$
a=\frac{\log_{10}(1.4\times10^{10}/1.9)}{88(1/\sqrt{4.07063}-1/\sqrt{5.51445})}\simeq1.606,\qquad b\simeq-59.92.
$$

This gives the order-of-magnitude estimates

$$
\boxed{\begin{aligned}
T_\alpha({}^{228}\mathrm{Ra})&\sim4\times10^8\,\mathrm y,&\lambda_\alpha&\sim6\times10^{-17}\,\mathrm s^{-1},\\
T_\alpha({}^{228}\mathrm{Ac})&\sim5\times10^4\,\mathrm y,&\lambda_\alpha&\sim4\times10^{-13}\,\mathrm s^{-1}.
\end{aligned}}
$$

Here $\lambda_\alpha=\ln2/T_\alpha$. The known [beta-minus decay](../../../beta-minus-decay.md) rates are approximately $3.8\times10^{-9}\,\mathrm s^{-1}$ and $3.2\times10^{-5}\,\mathrm s^{-1}$, respectively. Thus the reference alpha [branching fractions](../../../branching-fraction.md) are only about $1.6\times10^{-8}$ and $1.4\times10^{-8}$. Beta decay overwhelmingly removes the parents before alpha emission, explaining why the alpha branches are not seen in the stated chain.

These estimates are local extrapolations, not precision predictions. In particular, actinium is odd-odd, so extrapolating an even-even [Geiger-Nuttall law](../../../geiger-nuttall-law.md) neglects nuclear-structure and angular-momentum hindrance. Such effects can further suppress its alpha branch.

**Allowed daughter spin and parity.** The even-even parent in its [ground state](../../../ground-state.md) and the [alpha particle](../../../alpha-particle.md) both have $J^P=0^+$. The total final [angular momentum](../../../angular-momentum.md) must be zero, so coupling daughter spin $J_Y$ to relative orbital momentum $L$ requires $J_Y=L$. [Parity conservation](../../../parity-conservation.md) gives $+1=\pi_Y(+1)(-1)^L$. The [alpha-decay angular-momentum and parity selection rule](../../../alpha-decay-angular-momentum-and-parity-selection-rule.md) is therefore

$$
\boxed{J_Y^P=0^+,1^-,2^+,3^-,4^+,\ldots.}
$$

These are the [natural parity](../../../natural-parity.md) states. Restricting the list to even spin would be too strong; even-spin rotational bands are a further structural specialization.

**Ground-state line and recoil.** The [nuclear alpha-decay recoil correction](../../../nuclear-alpha-decay-recoil-correction.md) gives

$$
T_\alpha=Q_\alpha\frac{M_d}{M_d+m_\alpha}.
$$

For the thorium ground-state decay, this predicts $T_\alpha\simeq4.0004\,\mathrm{MeV}$, with daughter recoil about $70.2\,\mathrm{keV}$. This is close to the highest measured line, $4.0112\,\mathrm{MeV}$: the difference is $10.8\,\mathrm{keV}$, or $0.27\%$. Conversely that line implies $Q_\alpha\simeq4.0816\,\mathrm{MeV}$. The quoted nuclear masses have only five decimal places in atomic mass units; rounding three such entries can shift their mass difference by up to about $14\,\mathrm{keV}$. Thus the requested approximate agreement is supported, but the rounded table does not reproduce the line energy exactly. Dropping daughter recoil would give an error around $70\,\mathrm{keV}$ instead.

**Excited levels.** Relative to the highest line, the two alpha-energy deficits are $62.7$ and $201.2\,\mathrm{keV}$. Multiplying by the common recoil factor $1+m_\alpha/M_d\simeq232/228$ gives

$$
\boxed{E_{x,1}\simeq63.8\,\mathrm{keV},\qquad E_{x,2}\simeq204.7\,\mathrm{keV},\qquad\frac{E_{x,2}}{E_{x,1}}=3.209.}
$$

A deformed even-even [nucleus](../../../atomic-nucleus-split.md) has a ground-state [nuclear rotational band](../../../nuclear-rotational-band.md) with $E_J\simeq J(J+1)/(2\mathcal J)$ and $J^P=0^+,2^+,4^+,\ldots$. Its $4^+$ to $2^+$ excitation ratio is $20/6=10/3=3.333$, with the observed ratio about $3.7\%$ below this ideal value. The likely assignments are therefore **$2^+$ and $4^+$ rotational excitations**, with modest departures from a rigid constant-inertia rotor. The ratio supports this interpretation; it is not a unique spin measurement by itself.

**Sargent comparison.** For [beta-minus decay](../../../beta-minus-decay.md) using nuclear masses, subtract the emitted electron rest mass:

$$
\begin{aligned}
Q_\beta({}^{228}\mathrm{Ra})&=(227.98280-227.98220-0.00055)\,\mathrm u=0.046575\,\mathrm{MeV},\\
Q_\beta({}^{228}\mathrm{Ac})&=(227.98220-227.97937-0.00055)\,\mathrm u=2.12381\,\mathrm{MeV}.
\end{aligned}
$$

The simple $\lambda\propto Q^5$ version of [Sargent's rule](../../../sargent-s-rule.md) would predict

$$
\frac{\lambda_\beta(\mathrm{Ac})}{\lambda_\beta(\mathrm{Ra})}\simeq\left(\frac{2.12381}{0.046575}\right)^5=1.97\times10^8.
$$

The measured rate ratio is the inverse half-life ratio,

$$
\boxed{\frac{\lambda_\beta(\mathrm{Ac})}{\lambda_\beta(\mathrm{Ra})}=\frac{5.75\times365.25\times24}{6.1}=8.26\times10^3.}
$$

The naive fifth-power estimate is about **$2.4\times10^4$ times larger**. It correctly predicts the much faster actinium decay but fails quantitatively. The small radium endpoint is far below the electron rest mass, violating the negligible-mass approximation behind the fifth power; Coulomb distortion of the emitted electron, different nuclear matrix elements and different daughter excitations also matter. The rounded mass difference makes the very small radium $Q$ especially uncertain. The appropriate comparison of individual branches uses the actual endpoint-dependent statistical factor and [comparative half-life](../../../comparative-half-life.md), not a universal fifth power of the ground-state release.

**Beta selection rules and the four observed branches.** The radium parent has $0^+$, so the ground-state $0^+\to3^+$ transition is a [unique forbidden beta decay](../../../unique-forbidden-beta-decay.md) of second order: it preserves parity and requires three units of angular momentum. For the increasing daughter excitation energies, the endpoints decrease. The assignments are

$$
\begin{array}{c|c|c|l}
\text{daughter state}&\text{endpoint}/\mathrm{keV}&\text{intensity}&\text{classification}\\\hline
3^+\text{ ground state}&\text{about }46.6&\text{not listed}&\text{second-forbidden unique}\\
1^-\text{ first excited}&39.5&10\%&\text{first-forbidden nonunique}\\
1^+\text{ second excited}&39.1&40\%&\text{allowed Gamow-Teller}\\
1^-\text{ third excited}&25.6&20\%&\text{first-forbidden nonunique}\\
1^+\text{ fourth excited}&12.7&30\%&\text{allowed Gamow-Teller}
\end{array}.
$$

For $0^+\to1^+$, zero lepton orbital angular momentum and lepton-pair spin one give an [allowed beta decay](../../../allowed-beta-decay.md) of [Gamow-Teller transition](../../../gamow-teller-transition.md) type. The $0^+\to1^-$ branches need odd lepton orbital angular momentum, with lowest value one, and are [forbidden beta decays](../../../forbidden-beta-decay.md) of first order; they are not unique because they do not have the maximal transfer $\Delta J=2$ at that order.

The absence of a listed ground-state branch is consistent with its stronger forbiddenness. The two allowed branches carry $70\%$ in total, and the nearly equal-endpoint pair favours the allowed branch by four to one. These trends support the classification. However, first-forbidden branches still carry $30\%$, and the lower-endpoint first-forbidden branch is stronger than the higher-endpoint one. Thus selection-rule labels alone do not explain all intensities: nuclear overlaps and the endpoint-dependent [phase space](../../../phase-space.md) are indispensable. “Forbidden” means suppressed at leading order, not impossible.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [2017](../../2017-split.md)
3. [Past exam of the particle and nuclear physics course of the University of Cambridge](../../split.md)
4. [Particle and Nuclear Physics course of the University of Cambridge](../../../particle-and-nuclear-physics-course-of-the-university-of-cambridge.md)
5. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 3 of the natural sciences course of the University of Cambridge](../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../university-of-cambridge-split.md)
11. [List of universities](../../../list-of-universities.md)
12. [Codex Wiki](../../../split.md)
