# Point-mass tidal stretching and squeezing

↑ **Parent:** [Tidal tensor](tidal-tensor.md)

For a source [point mass](point-mass.md) $M$ at the origin, let $\mathbf R=R\mathbf n$, where $\mathbf n$ is an outward [unit vector](unit-vector.md), and let $\mu=GM$ be the source's [standard gravitational parameter](standard-gravitational-parameter.md). Differentiating $g_i=-\mu R_i/R^3$ gives the [tidal tensor](tidal-tensor.md)

$$
T_{ij}=\frac{\mu}{R^3}(3n_i n_j-\delta_{ij}),\qquad T=\frac{\mu}{R^3}(3\mathbf n\mathbf n^{\mathsf T}-I),
$$

where $\delta_{ij}$ is the [Kronecker delta](kronecker-delta.md) and $I$ is the [identity matrix](identity-matrix.md). In an [orthonormal basis](orthonormal-basis.md) with first axis radial, the [tidal tensor](tidal-tensor.md) is

$$
T=\frac{\mu}{R^3}\begin{pmatrix}2&0&0\\0&-1&0\\0&0&-1\end{pmatrix}.
$$

The radial [eigenvalue](eigenvalue.md) $2\mu/R^3$ separates nearby freely falling [test particles](test-particle.md); the two transverse [eigenvalues](eigenvalue.md) $-\mu/R^3$ bring them together. The farther radial [test particle](test-particle.md) falls inward less rapidly, so its [acceleration](acceleration.md) relative to the nearer one points outward. Transverse [gravitational accelerations](gravitational-acceleration.md) converge toward the source. Thus an initially resting small cloud stretches radially and squeezes in both transverse directions. These are instantaneous relative [accelerations](acceleration.md); the subsequent shape also depends on initial [velocities](velocity.md) and the changing [tidal tensor](tidal-tensor.md) along the cloud's [free fall](free-fall.md).

Outside the source, the [matrix trace](matrix-trace.md) is $2\mu/R^3-\mu/R^3-\mu/R^3=0$. This matches $\operatorname{tr}T=-\nabla^2\Phi=0$ in a region with zero [mass density](density.md), by the [Poisson equation for Newtonian gravity](poisson-equation-for-newtonian-gravity.md). Zero [matrix trace](matrix-trace.md) means no leading change of a small initially resting cloud's [volume](volume.md) at order $t^2$, not that each separation stays fixed. Inside matter, the same sign convention gives $\operatorname{tr}T=-4\pi G\rho$ instead.

## ↑ Ancestors (7)

1. [Tidal tensor](tidal-tensor.md)
2. [Newtonian gravitational field](newtonian-gravitational-field.md)
3. [Newton's law of universal gravitation](newton-s-law-of-universal-gravitation.md)
4. [Classical mechanics](classical-mechanics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Tidal force](tidal-force.md)
