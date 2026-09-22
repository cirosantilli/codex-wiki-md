<h1 id="4b/solution">Solution</h1>

↑ **Parent:** [4B](../4b.md)

In a [circular orbit](../../../../../circular-orbit.md), $r=a$ is constant, so the radial [acceleration](../../../../../acceleration.md) vanishes. The radial equation requires

$$
\boxed{h^2=ka^{n+3}}.
$$

For every $a>0$, this equation permits a real nonzero [specific angular momentum](../../../../../specific-angular-momentum.md), $h=\pm\sqrt{ka^{n+3}}$, and hence a [circular orbit](../../../../../circular-orbit.md). This chooses $h$ for the desired radius; it does not claim that one prescribed value of $h$ permits every radius.

To test [circular-orbit stability for a power-law central force](../../../../../circular-orbit-stability-for-a-power-law-central-force.md), keep that chosen [specific angular momentum](../../../../../specific-angular-momentum.md) fixed and write $r=a+\rho$, with $|\rho|\ll a$. The radial equation becomes

$$
\ddot\rho=\frac{h^2}{(a+\rho)^3}-k(a+\rho)^n.
$$

Expanding to first order and using $h^2=ka^{n+3}$ gives

$$
\ddot\rho=-\left(\frac{3h^2}{a^4}+kn a^{n-1}\right)\rho+O(\rho^2)
=-(n+3)ka^{n-1}\rho+O(\rho^2).
$$

For $n>-3$, the linearized equation is the [harmonic oscillator equation](../../../../../simple-harmonic-motion.md), with

$$
\boxed{\Omega_r^2=(n+3)ka^{n-1}>0}.
$$

The radial disturbance undergoes bounded [small oscillations](../../../../../small-oscillation.md), rather than growing. Equivalently, the [effective potential](../../../../../effective-potential.md) has a strict local minimum: its second derivative at $a$ is $(n+3)ka^{n-1}>0$. By the [effective potential stability criterion](../../../../../effective-potential-stability-criterion.md), sufficiently small radial disturbances remain small, proving **stability for $n>-3$**. For comparison, $n<-3$ gives exponential growth. At $n=-3$, the balancing value $h^2=k$ makes the radial acceleration identically zero, so a small radial velocity produces drift rather than a restoring oscillation.

## ↑ Ancestors (10)

1. [4B](../4b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
