# Saturated isotropic magnetostrictive strain

↑ **Parent:** [Magnetostriction](magnetostriction.md)

Consider a mechanically free [isotropic](isotropy.md) model of a saturated [ferromagnet](ferromagnet.md), at fixed [temperature](temperature-split.md) and fixed magnitude of [magnetization](magnetization.md). Let $\mathbf m=\mathbf M/M_s$ be a [unit vector](unit-vector.md), where $M_s$ is the [saturation magnetization](saturation-magnetization.md). The [magnetostrictive strain](magnetostrictive-strain.md) is an [infinitesimal strain tensor](infinitesimal-strain-tensor.md), measured relative to a reference with randomly oriented [magnetic domains](magnetic-domain.md). This reference convention matters: it sets the orientational average of the preferred [strain](strain.md) to zero. Define $\lambda_s$, the [saturation magnetostriction](saturation-magnetostriction.md), as the longitudinal relative length change in this model.

[Rotational symmetry](rotational-symmetry.md) permits a symmetric second-rank [tensor](tensor.md) made from $\mathbf m$ of the form $a\delta_{ij}+b m_i m_j$, where $\delta_{ij}$ is the [Kronecker delta](kronecker-delta.md). If we restrict attention to a change of shape with zero first-order [volume](volume.md) change, its [trace](matrix-trace.md) gives $3a+b=0$. Requiring the longitudinal component to equal $\lambda_s$ gives $a+b=\lambda_s$. Hence

$$
\varepsilon^{\rm mag}_{ij}=\frac{3\lambda_s}{2}\left(m_i m_j-\frac{\delta_{ij}}{3}\right),\qquad
\varepsilon_\parallel=\lambda_s,\qquad
\varepsilon_\perp=-\frac{\lambda_s}{2}.
$$

The [tensor product](tensor-product.md) $\mathbf m\otimes\mathbf m$ is symmetric and unchanged under $\mathbf m\mapsto-\mathbf m$. It uses two copies of the magnetic direction, so the third-rank [isotropic tensor](isotropic-tensor.md) obstruction in [isotropic linear magnetostriction vanishes](isotropic-linear-magnetostriction-vanishes.md) does not apply. More generally, a small-[magnetization](magnetization.md) expansion can contain $a M^2\delta_{ij}+b M_iM_j$; [isotropy](isotropy.md) alone does not require its [trace](matrix-trace.md) to vanish. The displayed saturated formula isolates the volume-preserving orientational contribution, rather than asserting that every material has zero [volume magnetostriction](volume-magnetostriction.md).

Along a measuring [unit vector](unit-vector.md) $\mathbf n$, with $\mathbf n\cdot\mathbf m=\cos\theta$, the fractional length change is

$$
\frac{\Delta L_{\mathbf n}}{L}=n_i\varepsilon^{\rm mag}_{ij}n_j
=\frac{\lambda_s}{2}(3\cos^2\theta-1).
$$

For a stipulated $\lambda_s=20\times10^{-6}$ and reference length $L=100\,\mathrm{mm}$, alignment gives $+2\,\mathrm{\mu m}$ and a perpendicular orientation gives $-1\,\mathrm{\mu m}$. Rotating from perpendicular to parallel therefore changes the length by $3\,\mathrm{\mu m}$, even though the saturated longitudinal value relative to the random reference is $2\,\mathrm{\mu m}$. A negative $\lambda_s$ reverses these elongation and contraction signs.

The [eigenvalues](eigenvalue.md) of this [infinitesimal strain tensor](infinitesimal-strain-tensor.md) are $\lambda_s,-\lambda_s/2,-\lambda_s/2$, so $\Delta V/V=\operatorname{tr}\varepsilon^{\rm mag}=0$ to first order. This is not exact finite [incompressibility](incompressible-flow.md): using the illustrative [deformation gradient](deformation-gradient.md) $F=I+\varepsilon^{\rm mag}$ gives

$$
\det F=(1+\lambda_s)(1-\lambda_s/2)^2
=1-\frac34\lambda_s^2+\frac14\lambda_s^3.
$$

A finite-deformation law would need higher-order corrections if exact [volume](volume.md) conservation were required.

**Table of contents**

- [Magnetic reversal and domain averaging](magnetic-reversal-and-domain-averaging.md)

## ↑ Ancestors (6)

1. [Magnetostriction](magnetostriction.md)
2. [Elasticity (physics)](elasticity-physics-split.md)
3. [Continuum mechanics](continuum-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Magnetic reversal and domain averaging](magnetic-reversal-and-domain-averaging.md)
- [Magnetostriction](magnetostriction.md)
- [Quadratic magnetostriction and frequency doubling](quadratic-magnetostriction-and-frequency-doubling.md)
- [Saturation magnetostriction](saturation-magnetostriction.md)
