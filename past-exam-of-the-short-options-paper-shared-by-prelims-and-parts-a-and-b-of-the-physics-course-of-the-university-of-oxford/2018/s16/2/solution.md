<h1 id="s16/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [plasma parameter](../../../../plasma-parameter.md) is the mean number of [electrons](../../../../electron.md) in a [Debye sphere](../../../../debye-sphere.md). With [electron](../../../../electron.md) [Debye length](../../../../debye-length.md) $\lambda_D=(\varepsilon_0k_BT/n_ee^2)^{1/2}$,

$$
\boxed{N_D=\frac{4\pi}{3}n_e\lambda_D^3.}
$$

Large $N_D$ describes weakly coupled collective screening; a single [electron](../../../../electron.md) does not dominate its screening cloud. For a small uniform [electron](../../../../electron.md) displacement $\xi$ relative to fixed [ions](../../../../ion.md), the restoring field gives $m_e\ddot\xi=-n_ee^2\xi/\varepsilon_0$, hence

$$
\boxed{\omega_p^2=\frac{n_ee^2}{\varepsilon_0m_e}.}
$$

This cold-electron [oscillation](../../../../oscillation.md) estimate neglects thermal dispersion and [ion](../../../../ion.md) motion.

Using the stipulated collision-time approximation,

$$
\tau\simeq\frac{N_D}{Z\omega_p}
=\frac{4\pi\varepsilon_0^2(k_BT)^{3/2}}{3Zn_ee^4\sqrt{m_e}}.
$$

With $C\sim3n_ek_B/2$ and $v^2\sim k_BT/m_e$, the kinetic estimate $K=Cv^2\tau/3$ gives

$$
\boxed{K=\frac{B}{Z\sqrt{m_e}}\frac{2\pi k_B\varepsilon_0^2}{3e^4}(k_BT)^{5/2}.}
$$

The elementary single-speed estimate corresponds to $B=1$; [velocity](../../../../velocity.md) averaging and the stated collision model are represented by the supplied $B$. A detailed Coulomb transport calculation also contains a [Coulomb logarithm](../../../../coulomb-logarithm.md) and cannot be inferred precisely from this simplified expression.

The [electron](../../../../electron.md) thermal [energy](../../../../energy-split.md) [density](../../../../density.md) is $3n_ek_BT/2$. Transporting all of it at the thermal [speed](../../../../speed.md) gives the free-streaming scale

$$
\boxed{\dot q_{\max}=\frac{3n_ek_BT}{2}\sqrt{\frac{k_BT}{m_e}}.}
$$

For [heat](../../../../heat-split.md) flowing in the positive $x$ direction, $-dT/dx>0$. Inserting $K$ into $K(-dT/dx)>A\dot q_{\max}$ gives

$$
\boxed{-\frac{dT}{dx}>
\frac{9AZ}{4\pi Bk_BT}\frac{n_ee^4}{k_B\varepsilon_0^2}.}
$$

This flux-limiting criterion expresses the failure of a local diffusive description when an [electron](../../../../electron.md) samples a substantial change in [temperature](../../../../temperature-split.md) over a transport path.

For the stipulated carbon [plasma](../../../../plasma-physics.md) and $B\simeq10$, setting the gradient equal to $10^{11}\,\mathrm{K\,m^{-1}}$ gives a critical flux fraction of order $A_{\rm crit}\simeq0.05$. Fourier transport is invalid according to this test when $\boxed{A<A_{\rm crit}}$; a still larger actual gradient raises the critical value. Thus the source's request for a **minimum** $A$ has the inequality reversed: the calculation gives an upper threshold, not a positive minimum. An arbitrarily smaller positive $A$ makes the criterion easier to satisfy. The exact numerical threshold is evaluated in the independent check.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [S16](../../s16.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../split.md)
5. [Short options paper shared by Prelims and Parts A and B of the physics course of the University of Oxford](../../../../short-options-paper-shared-by-prelims-and-parts-a-and-b-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../university-of-oxford-split.md)
10. [List of universities](../../../../list-of-universities.md)
11. [Codex Wiki](../../../../split.md)
