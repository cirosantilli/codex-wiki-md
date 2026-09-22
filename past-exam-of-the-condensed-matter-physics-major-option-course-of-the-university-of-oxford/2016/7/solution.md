<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For $N$ ion pairs per unit volume, a relative displacement $x$ produces ionic polarization $P=Nqx$. Solving the driven [Lorentz oscillator model](../../../lorentz-oscillator-model.md) with the source's $e^{-i\omega t}$ convention gives

$$
x=\frac{qE/\mu}{\omega_{\rm TO}^2-\omega^2-i\gamma\omega},\qquad \boxed{\epsilon_r(\omega)=\epsilon_\infty+\frac{Nq^2/(\epsilon_0\mu)}{\omega_{\rm TO}^2-\omega^2-i\gamma\omega}}.
$$

The constant $\epsilon_\infty$ includes the fast electronic response: infinity here means well above the [phonon](../../../phonon.md) band but below electronic resonances. Writing $\Delta\epsilon=\epsilon_s-\epsilon_\infty$ makes the numerator $\Delta\epsilon\,\omega_{\rm TO}^2$. In an undamped longitudinal mode the bulk displacement field vanishes without an external free charge, so a nonzero [electric field](../../../electric-field-split.md) requires $\epsilon_r(\omega_{\rm LO})=0$. Therefore

$$
\omega_{\rm LO}^2=\omega_{\rm TO}^2\left(1+\frac{\Delta\epsilon}{\epsilon_\infty}\right),\qquad \boxed{\frac{\epsilon_s}{\epsilon_\infty}=\frac{\omega_{\rm LO}^2}{\omega_{\rm TO}^2}}.
$$

This is the [Lyddane-Sachs-Teller relation](../../../lyddane-sachs-teller-relation.md) for the single polar mode.

At normal incidence from vacuum the [Fresnel equations](../../../fresnel-equations.md) give

$$
R=\left|\frac{\sqrt{\epsilon_r}-1}{\sqrt{\epsilon_r}+1}\right|^2.
$$

Below the transverse resonance the dielectric response increases, raising reflectivity. Between the transverse and longitudinal frequencies the undamped dielectric function is negative, giving an evanescent transmitted wave and nearly total reflection: the [Reststrahlen band](../../../reststrahlen-effect.md). Above the longitudinal edge it becomes small and positive, passing through $\epsilon_r\simeq1$ at the reflectivity minimum and eventually approaching its electronic background.

Reading the original graph to its limited precision gives $\hbar\omega_{\rm TO}\simeq30\ \mathrm{meV}$ and $\hbar\omega_{\rm LO}\simeq37\ \mathrm{meV}$, hence $\omega_{\rm TO}\simeq4.6\times10^{13}\ \mathrm{s^{-1}}$ and $\omega_{\rm LO}\simeq5.6\times10^{13}\ \mathrm{s^{-1}}$. Extrapolating the low-energy reflectivity to roughly $R(0)\simeq0.25$ gives

$$
\epsilon_s\simeq\left(\frac{1+\sqrt{R(0)}}{1-\sqrt{R(0)}}\right)^2\simeq9,\qquad \epsilon_\infty\simeq9\left(\frac{30}{37}\right)^2\simeq5.9.
$$

Values around $9$–$10$ and $5.5$–$6.5$ are appropriate to this graphical estimate. Neither the dip near $39\ \mathrm{meV}$ nor the finite-energy right endpoint represents the high-frequency asymptote; treating that endpoint as $R(\infty)$ would underestimate $\epsilon_\infty$.

At $\omega=\omega_{\rm TO}$, $\epsilon_r=\epsilon_\infty+iA$ with $A=\Delta\epsilon\,\omega_{\rm TO}/\gamma$. Weak damping gives $A\gg\epsilon_\infty$, so for the complex [refractive index](../../../refractive-index.md) $n+i\kappa$,

$$
n\simeq\kappa\simeq\sqrt{A/2},\quad R=\frac{(n-1)^2+\kappa^2}{(n+1)^2+\kappa^2},\quad \frac{1-R}{1+R}=\frac{2n}{n^2+\kappa^2+1}\simeq\frac1n.
$$

Squaring and substituting $A$ proves

$$
\boxed{\frac\gamma{\omega_{\rm TO}}\simeq\frac{\Delta\epsilon}{2}\left(\frac{1-R_{\rm TO}}{1+R_{\rm TO}}\right)^2}.
$$

Use the reflectivity at the estimated transverse resonance, not automatically the plateau maximum. A representative reading $R_{\rm TO}\simeq0.9$, with $\Delta\epsilon\simeq3.1$, gives $\gamma/\omega_{\rm TO}\simeq0.0043$, $\gamma\simeq2.0\times10^{11}\ \mathrm{s^{-1}}$ and

$$
\boxed{\tau_{\rm energy}=1/\gamma\sim5\ \mathrm{ps}}.
$$

Graphical uncertainty in the transverse edge makes this only a few-picosecond estimate: readings $R_{\rm TO}\simeq0.85$–$0.93$ give approximately $2$–$11\ \mathrm{ps}$. The displacement amplitude decays as $e^{-\gamma t/2}$ and has lifetime $2/\gamma$; [phonon](../../../phonon.md) occupation/energy decays as $e^{-\gamma t}$ and has lifetime $1/\gamma$. Anharmonic forces allow an [optical phonon](../../../optical-phonon.md) to decay into two lower-energy [phonons](../../../phonon.md) when energy and [crystal momentum](../../../crystal-momentum.md) are conserved. Spontaneous decay can persist at low [temperature](../../../temperature-split.md); defects and [electron](../../../electron.md)–[phonon](../../../phonon.md) scattering can add further linewidth.

## ↑ Ancestors (11)

1. [7](../7.md)
2. [2016](../../2016-split.md)
3. [Past exam of the condensed matter physics major option course of the University of Oxford](../../split.md)
4. [Condensed matter physics major option course of the University of Oxford](../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
