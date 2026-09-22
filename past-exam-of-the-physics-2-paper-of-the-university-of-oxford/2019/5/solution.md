<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

This is a [plane electromagnetic wave](../../../plane-electromagnetic-wave.md) with [linear polarization](../../../linear-polarization.md). $\mathbf E$ is the [electric field](../../../electric-field-split.md); $E_0$ its peak [amplitude](../../../wave-amplitude.md); $x$ the position along propagation; $t$ the time; $k=2\pi/\lambda$ the [wavenumber](../../../wavenumber.md); and $\omega=2\pi f$ the [angular frequency](../../../angular-frequency.md). Here $\lambda$ is the [wavelength](../../../wavelength.md), $f$ the [frequency](../../../frequency.md), and $\hat{\mathbf y}$ the [unit vector](../../../unit-vector.md) in the direction of the [electric field](../../../electric-field-split.md). Constant [phase](../../../phase-waves.md) $kx-\omega t$ moves along $+x$ with [phase velocity](../../../phase-velocity.md) $\omega/k$.

Put $\theta=kx-\omega t$. The differential [Faraday's law of induction](../../../faraday-s-law-of-induction.md) gives

$$
\nabla\times\mathbf E=-kE_0\sin\theta\,\hat{\mathbf z}=-\frac{\partial\mathbf B}{\partial t}.
$$

The accompanying oscillating [magnetic field](../../../magnetic-field-split.md), excluding any independent static background, is therefore $\mathbf B=(k/\omega)E_0\cos\theta\,\hat{\mathbf z}$. To determine the propagation speed, also use the source-free [Ampere-Maxwell law](../../../ampere-s-circuital-law.md):

$$
\nabla\times\mathbf B=\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t},\qquad
k\frac{k}{\omega}E_0\sin\theta=\mu_0\epsilon_0\omega E_0\sin\theta.
$$

Thus

$$
\boxed{v=\frac\omega k=\frac1{\sqrt{\mu_0\epsilon_0}}=c,\qquad \mathbf B(x,t)=\frac{E_0}{c}\cos(kx-\omega t)\,\hat{\mathbf z}.}
$$

The [electric field](../../../electric-field-split.md) and [magnetic field](../../../magnetic-field-split.md) oscillate in [phase](../../../phase-waves.md), perpendicular to one another and to propagation; $\mathbf E\times\mathbf B$ points along $+x$.

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2019](../../2019-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
