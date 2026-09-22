<h1 id="37e/solution">Solution</h1>

↑ **Parent:** [37E](../37e.md)

Substitution of $e^{i(kx-\omega t)}$ gives the [dispersion relation](../../../../../dispersion-relation.md) $\boxed{\omega(k)=Uk+k^3}$. The [phase velocity](../../../../../phase-velocity.md) is $U+k^2$, whereas the [group velocity](../../../../../group-velocity.md) is $U+3k^2$. Thus nonzero-wavenumber crests move more slowly than their wave packet; the velocities coincide at zero wavenumber.

Fourier evolution gives $\phi(Vt,t)=\int A(k)e^{it\Phi(k)}\,dk$, where $\Phi(k)=(V-U)k-k^3$. For $V>U$ the two nondegenerate stationary points are $k=\pm\kappa$, $\kappa=\sqrt{(V-U)/3}$. At these points $\Phi(\pm\kappa)=\pm2\kappa^3$ and $\Phi''(\pm\kappa)=\mp6\kappa$. Expanding the phase quadratically near each point and evaluating the oscillatory Gaussian integral gives the [stationary phase method](../../../../../stationary-phase-method.md)

$$
\boxed{\phi(Vt,t)\sim\sqrt{\frac{\pi}{3\kappa t}}\left[
A(\kappa)e^{i(2\kappa^3t-\pi/4)}+A(-\kappa)e^{-i(2\kappa^3t-\pi/4)}\right].}
$$

For a real initial field, $A(-\kappa)=\overline{A(\kappa)}$, so the two terms are conjugate. The approximation assumes a sufficiently smooth decaying amplitude; if a leading coefficient vanishes, the next stationary-phase terms determine that contribution.

For $V<U$, $\Phi'(k)=V-U-3k^2<0$ everywhere. There are no real stationary points, so no leading propagating packet reaches such a ray. For a Schwartz amplitude, repeated integration by parts with $e^{it\Phi}=(it\Phi')^{-1}\partial_ke^{it\Phi}$ makes the contribution $O(t^{-N})$ for every fixed $N$. With weaker data the decay rate depends on their regularity. This agrees with the minimum [group velocity](../../../../../group-velocity.md) being $U$.

## ↑ Ancestors (10)

1. [37E](../37e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
