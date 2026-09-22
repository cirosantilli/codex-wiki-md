<h1 id="38a/solution">Solution</h1>

↑ **Parent:** [38A](../38a.md)

Taking the [divergence](../../../../../divergence.md) and [curl](../../../../../curl.md) of the elastic equation gives

$$
(\nabla\cdot u)_{tt}=c_P^2\Delta(\nabla\cdot u),\qquad
(\nabla\times u)_{tt}=c_S^2\Delta(\nabla\times u),
\qquad
\boxed{c_P^2=(\lambda+2\mu)/\rho,\quad c_S^2=\mu/\rho}.
$$

Substitution of the [plane wave](../../../../../plane-wave.md) gives $\omega^2A=c_P^2k(k\cdot A)-c_S^2k\times(k\times A)$. Resolve $A$ parallel and perpendicular to $k$. A [P wave](../../../../../p-wave.md) has longitudinal polarization and $\omega^2=c_P^2|k|^2$; an [S wave](../../../../../s-wave.md) has transverse polarization and $\omega^2=c_S^2|k|^2$, with two transverse polarizations.

For the [Rayleigh wave](../../../../../rayleigh-wave.md), take displacement potentials in the $x,z$ plane,

$$
u_x=\phi_x-\psi_z,\quad u_z=\phi_z+\psi_x,\qquad
\phi=Ae^{k\alpha z}e^{ik(x-ct)},\quad
\psi=Be^{k\beta z}e^{ik(x-ct)},
$$

where $\alpha=\sqrt{1-c^2/c_P^2}$, $\beta=\sqrt{1-c^2/c_S^2}$. For $0<c<c_S<c_P$, both waves decay into $z<0$. These are an evanescent longitudinal wave and an evanescent vertically polarized shear wave. At $z=0$, the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md) $\sigma_{ij}=\lambda(\nabla\cdot u)\delta_{ij}+\mu(u_{i,j}+u_{j,i})$ gives

$$
\sigma_{xz}=\mu k^2[2i\alpha A-(1+\beta^2)B]e^{ik(x-ct)},\qquad
\sigma_{zz}=\mu k^2[(1+\beta^2)A+2i\beta B]e^{ik(x-ct)}.
$$

The third traction component is already zero. The two remaining stress-free conditions have a nonzero solution $(A,B)$ exactly when their determinant vanishes:

$$
\boxed{(1+\beta^2)^2=4\alpha\beta}.
$$

Substituting $\alpha,\beta$ gives the required Rayleigh wave equation. The nonzero subsonic root supplies a self-sustained surface wave; no existence proof for that root is required. The formal zero-speed root is degenerate and does not describe a propagating wave.

## ↑ Ancestors (10)

1. [38A](../38a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
