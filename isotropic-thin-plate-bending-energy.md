# Isotropic thin-plate bending energy

↑ **Parent:** [Elastic plate](elastic-plate.md)

For a homogeneous isotropic plate of thickness $h$, [Young's modulus](young-s-modulus.md) $E$ and [Poisson's ratio](poisson-s-ratio.md) $\nu$, the bending stiffness is $D=Eh^3/[12(1-\nu^2)]$. Its quadratic bending energy is

$$
\mathcal U[w]=\frac D2\int_\Omega
[w_{xx}^2+2\nu w_{xx}w_{yy}+w_{yy}^2+2(1-\nu)w_{xy}^2],dx,dy.
$$

It follows by integrating the [strain energy density](strain-energy-density.md) $\tfrac12\tau_{ij}e_{ij}$ through the thickness: linear bending strains are proportional to $z$, and $\int_{-h/2}^{h/2}z^2\,dz=h^3/12$. Taking a [first variation](first-variation.md) and integrating by parts twice gives $D\Delta^2w=0$ without applied transverse load. Clamped boundary variations have both zero value and zero normal derivative.

**Table of contents**

- [Free straight edge of an isotropic bending plate](free-straight-edge-of-an-isotropic-bending-plate.md)

## ↑ Ancestors (7)

1. [Elastic plate](elastic-plate.md)
2. [Linear elasticity](linear-elasticity.md)
3. [Elasticity (physics)](elasticity-physics-split.md)
4. [Continuum mechanics](continuum-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Free straight edge of an isotropic bending plate](free-straight-edge-of-an-isotropic-bending-plate.md)
