<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The [density contrast](../../../density-contrast.md) is $\delta(\mathbf x,t)=[\rho(\mathbf x,t)-\rho_0(t)]/\rho_0(t)$, and $\delta_k(t)$ is one spatial [Fourier mode](../../../fourier-mode.md) with comoving wavevector $\mathbf k$. The [scale factor](../../../scale-factor-cosmology.md) is $a(t)$, $H=\dot a/a$ is the [Hubble parameter](../../../hubble-parameter.md), $c_s$ is the physical [sound speed](../../../speed-of-sound.md), $\rho_0$ the mean matter density, and $G$ the [gravitational constant](../../../gravitational-constant.md). For each fixed $k$ the displayed equation is an ordinary differential equation in cosmic time. It compares [pressure](../../../pressure-split.md) restoration, self-gravity and expansion-induced damping:

$$
\ddot\delta_k+2H\dot\delta_k+\left(\frac{c_s^2k^2}{a^2}-4\pi G\rho_0\right)\delta_k=0.
$$

The [pressure](../../../pressure-split.md) term resists compression; self-gravity enhances an overdensity; the $2H\dot\delta$ term slows the motion relative to a static background. The Newtonian treatment is appropriate to small perturbations on subhorizon scales within the specified fluid model, rather than an arbitrary gauge-independent treatment of superhorizon perturbations.

The physical [Jeans length](../../../jeans-length.md) follows by equating [pressure](../../../pressure-split.md) and gravity:

$$
\boxed{k_{J,\rm phys}=\frac{\sqrt{4\pi G\rho_0}}{c_s},\qquad
\lambda_{J,\rm phys}=\frac{2\pi}{k_{J,\rm phys}}=c_s\sqrt{\frac\pi{G\rho_0}}.}
$$

The comoving Jeans wavenumber is $a k_{J,\rm phys}$. Perturbations well below the physical Jeans length are [pressure](../../../pressure-split.md)-supported acoustic oscillations whose amplitude is modified by expansion; those above it admit gravitational growth when the background evolution permits. Pressureless matter in a matter-dominated universe is the example below. Merely having a large wavelength is not sufficient to apply this Newtonian equation outside the horizon.

For a gas of particle [mass](../../../mass.md) $m$ and [temperature](../../../temperature-split.md) $T$, write $c_s^2=\Gamma k_BT/m$, with $\Gamma=1$ for the isothermal sound-speed convention or the appropriate adiabatic heat-capacity ratio otherwise. Then

$$
\boxed{\lambda_{J,\rm phys}=\left(\frac{\pi\Gamma k_BT}{G\rho_0m}\right)^{1/2}.}
$$

At fixed density it is larger for hotter or lighter particles, and it decreases with increasing density. Numerical coefficients differ between sound-crossing and self-gravitating-sphere conventions; the expression here uses the Fourier instability boundary of the stated equation.

In an [Einstein-de Sitter universe](../../../einstein-de-sitter-universe.md), the spatially flat [Friedmann-Lemaître-Robertson-Walker metric](../../../friedmann-lemaitre-robertson-walker-metric.md) is $ds^2=-c^2dt^2+a^2(t)d\mathbf x^2$. Conservation of pressureless matter gives $\rho_0a^3=\mathrm{constant}$; the [Friedmann equation](../../../friedmann-equations.md) then gives $a\propto t^{2/3}$, $H=2/(3t)$ and $\rho_0=1/(6\pi Gt^2)$. With $c_s=0$,

$$
\ddot\delta+\frac4{3t}\dot\delta-\frac2{3t^2}\delta=0.
$$

Trying $\delta=t^p$ gives $p^2+p/3-2/3=(p-2/3)(p+1)=0$. Hence the [Einstein-de Sitter density-growth modes](../../../einstein-de-sitter-density-growth-modes.md) are

$$
\boxed{\delta=C_+t^{2/3}+C_-t^{-1}=D_+a+D_-a^{-3/2}.}
$$

The growing mode increases only as a power law because the expansion dilutes and slows the collapsing matter.

[Conformal time](../../../conformal-time.md) is defined by $d\eta=dt/a(t)$, so the metric becomes $ds^2=a^2(-c^2d\eta^2+d\mathbf x^2)$. Choosing its origin at the big bang gives $\eta\propto t^{1/3}$ and $a\propto\eta^2$. Therefore

$$
\boxed{\delta=A_+\eta^2+A_-\eta^{-3}.}
$$

Equivalently the equation is $\delta''+2\delta'/\eta-6\delta/\eta^2=0$, where primes denote conformal-time derivatives.

Before and through [cosmological recombination](../../../recombination-cosmology.md), [photons](../../../photon.md) diffuse between hotter and cooler parts of the tightly coupled [photon](../../../photon.md)–baryon fluid. Radiative viscosity and heat transport erase short-wavelength acoustic perturbations. As free [electrons](../../../electron.md) disappear, the [photon](../../../photon.md) mean free path grows, enhancing this diffusion before decoupling. [Silk damping](../../../cosmic-microwave-background-diffusion-damping.md) can be represented by a factor approximately $e^{-k^2/k_D^2}$ in the linear acoustic amplitude. The comoving Silk wavelength may be defined as $\lambda_D=2\pi/k_D$; the associated diffusion-length convention is $r_D=1/k_D$.

A random-walk estimate is $r_D^2\sim\int c\lambda_\gamma\,dt/a^2$ up to transport and baryon-loading factors, with physical $\lambda_\gamma=(n_e\sigma_T)^{-1}$. Scales much shorter than the damping wavelength are strongly suppressed. This is [photon](../../../photon.md) diffusion, not the Jeans boundary and not erasure of every cold-dark-matter perturbation. After decoupling, [photon](../../../photon.md) free streaming is a distinct part of the evolution.

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2016](../../2016-split.md)
3. [Past exam of the astrophysics course of the University of Oxford](../../split.md)
4. [Astrophysics course of the University of Oxford](../../../astrophysics-course-of-the-university-of-oxford.md)
5. [Year 4 of the physics course of the University of Oxford](../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
