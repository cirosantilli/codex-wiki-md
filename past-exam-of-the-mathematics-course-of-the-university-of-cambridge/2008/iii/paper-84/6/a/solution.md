<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use pi-normalized [kinematic plume fluxes](../../../../../../kinematic-plume-fluxes.md): physical volume, momentum and buoyancy fluxes are $\pi Q$, $\pi M$ and $\pi F$. For a [top-hat plume model](../../../../../../top-hat-plume-model.md) in a homogeneous ambient, constant [entrainment coefficient](../../../../../../entrainment-coefficient.md) $\alpha$ gives

$$
\frac{dQ}{dz}=2\alpha\sqrt M,
\qquad \frac{dM}{dz}=\frac{FQ}{M},
\qquad \frac{dF}{dz}=0.
$$

Eliminating height between the first two equations yields $d(M^{5/2})/dQ=5FQ/(4\alpha)$. Hence the [plume flux-balance invariant](../../../../../../plume-flux-balance-invariant.md) is $M^{5/2}-5FQ^2/(8\alpha)$. [Pure plume balance](../../../../../../pure-plume-balance.md) means that this invariant vanishes, including at a finite-volume source:

$$
\boxed{M_s^{5/2}=\frac{5F_sQ_s^2}{8\alpha}.}
$$

It does not mean that $Q_s$ and $M_s$ must individually be zero. The balanced solution has a [plume virtual origin](../../../../../../plume-virtual-origin.md) below the physical source:

$$
Q(z)=C F_s^{1/3}(z+z_v)^{5/3},
\quad M(z)=\left(\frac{9\alpha F_s}{10}\right)^{2/3}(z+z_v)^{4/3},
\quad C=\frac{6\alpha}{5}\left(\frac{9\alpha}{10}\right)^{1/3},
$$

where $z_v=[Q_s/(CF_s^{1/3})]^{3/5}>0$. For given nonzero source fluxes, the displayed balance is a compatibility condition; they cannot be chosen independently and still describe an exactly balanced source.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [6](../../6.md)
3. [Paper 84](../../../paper-84-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
