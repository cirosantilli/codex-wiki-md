<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\kappa=kV_e/\omega_{\mathrm pe}$ and $s=\omega/(kV_e)$. The long-[wavelength](../../../../wavelength.md) electron branch has $|s|\gg1$. The convergent [power series](../../../../power-series.md)

$$
\log\frac{s-1}{s+1}=-2\left(\frac1s+\frac1{3s^3}+\frac1{5s^5}+\cdots\right)
$$

turns the [degenerate-plasma dielectric response](../../../../degenerate-plasma-dielectric-response.md) into

$$
0=1-\frac{\omega_{\mathrm pe}^2}{\omega^2}
-\frac{3\omega_{\mathrm pe}^2 k^2V_e^2}{5\omega^4}
+O\left(\frac{\omega_{\mathrm pe}^2 k^4V_e^4}{\omega^6}\right).
$$

Substitute $\omega^2=\omega_{\mathrm pe}^2+a k^2V_e^2+O(k^4V_e^4/\omega_{\mathrm pe}^2)$. The coefficient of $k^2$ is $a-3/5$, so the [degenerate-plasma Langmuir dispersion](../../../../degenerate-plasma-langmuir-dispersion.md) is

$$
\boxed{\omega^2=\omega_{\mathrm pe}^2+\frac35 k^2V_e^2+O\left(\frac{k^4V_e^4}{\omega_{\mathrm pe}^2}\right),\qquad
\omega_\pm=\pm\omega_{\mathrm pe}\left[1+\frac3{10}\kappa^2+O(\kappa^4)\right].}
$$

The [Langmuir wave](../../../../langmuir-wave.md) therefore has a finite [frequency](../../../../frequency.md) at zero [wavenumber](../../../../wavenumber.md), with the first dispersive correction set by the [Fermi velocity](../../../../fermi-velocity.md). Indeed the occupied [Fermi sphere](../../../../fermi-sphere.md) has $\langle v_\parallel^2\rangle=V_e^2/5$, so the coefficient $3\langle v_\parallel^2\rangle=3V_e^2/5$ agrees with the high-[phase velocity](../../../../phase-velocity.md) [velocity moment](../../../../velocity-moment.md) expansion.

**Screening-length convention.** The source defines $\lambda_{\mathrm De}^{\rm exam}=\sqrt3 V_e/\omega_{\mathrm pe}$, so its long-[wavelength](../../../../wavelength.md) condition is equivalent to $\kappa\ll1$. We retain that definition when expressing answers in its symbols. The actual electron [Thomas-Fermi screening length](../../../../thomas-fermi-screening-length.md) obtained from the static response is instead

$$
\epsilon_e(0,k)=1+\frac{3\omega_{\mathrm pe}^2}{k^2V_e^2}
=1+\frac1{k^2\lambda_{\rm TF}^2},\qquad
\boxed{\lambda_{\rm TF}=\frac{V_e}{\sqrt3\omega_{\mathrm pe}}=\frac{\lambda_{\mathrm De}^{\rm exam}}3.}
$$

For a concrete comparison, at $k=\omega_{\mathrm pe}/V_e$, the static [dielectric function](../../../../dielectric-function.md) is $4$; using the printed length as the physical [Thomas-Fermi screening length](../../../../thomas-fermi-screening-length.md) would give $1+1/3=4/3$. Calling the printed length the [Debye length](../../../../debye-length.md) thus differs from the physical degenerate-electron screening convention by a factor of three. It does not affect the boxed dimensional [dispersion relation](../../../../dispersion-relation-split.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
