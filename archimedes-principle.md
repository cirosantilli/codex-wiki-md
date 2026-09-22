# Archimedes' principle

↑ **Parent:** [Buoyancy](buoyancy.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Archimedes'_principle)

[Archimedes' principle](archimedes-principle.md) states that [buoyancy](buoyancy.md) equals the downward [gravitational weight](weight-physics.md), or weight, of the displaced [fluid](fluid.md). In a resting [fluid](fluid.md) of constant [mass density](density.md) $\rho_f$ under uniform [gravitational acceleration](gravitational-acceleration.md) $g$, its magnitude is

$$
F_b=\rho_fgV_{\mathrm{displaced}}.
$$

Here $V_{\mathrm{displaced}}$ is the [volume](volume.md) from which the body excludes the [fluid](fluid.md): the whole external [volume](volume.md) for a fully immersed solid body, and just the immersed [volume](volume.md) for a partly immersed one. The body's own [mass](mass.md) does not enter this [buoyancy](buoyancy.md) formula. [OpenStax, University Physics, §14.4: Archimedes' principle](https://openstax.org/books/university-physics-volume-1/pages/14-4-archimedes-principle-and-buoyancy)

A short proof outline for a fully immersed body is to imagine replacing it by exactly the [fluid](fluid.md) it displaces. The surrounding [hydrostatic pressure](hydrostatic-pressure.md) is unchanged. That replacement [fluid](fluid.md) is at rest, so its upward [pressure](pressure-split.md) [force](force-split.md) must balance its downward [force](force-split.md) from [gravity](gravity.md). The original body receives the same inward [pressure](pressure-split.md) [forces](force-split.md) on the same closed surface, hence the same upward [buoyancy](buoyancy.md).

Equivalently, let $\Omega$ be the displaced region, $\partial\Omega$ its closed surface and $\mathbf e_z$ the upward unit direction. The [divergence theorem](divergence-theorem.md), applied component by component to the [surface integral](surface-integral.md), and [hydrostatic pressure](hydrostatic-pressure.md) give

$$
\mathbf F_b=-\int_{\partial\Omega}p\mathbf n\,dA
=-\int_\Omega\nabla p\,dV
=\rho_fgV_{\mathrm{displaced}}\mathbf e_z.
$$

This also explains why horizontal [forces](force-split.md) cancel even for an irregular shape. A spatially constant surface [pressure](pressure-split.md) contributes zero to the closed-surface [integral](integral-split.md). If the [mass density](density.md) varies with depth, replace $\rho_fV_{\mathrm{displaced}}$ by the [mass](mass.md) $\int_\Omega\rho_f\,dV$ of the displaced [fluid](fluid.md).

The closed-surface argument assumes that the [fluid](fluid.md) applies [pressure](pressure-split.md) over the entire boundary of a fully immersed body. A body sealing against a tank bottom may have no [fluid](fluid.md) beneath it; then the lower-face [pressure](pressure-split.md) [force](force-split.md) used in the proof is absent, and a supporting contact [force](force-split.md) must be treated separately. For partial immersion, the usual [buoyancy](buoyancy.md) formula assumes the exposed surface receives the common atmospheric [pressure](pressure-split.md), neglects the much smaller [buoyancy](buoyancy.md) from the air, and neglects [surface tension](surface-tension-split.md).

For the $0.10\ \mathrm m$ [cube](cube.md) in the stipulated [water](water.md), full immersion displaces $0.001\ \mathrm{m^3}$, so $F_b=1000\times9.81\times0.001=9.81\ \mathrm N$. If its uniform [mass density](density.md) is $600\ \mathrm{kg\,m^{-3}}$, its [mass](mass.md) is $m=600\times0.001=0.600\ \mathrm{kg}$ and its downward [force](force-split.md) from [gravity](gravity.md) is $mg=5.886\ \mathrm N$. To hold it fully immersed at rest requires an additional downward [force](force-split.md)

$$
F_{\mathrm{hold}}=F_b-mg=9.81-5.886=3.924\ \mathrm N.
$$

On release from rest it initially moves upward; its eventual [floating equilibrium](floating-equilibrium.md) has a smaller displaced [volume](volume.md). A same-size [cube](cube.md) of uniform [mass density](density.md) $1200\ \mathrm{kg\,m^{-3}}$ has [mass](mass.md) $1.200\ \mathrm{kg}$ and downward [force](force-split.md) from [gravity](gravity.md) $11.772\ \mathrm N$. Full immersion still gives $9.81\ \mathrm N$ of [buoyancy](buoyancy.md), leaving an initial net downward [force](force-split.md) of $11.772-9.81=1.962\ \mathrm N$. Subsequent motion also involves [drag](drag-physics.md).

**Table of contents**

- [Floating equilibrium](floating-equilibrium.md)
  - [Metacentric height](metacentric-height.md)
  - [Vertical oscillations of a floating cylinder](vertical-oscillations-of-a-floating-cylinder.md)

## ↑ Ancestors (5)

1. [Buoyancy](buoyancy.md)
2. [Fluid mechanics](fluid-mechanics-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Archimedes' principle](archimedes-principle.md)
- [Buoyancy](buoyancy.md)
- [Floating equilibrium](floating-equilibrium.md)
- [Iceberg freeboard](iceberg-freeboard.md)
- [Melting pressure inferred from flotation and latent heats](melting-pressure-inferred-from-flotation-and-latent-heats.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/6g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-77/4/a/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2012/paper-2/section-c/c10/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2017/paper-2/section-b/b8/d/solution.md)
- [Solution](past-exam-of-the-physics-b-course-of-the-university-of-cambridge/2018/paper-1/section-a/a3/solution.md)
- [Solution](past-exam-of-the-physics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2021/section-a/3/solution.md)
- [Vertical oscillations of a floating cylinder](vertical-oscillations-of-a-floating-cylinder.md)
