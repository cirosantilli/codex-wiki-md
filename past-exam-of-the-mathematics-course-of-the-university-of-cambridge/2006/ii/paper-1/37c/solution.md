<h1 id="37c/solution">Solution</h1>

↑ **Parent:** [37C](../37c.md)

For the [reflection of a P-wave from a rigid plane](../../../../../reflection-of-a-p-wave-from-a-rigid-plane.md), use the [displacement](../../../../../displacement.md) convention $u_x=\phi_x+\psi_y$, $u_y=\phi_y-\psi_x$, where $\phi$ is the P potential and $\psi$ the SV potential. Put $\omega=kc_p$, $\kappa=k\sin\theta$, $a=k\cos\theta$, and $b=\sqrt{\omega^2/c_s^2-\kappa^2}$. The reflected waves must share the tangential [wavenumber](../../../../../wavenumber.md) and [frequency](../../../../../frequency.md) and propagate towards negative $y$, so write

$$
\phi_R=Ae^{i(\kappa x-ay-\omega t)},\qquad\psi_R=Be^{i(\kappa x-by-\omega t)}.
$$

The rigid barrier requires both [displacement](../../../../../displacement.md) components to vanish. On $y=0$ this gives $\kappa(1+A)-bB=0$ and $a(1-A)-\kappa B=0$. Solving,

$$
\boxed{A=\frac{ab-\kappa^2}{ab+\kappa^2},\qquad B=\frac{2a\kappa}{ab+\kappa^2}.}
$$

The total P potential is the given incident wave plus $\phi_R$, and the S potential is $\psi_R$. Reversing the sign convention for $\psi$ reverses $B$ but leaves the [displacement](../../../../../displacement.md) unchanged. At normal incidence $A=1,B=0$.

An evanescent reflected [S wave](../../../../../s-wave.md) would require $b^2<0$, or $\sin\theta>c_p/c_s$. In a stable isotropic elastic solid $c_p>c_s$, so this is impossible for real incidence angles: $b^2=k^2[(c_p/c_s)^2-\sin^2\theta]>0$. **The reflected [S wave](../../../../../s-wave.md) is never evanescent in the physical isotropic case.** The inequality identifies the hypothetical critical-angle case if the speed ordering were reversed; it is S-to-P conversion, not this P-to-S conversion, that can become evanescent in an ordinary solid.

## ↑ Ancestors (10)

1. [37C](../37c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
