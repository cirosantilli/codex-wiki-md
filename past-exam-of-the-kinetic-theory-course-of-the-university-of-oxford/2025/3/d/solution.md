<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The restriction $k_\varphi=\pm m$ describes an $m$-fold rotating perturbation of a [galactic disk](../../../../galactic-disk.md), for example a transient [spiral density wave](../../../../spiral-density-wave.md) or, for $m=2$, a [galactic bar](../../../../galactic-bar.md). Its [pattern speed](../../../../pattern-speed.md) is $\Omega_{\mathrm p}$, its amplitude peaks at $t_{\mathrm{peak}}$, and its [Gaussian function](../../../../gaussian-function.md) envelope has duration of order $\tau$. The coefficients $u_{\mathbf k}(\mathbf J)$ describe its strength along different [stellar orbits](../../../../stellar-orbit.md). A real perturbing potential requires $u_{-\mathbf k}=u_{\mathbf k}^*$.

Write $g(t)=\exp[-(t-t_{\mathrm{peak}})^2/(2\tau^2)]$. The product entering [c](../c.md) is

$$
\delta\phi_{\mathbf k}(t')\delta\phi_{\mathbf k}^*(t)=|u_{\mathbf k}|^2e^{ik_\varphi\Omega_{\mathrm p}(t-t')}g(t')g(t).
$$

The phase therefore measures detuning from the rotating pattern:

$$
\boxed{\omega_{\mathbf k}(\mathbf J)=\mathbf k\cdot\boldsymbol\Omega-k_\varphi\Omega_{\mathrm p}=k_\varphi(\Omega_\varphi-\Omega_{\mathrm p})+k_R\Omega_R.}
$$

Substitution gives

$$
\boxed{\begin{aligned}
Q_0={}&-2\pi\sum_{k_\varphi=\pm m}\sum_{k_R}k_\varphi\int_0^\infty dJ_R\,|u_{\mathbf k}|^2\\
&\times\int_0^t dt'\,\mathbf k\cdot\partial_{\mathbf J}f_0(\mathbf J,t')\,e^{-i\omega_{\mathbf k}(t-t')}\\
&\times\exp\left[-\frac{(t-t_{\mathrm{peak}})^2}{2\tau^2}-\frac{(t'-t_{\mathrm{peak}})^2}{2\tau^2}\right].
\end{aligned}}
$$

The strongest long-lived response occurs near an orbital [resonance](../../../../resonance.md), $\omega_{\mathbf k}=0$, where successive [force](../../../../force-split.md) contributions do not rapidly cancel in phase.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [3](../../3.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
