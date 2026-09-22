<h1 id="39c/solution">Solution</h1>

↑ **Parent:** [39C](../39c.md)

Write the density and pressure as $\rho_0+\rho'$ and $p_0+p'$, and let the small fluid velocity be the gradient of an [acoustic velocity potential](../../../../../acoustic-velocity-potential.md), $\mathbf u=\nabla\phi$. The [linear homentropic acoustic equations](../../../../../linear-homentropic-acoustic-equations.md) are

$$
\rho'_t+\rho_0\nabla^2\phi=0,
\qquad
\rho_0\nabla\phi_t=-\nabla p',
\qquad
p'=c_0^2\rho',
$$

where the [adiabatic sound speed](../../../../../adiabatic-sound-speed.md) of a perfect gas is $c_0^2=\gamma p_0/\rho_0$. Absorbing a function of time into $\phi$, the momentum equation gives

$$
\boxed{p'=-\rho_0\phi_t.}
$$

Eliminating $p'$ and $\rho'$ gives the acoustic [wave equation](../../../../../wave-equation-split.md)

$$
\boxed{\phi_{tt}=c_0^2\nabla^2\phi.}
$$

Let the shell displacement be $a(t)-a_0=\operatorname{Re}(\eta e^{-i\omega t})$ and put $k=\omega/c_0$, $\theta=ka_0$. The spherically symmetric solution regular at the centre is

$$
\phi(r,t)=\operatorname{Re}\left(A\frac{\sin kr}{r}e^{-i\omega t}\right).
$$

The [kinematic boundary condition](../../../../../kinematic-boundary-condition.md) $\phi_r(a_0,t)=\dot a(t)$ gives

$$
A\frac{\sin\theta}{a_0^2}(\theta\cot\theta-1)
=-i\omega\eta.
$$

Since $p'=-\rho_0\phi_t$, the pressure amplitude on the shell is therefore

$$
\widehat p(a_0)=
\frac{\rho_0\omega^2a_0}{\theta\cot\theta-1}\eta.
$$

The radial [Newton's second law](../../../../../newton-s-second-law.md) per unit area is

$$
m\ddot a=p'(a_0,t)-\kappa(a-a_0),
$$

so its complex amplitude satisfies

$$
(\kappa-m\omega^2)\eta=\widehat p(a_0).
$$

For a nonzero mode, cancellation of $\eta$ and multiplication by $a_0^2/(mc_0^2)$ yield the frequency equation for [spherically symmetric vibration of a gas-filled elastic shell](../../../../../spherically-symmetric-vibration-of-a-gas-filled-elastic-shell.md):

$$
\boxed{\theta^2\left(1+\frac{\alpha}{\theta\cot\theta-1}\right)
=\frac{\kappa a_0^2}{mc_0^2},
\qquad
\alpha=\frac{\rho_0a_0}{m}.}
$$

The spectrum is discrete and contains infinitely many positive solutions. Indeed, for sufficiently large $n$, $\theta\cot\theta-1$ runs from $+\infty$ to $-\infty$ on $(n\pi,(n+1)\pi)$, forcing at least one root there. These high modes are predominantly standing acoustic modes of the gas, while the lowest mode is predominantly the shell's radial breathing mode; the coupling shifts both families.

## ↑ Ancestors (10)

1. [39C](../39c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
