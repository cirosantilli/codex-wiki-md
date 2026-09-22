# Material surface element evolution

↑ **Parent:** [Material surface element](material-surface-element.md)

Parameterize a [material surface](material-surface.md) by fixed particle labels $a,b$, with tangents $\mathbf a=\partial_a\mathbf x$, $\mathbf b=\partial_b\mathbf x$. The [material derivative](material-derivative.md) gives $D\mathbf a/Dt=(\nabla\mathbf u)\mathbf a$ and similarly for $\mathbf b$. Differentiate $d\mathbf S=(\mathbf a\times\mathbf b)\,da\,db$ and use the [cross product](cross-product.md) identity

$$
(A\mathbf a)\times\mathbf b+\mathbf a\times(A\mathbf b)
=[(\operatorname{tr}A)\mathsf I-A^{\mathsf T}](\mathbf a\times\mathbf b).
$$

This proves the displayed oriented-area evolution law, with $(\nabla\mathbf u)_{ij}=\partial_ju_i$. It allows both area change and rotation; even [incompressible flow](incompressible-flow.md) need not preserve the magnitude of a material area element.

## ↑ Ancestors (6)

1. [Material surface element](material-surface-element.md)
2. [Material surface](material-surface.md)
3. [Fluid mechanics](fluid-mechanics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Conservation of vorticity flux through a material surface](conservation-of-vorticity-flux-through-a-material-surface.md)
- [Material magnetic-flux transport theorem](material-magnetic-flux-transport-theorem.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2017/4/b/solution.md)
- [Solution](past-exam-of-the-astrophysical-fluid-dynamics-course-of-the-university-of-cambridge/2022/section-a/3/solution.md)
