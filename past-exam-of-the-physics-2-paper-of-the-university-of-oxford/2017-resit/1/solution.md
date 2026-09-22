<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

In a source-free [vacuum](../../../vacuum.md), the [Maxwell equations](../../../maxwell-equations-split.md) in [SI](../../../international-system-of-units.md) are

$$
\nabla\cdot\mathbf E=0,\qquad \nabla\cdot\mathbf B=0,\qquad
\nabla\times\mathbf E=-\frac{\partial\mathbf B}{\partial t},\qquad
\nabla\times\mathbf B=\mu_0\epsilon_0\frac{\partial\mathbf E}{\partial t},
$$

where $\epsilon_0$ and $\mu_0$ are the [vacuum permittivity](../../../vacuum-permittivity.md) and [vacuum permeability](../../../vacuum-permeability.md). Take the [curl](../../../curl.md) of the last equation, substitute [Faraday's law of induction](../../../faraday-s-law-of-induction.md), and use the [curl of the curl identity](../../../curl-of-the-curl-identity.md):

$$
\nabla\times(\nabla\times\mathbf B)
=\nabla(\nabla\cdot\mathbf B)-\nabla^2\mathbf B
=-\mu_0\epsilon_0\frac{\partial^2\mathbf B}{\partial t^2}.
$$

The zero [divergence](../../../divergence.md) therefore gives the [wave equation](../../../wave-equation-split.md)

$$
\boxed{\nabla^2\mathbf B=\frac1{c^2}\frac{\partial^2\mathbf B}{\partial t^2},\qquad c=\frac1{\sqrt{\mu_0\epsilon_0}}.}
$$

For a propagating [plane wave](../../../plane-wave.md), write $\mathbf B=\operatorname{Re}[\mathbf B_0e^{i(\mathbf k\cdot\mathbf r-\omega t)}]$. The [wave equation](../../../wave-equation-split.md) gives $\omega^2=c^2|\mathbf k|^2$, and [Gauss's law for magnetism](../../../gauss-s-law-for-magnetism.md) gives $\mathbf k\cdot\mathbf B_0=0$. Thus the oscillating [magnetic field](../../../magnetic-field-split.md) is a [transverse wave](../../../transverse-wave.md): it is perpendicular to the propagation [wavevector](../../../wavevector.md). A static background [magnetic field](../../../magnetic-field-split.md), if present, is separate from this propagating component.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2017 resit](../../2017-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
