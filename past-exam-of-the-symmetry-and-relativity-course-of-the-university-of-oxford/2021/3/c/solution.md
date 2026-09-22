<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let starred quantities denote the [capacitor](../../../../capacitor.md)'s rest [inertial frame](../../../../inertial-frame.md), $u_0=\epsilon_0E^2/2$, $\beta=v/c$, and $\gamma=(1-\beta^2)^{-1/2}$. Work in the uniform interplate region of an ideal [parallel-plate capacitor](../../../../parallel-plate-capacitor.md), neglecting its [fringing field of a capacitor](../../../../fringing-field-of-a-capacitor.md). To transform from that rest [inertial frame](../../../../inertial-frame.md) to a laboratory in which the [capacitor](../../../../capacitor.md) moves along $+x$, use the positive-sign [Lorentz transformation](../../../../lorentz-transformation.md)

$$
L=\begin{pmatrix}\gamma&\gamma\beta&0&0\\\gamma\beta&\gamma&0&0\\0&0&1&0\\0&0&0&1\end{pmatrix},\qquad
F=LF_*L^T,\qquad T=LT_*L^T.
$$

For a purely electric field, the spatial block of the [electromagnetic stress-energy tensor](../../../../electromagnetic-stress-energy-tensor.md) is

$$
T_*^{ij}=u_0\delta_{ij}-\epsilon_0E_iE_j.
$$

This is the negative of the [Maxwell stress tensor](../../../../maxwell-stress-tensor.md): it has $-u_0$ along the [electric field](../../../../electric-field-split.md) and $+u_0$ perpendicular to it. The [stress contribution to energy transport in a moving capacitor](../../../../stress-contribution-to-energy-transport-in-a-moving-capacitor.md) is essential to the [Lorentz transformation](../../../../lorentz-transformation.md) of the [energy](../../../../energy-split.md) density and flux.

**Plates parallel to $xy$.** Choose $\mathbf E_*=E\hat{\mathbf z}$ and $\mathbf B_*=0$. The [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) and [electromagnetic stress-energy tensor](../../../../electromagnetic-stress-energy-tensor.md) are

$$
F_*^{\mu\nu}=\begin{pmatrix}
0&0&0&E/c\\0&0&0&0\\0&0&0&0\\-E/c&0&0&0
\end{pmatrix},\qquad
T_*^{\mu\nu}=u_0\operatorname{diag}(1,1,1,-1).
$$

The transformed nonzero independent [electromagnetic field tensor](../../../../electromagnetic-field-tensor.md) components are $F^{03}=\gamma E/c$ and $F^{13}=\gamma\beta E/c$. Thus $\mathbf E=\gamma E\hat{\mathbf z}$ and $\mathbf B=-\gamma vE\hat{\mathbf y}/c^2$, consistent with $\mathbf B=\mathbf v\times\mathbf E/c^2$. Transforming the [electromagnetic stress-energy tensor](../../../../electromagnetic-stress-energy-tensor.md) gives

$$
\boxed{T^{\mu\nu}=u_0\begin{pmatrix}
\gamma^2(1+\beta^2)&2\gamma^2\beta&0&0\\
2\gamma^2\beta&\gamma^2(1+\beta^2)&0&0\\
0&0&1&0\\0&0&0&-1
\end{pmatrix}.}
$$

In particular, the laboratory [Poynting vector](../../../../poynting-vector.md) is $\mathbf S=2u_0\gamma^2v\hat{\mathbf x}$, and the [electromagnetic energy density](../../../../electromagnetic-energy-density.md) is $u=u_0\gamma^2(1+\beta^2)$. The ratio $S_x/u=2v/(1+\beta^2)$ is subluminal for $v<c$, but differs from the [capacitor](../../../../capacitor.md)'s [velocity](../../../../velocity.md). The difference from a simple convective flux is

$$
S_x-uv=u_0v.
$$

The extra term is $vT_*^{xx}$, the rest-frame stress multiplied by the [velocity](../../../../velocity.md). This shows why treating stored field [energy](../../../../energy-split.md) as an unstressed parcel moving rigidly with the plates misses part of the [energy](../../../../energy-split.md) transport.

**Plates parallel to $yz$.** Now $\mathbf E_*=E\hat{\mathbf x}$. The rest [tensors](../../../../tensor.md) are

$$
F_*^{\mu\nu}=\begin{pmatrix}
0&E/c&0&0\\-E/c&0&0&0\\0&0&0&0\\0&0&0&0
\end{pmatrix},\qquad
T_*^{\mu\nu}=u_0\operatorname{diag}(1,-1,1,1).
$$

The [electric field](../../../../electric-field-split.md) is parallel to the [Lorentz boost](../../../../lorentz-boost.md), so $F^{01}=E/c$ remains unchanged and $\mathbf B=0$. The cancellation between $T_*^{00}$ and $T_*^{11}$ gives

$$
\boxed{T^{\mu\nu}=u_0\operatorname{diag}(1,-1,1,1),\qquad
u=u_0,\qquad \mathbf S=0.}
$$

There is no [Poynting flux](../../../../poynting-flux.md) in the ideal interior in this orientation, although the region containing the [electric field](../../../../electric-field-split.md) moves. The longitudinal negative stress contribution cancels the convective term: $S_x=\gamma^2v(u_0+T_*^{xx})=0$. Field [energy](../../../../energy-split.md) is removed at the receding boundary and supplied at the advancing boundary by [work](../../../../work.md) on the charged plates; it need not flow through the interior to accompany the moving region. At edges, omitted [fringing fields](../../../../fringing-field-of-a-capacitor.md) provide additional local structure.

For a finite idealized interplate rest [volume](../../../../volume.md) $V_0$, [length contraction](../../../../length-contraction.md) gives $V=V_0/\gamma$. The field-only integrated laboratory [energies](../../../../energy-split.md) would consequently be $U_{xy}=\gamma(1+\beta^2)U_0$ and $U_{yz}=U_0/\gamma$, with $U_0=u_0V_0$. Their different transformation laws are not paradoxical: the field alone is not a closed system. Include the plates and the supports holding them apart, whose mechanical stresses balance the [Maxwell stress tensor](../../../../maxwell-stress-tensor.md). The total closed-system [four-momentum](../../../../four-momentum.md) then has the ordinary [Lorentz transformation](../../../../lorentz-transformation.md) law. This is the same distinction between a subsystem and a conserved whole that appears in [b](../../1/b.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the symmetry and relativity course of the University of Oxford](../../../split.md)
5. [Symmetry and relativity course of the University of Oxford](../../../../symmetry-and-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
