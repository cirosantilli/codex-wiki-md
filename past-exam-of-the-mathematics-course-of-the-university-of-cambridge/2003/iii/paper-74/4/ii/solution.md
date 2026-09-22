<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Interpret the surface delta as $\delta_s=|\nabla F|\delta(F)$, so integration against it gives a surface integral. If $F$ is signed distance, this equals the notation $\delta(F)$ directly. This convention is needed because an arbitrary rescaling of the level-set function must not change the physical source.

Define the volume flux $\mathcal V(t)=\int_S V_n\,dS$ and total [pressure](../../../../../../pressure.md) [force](../../../../../../force.md) $f(t)=\int_S pn\,dS$. Here $\mathcal V$ is the rate of change of body volume, not the volume itself. The surface [acoustic monopole](../../../../../../acoustic-monopole.md) contributes, in the [acoustic compact-source approximation](../../../../../../acoustic-compact-source-approximation.md),

$$
\rho'_M=\partial_t\frac{\rho_0\mathcal V(\tau)}{4\pi c_0^2r}
=\frac{\rho_0\dot{\mathcal V}(\tau)}{4\pi c_0^2r}.
$$

The surface [acoustic dipole](../../../../../../acoustic-dipole.md) contributes

$$
\rho'_D=-\nabla_x\cdot\frac{f(\tau)}{4\pi c_0^2r}
=\frac{n\cdot\dot f(\tau)}{4\pi c_0^3r}+\frac{n\cdot f(\tau)}{4\pi c_0^2r^2}.
$$

The second term is a nonradiating near-field term and is smaller in the [acoustic far field](../../../../../../acoustic-far-field.md). Writing $\mathcal F(t)=x\cdot f(t)$ with the observation point fixed, the leading augmentation is therefore

$$
\boxed{\rho'_{\rm surf}\sim\frac{\rho_0\dot{\mathcal V}(\tau)}{4\pi rc_0^2}
+\frac{\dot{\mathcal F}(\tau)}{4\pi r^2c_0^3}}.
$$

**The printed dipole coefficient is missing a factor $1/c_0$.** The extra inverse speed follows from differentiating $\tau=t-r/c_0$, and is required dimensionally: the printed expression with $c_0^2$ has the units of density times speed. This corrected [acoustic loading noise](../../../../../../acoustic-loading-noise.md) term also agrees with the [far-field acoustic force and stress moments](../../../../../../far-field-acoustic-force-and-stress-moments.md). The monopole coefficient is unchanged.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
