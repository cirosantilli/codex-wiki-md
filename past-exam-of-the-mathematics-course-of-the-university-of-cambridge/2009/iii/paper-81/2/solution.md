<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $\omega=kc$, $q=k(1+i)$, and $E=e^{qL}$. The local [resistive-force theory](../../../../../resistive-force-theory.md) force per unit length on the filament is

$$
\mathbf f=-\mu K_N\left[\mathbf v+(\gamma-1)(\mathbf v\cdot\mathbf t)\mathbf t\right],\qquad \gamma=K_T/K_N,
$$

where $\mathbf t=(X_s,Y_s)$ is the unit tangent and $\mathbf v=(X_t-U,Y_t-V)$ the material [velocity](../../../../../velocity.md) relative to the fluid. Inextensibility gives $X_s=(1-Y_s^2)^{1/2}=1-Y_s^2/2+\cdots$. With $X(0,t)=0$, $X_t=-\int_0^sY_sY_{st}\,ds'+\cdots$ is second order and has zero time average for a periodic prescribed stroke. The actual small-slope condition is $k|H|e^{kL}\ll1$ for fixed $kL$; $kH\ll1$ alone is not uniform when $kL$ grows.

At first order, the transverse [force](../../../../../force.md) is $f_y=-\mu K_N(Y_t-V)$. Adding the spherical-head [drag force](../../../../../drag-physics.md) $\mu K_NL\delta V$ and imposing zero total [force](../../../../../force.md) gives

$$
\boxed{V(t)=\frac1{L(1+\delta)}\int_0^LY_t(s,t)ds
=\frac{cH}{2L(1+\delta)}\left\{e^{kL}[\sin(kL-\omega t)-\cos(kL-\omega t)]+\sin\omega t+\cos\omega t\right\}.}
$$

Equivalently $V(t)=\operatorname{Re}[-i\omega H(E-1)e^{-i\omega t}/(qL(1+\delta))]$. This form is useful for the subsequent time averages.

At second order, the axial [resistive-force theory](../../../../../resistive-force-theory.md) force is

$$
f_x=\mu K_N\left[\gamma(U-X_t)+(1-\gamma)Y_s(Y_t-V)\right]+\cdots.
$$

Adding the head [drag force](../../../../../drag-physics.md) gives the [head-drag correction to planar flagellar propulsion](../../../../../head-drag-correction-to-planar-flagellar-propulsion.md):

$$
L(\delta+\gamma)\overline U=-(1-\gamma)\overline{\int_0^LY_s(Y_t-V)ds},
$$

since $\overline{X_t}=0$. Directly, $Y_s=kHe^{ks}(\cos\vartheta-\sin\vartheta)$ and $Y_t=kcHe^{ks}\sin\vartheta$, with $\vartheta=k(s-ct)$. Hence

$$
\overline{\int_0^LY_sY_tds}=-\frac{ckH^2}{4}(e^{2kL}-1).
$$

Also $\int_0^LY_sds=Y(L,t)-Y(0,t)$, whose complex amplitude is $H(E-1)$. Using $\overline{\operatorname{Re}(ae^{-i\omega t})\operatorname{Re}(be^{-i\omega t})}=\operatorname{Re}(a\overline b)/2$, together with $\operatorname{Re}(-i\omega/q)=-c/2$, gives

$$
\overline{V\int_0^LY_sds}=-\frac{cH^2|E-1|^2}{4L(1+\delta)}.
$$

As $|E-1|^2=e^{2kL}-2e^{kL}\cos kL+1$, the requested mean speed follows:

$$
\boxed{\overline U=\frac{ck^2H^2}{4kL}\frac{1-\gamma}{\delta+\gamma}\left[e^{2kL}-1-\frac{e^{2kL}-2e^{kL}\cos kL+1}{(1+\delta)kL}\right]+o(H^2).}
$$

Anisotropic resistance is essential: $\gamma=1$ removes propulsion at this order. The mean motion is opposite to the direction of wave propagation when the bracket is positive, since the head's axial [velocity](../../../../../velocity.md) is $-U$.

For the [basal bending moment of a planar flagellum](../../../../../basal-bending-moment-of-a-planar-flagellum.md), take positive moment to be the positive out-of-plane [torque](../../../../../torque.md) exerted on the distal filament at its base. The leading hydrodynamic [torque](../../../../../torque.md) on that filament is $-\mu K_N\int_0^Ls(Y_t-V)ds$, so balance requires

$$
\boxed{M_0(t)=\mu K_N\left[\int_0^LsY_t(s,t)ds-\frac{L^2}{2}V(t)\right].}
$$

An explicit unsimplified time-dependent answer is

$$
\boxed{M_0(t)=\mu K_N\operatorname{Re}\left[-i\omega H\left\{\frac{E(qL-1)+1}{q^2}-\frac{L(E-1)}{2q(1+\delta)}\right\}e^{-i\omega t}\right].}
$$

The first term follows from $\int_0^Lse^{qs}ds=[E(qL-1)+1]/q^2$. This is the total internal [bending moment](../../../../../bending-moment.md) required by the hydrodynamic load. It equals the contractile moment when passive elasticity is neglected. If a specified passive moment $M_{\mathrm{pass}}$ also acts, the required active moment is $M_0-M_{\mathrm{pass}}$; no elastic modulus is supplied here.

**The prescribed base coordinate needs a geometrical qualification.** Literally, a coordinate measured from the attachment point must have $Y(0,t)=0$, whereas the printed waveform has $Y(0,t)=H\cos\omega t$. The preceding calculation reproduces the printed speed by treating that waveform as the prescribed coordinate, including its moving transverse offset. If the intention is instead a fixed attachment at the origin, replace it by $\widetilde Y=H[e^{ks}\cos k(s-ct)-\cos\omega t]$. Then

$$
\widetilde V=V+\frac{\omega H\sin\omega t}{1+\delta},\qquad
\overline{\widetilde U}=\overline U-\frac{(1-\gamma)\delta\,\omega H^2e^{kL}\sin kL}{2L(\delta+\gamma)(1+\delta)}.
$$

These follow by replacing $Y_t$ with $Y_t-Y_t(0,t)$ in the same [force balance](../../../../../force-balance.md). The basal moment likewise uses $\widetilde Y_t$ and $\widetilde V$. Thus the printed kinematics and its claim that the origin is the actual attachment cannot both be imposed without this correction.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
