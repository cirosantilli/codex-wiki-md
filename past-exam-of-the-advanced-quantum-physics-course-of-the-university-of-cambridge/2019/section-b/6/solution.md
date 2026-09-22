<h1 id="section-b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

Expand the time-dependent [quantum state](../../../../quantum-state.md) in unperturbed [energy eigenstates](../../../../energy-eigenstate.md), factoring out free dynamical phases:

$$
|\psi(t)\rangle=\sum_n c_n(t)e^{-iE_nt/\hbar}|n\rangle.
$$

The [Schrödinger equation](../../../../schrodinger-equation.md) gives the exact [interaction picture](../../../../interaction-picture.md) coefficient equations

$$
i\hbar\dot c_j(t)=\sum_n e^{i(E_j-E_n)t/\hbar}
\langle j|\Delta V(t)|n\rangle c_n(t).
$$

Initially $c_n(-\infty)=\delta_{ni}$. To first order in [time-dependent perturbation theory](../../../../time-dependent-perturbation-theory.md), replace the coefficients on the right by these zeroth-order values and integrate. Thus

$$
S_{ji}=\delta_{ji}+\gamma_{ji}^{(1)}+O(\Delta V^2),\qquad
\boxed{\gamma_{ji}^{(1)}=\frac1{i\hbar}\int_{-\infty}^{\infty}
 e^{i\omega_{ji}t}\langle j|\Delta V(t)|i\rangle dt.}
$$

For a transition $j\ne i$, this is the desired leading [probability amplitude](../../../../probability-amplitude.md), and $P_{ji}=|\gamma_{ji}^{(1)}|^2$ to leading order. The formula is understood with free asymptotic phases removed. For $j=i$, the full survival amplitude also contains the zeroth-order $1$; the displayed integral alone is its first-order correction, not the whole amplitude. This specifies the usual [scattering operator](../../../../s-matrix.md) meaning of the paper's notation at infinite times.

For the ion pulse, write $x_{ji}=\langle j|x|i\rangle$ and $y_{ji}=\langle j|y|i\rangle$. Then

$$
\gamma_{ji}^{(1)}=\frac{Ze^2}{i\hbar}(x_{ji}I_x+y_{ji}I_y),
$$



$$
I_x=\int_{-\infty}^{\infty}\frac{b e^{i\omega_{ji}t}}{(b^2+v^2t^2)^{3/2}}dt,\qquad
I_y=\int_{-\infty}^{\infty}\frac{vt e^{i\omega_{ji}t}}{(b^2+v^2t^2)^{3/2}}dt.
$$

Consider an excitation with $\omega_{ji}>0$ and put $\beta=\omega_{ji}b/v$, $u=\omega_{ji}t$. The first real pulse is even in time and the second is odd. Their respective surviving Fourier components are therefore cosine and imaginary sine:

$$
I_x=\frac{2b\omega_{ji}^2}{v^3}\int_0^\infty
\frac{\cos u}{(\beta^2+u^2)^{3/2}}du
\simeq\frac{2b\omega_{ji}^2}{v^3\beta^2}=\frac2{bv},
$$



$$
I_y=\frac{2i\omega_{ji}}{v^2}\int_0^\infty
\frac{u\sin u}{(\beta^2+u^2)^{3/2}}du
\simeq\frac{2i}{bv}\,\beta(c-\log\beta).
$$

Since $\beta\log(1/\beta)\to0$, the longitudinal term is smaller for comparable position [matrix elements](../../../../matrix-element.md). Hence the [electric-dipole excitation by a passing ion](../../../../electric-dipole-excitation-by-a-passing-ion.md) has

$$
\gamma_{ji}^{(1)}\simeq\frac{2Ze^2}{i\hbar bv}x_{ji},\qquad
\boxed{P_{ji}\simeq\left(\frac{2Ze^2}{\hbar bv}\right)^2|x_{ji}|^2.}
$$

This leading limit extends to either sign of $\omega_{ji}$ using $|\omega_{ji}|b/v\ll1$. If $x_{ji}=0$ by a [selection rule](../../../../selection-rule.md), the retained leading term vanishes and the smaller longitudinal term may give the first nonzero probability. The conditions also include a small total transition probability, approximately straight constant-velocity motion, and $b$ large compared with atomic size for the [electric-dipole approximation](../../../../electric-dipole-approximation.md). The paper uses a Coulomb-coupling convention in which the factor is written $Ze^2$; in SI units replace $e^2$ throughout by $e^2/(4\pi\epsilon_0)$.

The collision duration is of order $b/v$. Excitations with angular frequency $\omega_{ji}$ receive an unsuppressed impulse when this is short relative to $1/\omega_{ji}$. In contrast, for $\omega_{ji}b/v\gg1$, cancellations in the [Fourier transform](../../../../fourier-transform-split.md) suppress the transition: a slowly varying distant field approximately preserves the atomic [energy eigenstate](../../../../energy-eigenstate.md). The exact dipole-pulse transforms make this explicit:

$$
I_x=\frac{2\beta K_1(\beta)}{bv},\qquad I_y=\frac{2i\beta K_0(\beta)}{bv}\quad(\omega_{ji}>0),
$$

where $K_\nu$ is a [Modified Bessel function of the second kind](../../../../modified-bessel-function-of-the-second-kind.md). Their large-argument exponential decrease explains the slow-passage cutoff. These transforms are optional refinements of the small-$\beta$ derivation above, not a separate assumption about the target.

To connect the microscopic [transition probability](../../../../transition-probability.md) to energy loss, suppose the atom begins in a low-energy state. Exciting bound electronic states and causing [ionization](../../../../ionization.md) transfer positive energies $E_j-E_i$ from the ion to the material. For target atomic [number density](../../../../number-density.md) $n_{\rm at}$ and path length $d$, a schematic independent-encounter sum is

$$
\delta E\simeq n_{\rm at}d\sum_j(E_j-E_i)
\int 2\pi b\,db\,P_{ji}(b,v),
$$

with a continuum integral as well as a sum for ionized final states. The short-collision formula gives $P_{ji}\propto Z^2/(b^2v^2)$, so the impact-parameter integral has logarithmic dependence on its cutoffs. Its upper effective cutoff is of order $v/\omega_{ji}$, where the transition ceases to be sudden; the lower cutoff must exclude regions where the dipole or weak-collision approximation fails. Thus the leading [high-speed charge and isotope scaling of electronic stopping](../../../../high-speed-charge-and-isotope-scaling-of-electronic-stopping.md) is

$$
\boxed{\delta E\propto\frac{Z^2}{v^2}\times\text{a slowly varying excitation factor}.}
$$

Although a faster ion can access more energetic transitions and a wider range of distant encounters, its shorter interaction time reduces each ordinary excitation probability. In the fast-ion regime shown, the $1/v^2$ decrease dominates the slower variation of the excitation factor. The energy loss consequently falls with increasing incident [kinetic energy](../../../../kinetic-energy.md). The original figure has $\delta E$ increasing downward, so the curves' rise toward the top of the page means decreasing loss, not increasing loss. A low-speed extrapolation of the inverse-square law is invalid because excitation thresholds, slow-passage suppression, changing ion charge and nuclear recoil can then matter.

For nonrelativistic ion mass $M$, $E=Mv^2/2$. At fixed incident energy the leading prediction becomes

$$
\boxed{\delta E\propto\frac{Z^2M}{E}\quad\text{up to the slower excitation dependence}.}
$$

The greater [atomic number](../../../../atomic-number.md) of nitrogen than carbon than boron therefore gives larger loss; at the same velocity the leading species factor is $Z^2$. Within an isotopic family, the heavier ion moves more slowly at the same $E$ and loses more energy. Equivalently, a heavier isotope needs proportionally greater kinetic energy to achieve the same velocity and approximately the same electronic loss. Comparing at fixed energy per nucleon, rather than fixed total $E$, approximately removes this leading [isotope](../../../../isotope.md) mass dependence. This accounts for the separate isotope bands in the original graph without assigning different electronic excitation spectra to isotopes of the same projectile element.

The charge in this scaling is the effective ion charge if screening by bound projectile electrons is important. The interpretation assumes the same traversed material and thickness and uses the paper's small-fractional-loss regime, $\delta E/E\ll1$; points with loss comparable to incident energy cannot be described quantitatively by treating $v$ as constant. The plotted curves support the qualitative ordering and high-energy decrease, rather than determining a universal normalization from the supplied single-atom model.

## ↑ Ancestors (13)

1. [6](../6.md)
2. [Section B](../../section-b.md)
3. [2019](../../../2019-split.md)
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
