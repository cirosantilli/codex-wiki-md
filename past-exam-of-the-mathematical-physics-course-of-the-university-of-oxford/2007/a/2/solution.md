<h1 id="a/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the normalized [Rayleigh quotient](../../../../rayleigh-quotient.md) $R(\psi)=\langle\psi,H\psi\rangle/\langle\psi,\psi\rangle$. Its real directional [derivative](../../../../derivative.md) in an arbitrary complex direction $\eta$ is

$$
\delta R=\frac{2\operatorname{Re}\langle\eta,(H-R)\psi\rangle}{\langle\psi,\psi\rangle}.
$$

It vanishes for every direction precisely when $(H-R)\psi=0$, since testing $\eta=(H-R)\psi$ gives its squared norm. Conversely an [eigenvector](../../../../eigenvector.md) makes every [derivative](../../../../derivative.md) zero. Stationarity over all states is stronger than stationarity in a restricted trial family.

Normalize the [Gaussian](../../../../normal-distribution.md) as $\psi_\alpha=(\alpha/\pi)^{1/4}e^{-\alpha x^2/2}$, with $\alpha>0$. Its moments are $\langle X^2\rangle=1/(2\alpha)$, $\langle X^4\rangle=3/(4\alpha^2)$ and $\langle P^2\rangle=\hbar^2\alpha/2$. The printed [potential energy](../../../../potential-energy.md) consequently gives

$$
\boxed{\mathcal E(\alpha)=\frac{\hbar^2\alpha}{4m}+\frac{m\omega^2}{4\alpha}+
\frac{15m^2\omega^3}{256\hbar\alpha^2}.}
$$

Put $a=\alpha\hbar/(m\omega)$. Then $\mathcal E/(\hbar\omega)=a/4+1/(4a)+15/(256a^2)$, whose second [derivative](../../../../derivative.md) is $1/(2a^3)+45/(128a^4)>0$. It diverges at both positive endpoints, so its sole [stationary point](../../../../stationary-point.md) is the unique [global minimum](../../../../global-minimum.md). Its equation is

$$
\boxed{a^3-a-\frac{15}{32}=0,\qquad a_*\simeq1.18179610.}
$$

The [variational principle](../../../../variational-principle.md) therefore yields the optimized upper bound

$$
\boxed{E_0\leq\mathcal E(\alpha_*)\simeq0.548944745\,\hbar\omega,\qquad
\alpha_*\simeq1.18179610\,\frac{m\omega}\hbar.}
$$

**The printed minimizer is inconsistent with the printed quartic coefficient.** At $a=3/2$ the [derivative](../../../../derivative.md) is $5/48>0$, so this is not the stationary [Gaussian](../../../../normal-distribution.md) for that [potential energy](../../../../potential-energy.md). It is nevertheless a legitimate trial vector and gives the simple, weaker bound $\boxed{E_0\leq109\hbar\omega/192}$. If the quartic coefficient were instead $5m^2\omega^3/(16\hbar)$, four times the printed value, then $a=3/2$ would indeed minimize the family and its [energy](../../../../energy-split.md) would be $31\hbar\omega/48$. This possible coefficient correction is identified explicitly rather than silently used. The reusable calculation is [Gaussian trial for a quadratic-plus-quartic oscillator](../../../../gaussian-trial-for-a-quadratic-plus-quartic-oscillator.md).

## ↑ Ancestors (12)

1. [2](../2.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematical physics course of the University of Oxford](../../../split.md)
5. [Mathematical physics course of the University of Oxford](../../../../mathematical-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
