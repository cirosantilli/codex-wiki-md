# Far-field approximation for a current loop

↑ **Parent:** [Magnetic dipole moment](magnetic-dipole-moment.md)

Far outside a localized steady source of size $a$, at distance $r\gg a$, its [multipole expansion](electric-multipole-expansion.md) starts with the [magnetic dipole moment](magnetic-dipole-moment.md) if that moment is nonzero. In [vacuum](vacuum.md), using [SI](international-system-of-units.md) units,

$$
\mathbf A_{\mathrm{dip}}(\mathbf r)=\frac{\mu_0}{4\pi}\frac{\mathbf m\times\mathbf r}{r^3},
\qquad
\mathbf B_{\mathrm{dip}}(\mathbf r)=\frac{\mu_0}{4\pi r^3}\left[3(\mathbf m\cdot\widehat{\mathbf r})\widehat{\mathbf r}-\mathbf m\right],
$$

where $\mu_0$ is the [vacuum permeability](vacuum-permeability.md), $\widehat{\mathbf r}=\mathbf r/r$, and the [magnetic field](magnetic-field.md) is the [curl](curl.md) of the [magnetic vector potential](magnetic-vector-potential.md). The [magnetic dipole field](magnetic-dipole-field.md) falls as $r^{-3}$, and the [magnetic vector potential](magnetic-vector-potential.md) as $r^{-2}$. The [localized steady-current moment identities](localized-steady-current-moment-identities.md) remove the putative $r^{-1}$ term in the [magnetic vector potential](magnetic-vector-potential.md). No [magnetic monopole](magnetic-monopole.md) is needed. If different [current loops](current-loop.md) cancel the total [magnetic dipole moment](magnetic-dipole-moment.md), a higher term of the [multipole expansion](electric-multipole-expansion.md) supplies the leading distant [magnetic field](magnetic-field.md). [Localized Current Distribution](classical-electromagnetism-by-richard-fitzpatrick/localized-current-distribution.md).

The approximation is not valid at the center of a finite [current loop](current-loop.md). For a circular [current loop](current-loop.md) of [radius](radius.md) $R$ and [electric current](electric-current.md) $I$, the exact [on-axis magnetic field of a circular current loop](on-axis-magnetic-field-of-a-circular-current-loop.md) and the distant approximation are

$$
B_z(z)=\frac{\mu_0IR^2}{2(R^2+z^2)^{3/2}},
\qquad
B_{z,\mathrm{dip}}(z)=\frac{\mu_0IR^2}{2|z|^3}.
$$

Their ratio is $B_z/B_{z,\mathrm{dip}}=(1+R^2/z^2)^{-3/2}$: at $|z|=10R$, the approximate [magnetic field](magnetic-field.md) exceeds the exact [magnetic field](magnetic-field.md) by about $1.50\%$ relative to the exact value. Near the source, retain its geometry rather than replacing it with a point source specified only by its [magnetic dipole moment](magnetic-dipole-moment.md).

## ↑ Ancestors (6)

1. [Magnetic dipole moment](magnetic-dipole-moment.md)
2. [Magnetic vector potential](magnetic-vector-potential.md)
3. [Electromagnetism](electromagnetism-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)
