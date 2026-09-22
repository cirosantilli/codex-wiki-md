# Free Gaussian wave packet evolution

↑ **Parent:** [Gaussian wave packet](gaussian-wave-packet.md)

Let the initial [Gaussian wave packet](gaussian-wave-packet.md) be

$$
\psi(x,0)=(2\pi\sigma_0^2)^{-1/4}\exp\left[-\frac{(x-x_0)^2}{4\sigma_0^2}+\frac{ip_0(x-x_0)}\hbar\right].
$$

Fourier transforming, multiplying each momentum amplitude by $e^{-ip^2t/(2m\hbar)}$ and evaluating the [Gaussian integral](gaussian-integral.md) gives

$$
\psi(x,t)=\frac{(2\pi\sigma_0^2)^{-1/4}}{\sqrt{1+i\eta}}\exp\left[-\frac{(x-x_0-p_0t/m)^2}{4\sigma_0^2(1+i\eta)}+\frac{ip_0(x-x_0)}\hbar-\frac{ip_0^2t}{2m\hbar}\right],\qquad \eta=\frac{\hbar t}{2m\sigma_0^2}.
$$

Its [probability density](probability-density.md) is a normalized Gaussian with center $x_0+p_0t/m$ and width $\sigma_x=\sigma_0\sqrt{1+\eta^2}$; the momentum width remains $\sigma_p=\hbar/(2\sigma_0)$. Its symmetrized position-momentum [covariance](covariance.md) is $C_{xp}=t\sigma_p^2/m$, so

$$
\sigma_x\sigma_p=\frac\hbar2\sqrt{1+\eta^2},\qquad \sigma_x^2\sigma_p^2-C_{xp}^2=\frac{\hbar^2}4.
$$

Thus free spreading preserves equality in the [Robertson-Schrödinger uncertainty relation](robertson-schrodinger-uncertainty-relation.md) while producing a nonzero quadratic position-dependent phase and a product $\sigma_x\sigma_p$ larger than $\hbar/2$. More generally, $\sigma_x(t)^2=\sigma_x(0)^2+2tC_{xp}(0)/m+t^2\sigma_p(0)^2/m^2$, so an initially correlated Gaussian can first contract.

## ↑ Ancestors (6)

1. [Gaussian wave packet](gaussian-wave-packet.md)
2. [Wave function](wave-function-split.md)
3. [Quantum mechanics](quantum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
