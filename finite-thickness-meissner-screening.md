# Finite-thickness Meissner screening

↑ **Parent:** [Meissner state](meissner-state.md)

To isolate finite size from [quantum vortex](quantum-vortex.md) penetration, keep the same weak-field [London equations](london-equations.md) but replace the [half-space](half-space.md) by an infinite slab $-d/2\leq z\leq d/2$. Put equal tangential [magnetic fields](magnetic-field.md) $B_0\widehat{\mathbf x}$ at its two faces. With $z=0$ now at the slab center, the even solution and its signed [current density](current-density.md) are

$$
B_x(z)=B_0\frac{\cosh(z/\lambda_L)}{\cosh(d/(2\lambda_L))},\qquad
J_y(z)=\frac{B_0}{\mu_0\lambda_L}\frac{\sinh(z/\lambda_L)}{\cosh(d/(2\lambda_L))}.
$$

The [hyperbolic cosine](hyperbolic-cosine.md) profile has equal boundary values, while the [electric currents](electric-current.md) on the two sides have opposite signs. In particular,

$$
\frac{B_x(0)}{B_0}=\frac{1}{\cosh(d/(2\lambda_L))},\qquad
\frac{\overline B_x}{B_0}=\frac{1}{dB_0}\int_{-d/2}^{d/2}B_x(z)\,dz
=\frac{2\lambda_L}{d}\tanh\!\left(\frac{d}{2\lambda_L}\right).
$$

For the stipulated thickness $d=2\lambda_L$, the center retains about $0.648B_0$ and the mean is about $0.762B_0$, even though this is a [Meissner state](meissner-state.md). For $d\gg\lambda_L$, the center [magnetic field](magnetic-field.md) is exponentially small and the mean is about $2\lambda_LB_0/d$, reflecting the two surface layers. For $d\ll\lambda_L$, the mean tends to $B_0$: little screening is possible across such a short distance. These are analytic model examples, not material measurements. Real finite objects also need their [demagnetizing field](demagnetizing-field.md) and edge geometry accounted for; the slab calculation only isolates the effect of thickness.

## ↑ Ancestors (8)

1. [Meissner state](meissner-state.md)
2. [Meissner effect](meissner-effect.md)
3. [London equations](london-equations.md)
4. [Magnetic field](magnetic-field.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Meissner effect](meissner-effect.md)
- [Planar London screening](planar-london-screening.md)
