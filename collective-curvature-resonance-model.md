# Collective-curvature resonance model

↑ **Parent:** [Nuclear magnetic resonance fingerprint of superfluid helium-3](nuclear-magnetic-resonance-fingerprint-of-superfluid-helium-3.md)

Consider an original scalar response model for a small collective [angle](angle.md) $u$. Stipulate effective inertia $I>0$, restoring curvature $K\geq0$, [damping](damping.md) rate $\Gamma>0$, and a drive torque $\tau_0\cos\omega t$:

$$
I\ddot u+2I\Gamma\dot u+(I\omega_L^2+K)u=\tau_0\cos\omega t.
$$

The undamped resonance scale is $\omega_0=\sqrt{\omega_L^2+\Omega^2}$, where $\Omega^2=K/I$. This illustrates the role of an additional collective restoring energy. It is not the full coupled spin dynamics of either helium phase, and its parameters are not fitted to historical observations.

The steady response and mean absorbed [power](power.md) follow directly:

$$
\chi(\omega)=\frac{1/I}{\omega_0^2-\omega^2-2i\Gamma\omega},\qquad
\overline P=\frac{\tau_0^2\omega}{2}\operatorname{Im}\chi(\omega)
=\frac{\tau_0^2\Gamma\omega^2/I}{(\omega_0^2-\omega^2)^2+4\Gamma^2\omega^2}.
$$

With constant damping, differentiating this last expression places its positive-frequency maximum exactly at $\omega_0$. Setting chosen $\Omega=1$ and $\omega_L=2$ moves the peak from $2$ to $\sqrt5\simeq2.236$, about $11.8\%$. At $\omega_L=10$ the same curvature moves it only to $\sqrt{101}\simeq10.050$, about $0.50\%$. At large $\omega_L$, the shift is $\Omega^2/(2\omega_L)$ to leading order. A smaller shift at larger field therefore need not mean that the restoring curvature vanished.

<a id="image-angular-pairing-structure-and-a-chosen-collective-resonance-response"></a>
![](helium-three-gap-symmetry-and-collective-resonance.png)

**[Figure 9](#image-angular-pairing-structure-and-a-chosen-collective-resonance-response). Angular pairing structure and a chosen collective resonance response**. Original calculations, not measured helium-3 data. Left: meridional cuts of the two stipulated gap matrices, normalized by their common maximum gap. Center and right: the scalar response model with chosen $\Omega=1$ and $\Gamma=0.08$; the absorption plot uses $\omega_L=2$ and unit peak normalization. The scalar model does not identify a phase without the experimental geometry and the full spin response.

## ↑ Ancestors (7)

1. [Nuclear magnetic resonance fingerprint of superfluid helium-3](nuclear-magnetic-resonance-fingerprint-of-superfluid-helium-3.md)
2. [Helium-3 superfluidity](helium-3-superfluidity.md)
3. [Superfluidity](superfluidity.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)
