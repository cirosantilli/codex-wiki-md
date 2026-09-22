<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume small-amplitude, nonrotating, inviscid [Boussinesq approximation](../../../../../../boussinesq-approximation.md) motion about a fluid at rest, with stable background stratification. In either uniform layer let $b=-g\rho'/\rho_*$ be the buoyancy perturbation and $N^2=-(g/\rho_*)\rho_0'(z)>0$. The linear equations are

$$
u_t=-p_x/\rho_*,\qquad w_t=-p_z/\rho_*+b,\qquad b_t+N^2w=0,\qquad u_x+w_z=0.
$$

For a [plane internal gravity wave](../../../../../../plane-internal-gravity-wave.md) proportional to $e^{i(kx+mz-\omega t)}$, continuity gives $u=-mw/k$, and horizontal momentum gives $p=\rho_*\omega u/k$. Substituting these into vertical momentum and buoyancy evolution gives

$$
\boxed{\omega^2=\frac{N^2k^2}{k^2+m^2}.}
$$

Choose $k>0$, $\omega>0$. Its [group velocity](../../../../../../group-velocity.md) is

$$
\mathbf c_g=\left(\frac{Nm^2}{(k^2+m^2)^{3/2}},-\frac{Nkm}{(k^2+m^2)^{3/2}}\right).
$$

Thus downward energy propagation has $m>0$. If $\theta$ is the acute angle between the ray and the vertical in its direction of propagation, then $\tan\theta=|m|/k$, so

$$
\boxed{\cos\theta_j=\omega/N_j,\qquad\theta_j=\arccos(\omega/N_j).}
$$

The [phase velocity](../../../../../../phase-velocity.md) is parallel to $(k,m)$, while $\mathbf c_g\cdot(k,m)=0$: **phase and group velocities are perpendicular**, and their vertical components have opposite signs. Propagating incident waves require $0<\omega<N_1$; both layers support propagating waves only when $0<\omega<\min(N_1,N_2)$. At or above $N_2$, the lower layer cannot carry a propagating downward internal wave.

For the amplitude convention used below, $\eta$ multiplies the unit particle-displacement vector along the ray, with positive horizontal component. That vector is $(\sin\theta,-\cos\theta)$ for a downward wave and $(\sin\theta,+\cos\theta)$ for an upward wave. Stating this polarization convention is important when assigning a sign to a reflection coefficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 79](../../../paper-79-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
