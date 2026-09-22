<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume the relative [permittivity](../../../../../../../permittivity.md) is real and the field decays sufficiently at transverse infinity, or impose boundary conditions with zero transverse flux. Then $L(x)$ is self-adjoint on its transverse domain by [integration by parts](../../../../../../../integration-by-parts.md). The scalar [parabolic wave equation](../../../../../../../parabolic-wave-equation.md) gives

$$
\frac{d}{dx}\int_{\mathbb R^2}|U|^2\,dy\,dz
=i\int_{\mathbb R^2}\left[U^*LU-U(LU)^*\right]dy\,dz=0.
$$

This is [norm conservation for the scalar parabolic wave equation](../../../../../../../norm-conservation-for-the-scalar-parabolic-wave-equation.md). It remains true when $L$ depends explicitly on $x$; its instantaneous self-adjointness suffices. Equivalently, the local balance is

$$
\partial_x|U|^2+\nabla_\perp\cdot\left[\frac1k\operatorname{Im}(U^*\nabla_\perp U)\right]=0.
$$

Since $|E|=|U|$, the invariant can also be written

$$
\boxed{\mathcal N(x)=\int|E(x,y,z)|^2dy\,dz=\text{constant}.}
$$

For a unit transverse polarization in a fixed reference medium with impedance $Z_0=\sqrt{\mu_0/\epsilon_0}$, the leading forward paraxial [Poynting vector](../../../../../../../poynting-vector.md) has $S_x\simeq |E|^2/(2Z_0)$. Thus the scalar model conserves its leading reference-normalized power $P_0=\mathcal N/(2Z_0)$. This is the intended consequence of the Hermitian-operator hint. Complex [permittivity](../../../../../../../permittivity.md) would add absorption or gain and invalidate this [norm](../../../../../../../norm.md) invariant.

Two qualifications are necessary for the printed physical interpretation. First, $(1,0,1)$ is neither a unit vector nor transverse to nearly axial propagation: its longitudinal electric component is as large as its transverse one. In a homogeneous source-free medium, the example $\mathbf E=(1,0,1)e^{ikx}$ satisfies the componentwise Helmholtz equation but violates $\nabla\cdot\mathbf E=0$. It therefore is not the stated near-axial electromagnetic plane wave. The same scalar calculation formally conserves $\int|\mathbf U|^2=2\mathcal N$ for that fixed vector, but does not make it a physical Maxwell field. A unit transverse polarization, for example $(0,0,1)$, is the consistent paraxial choice, with only small longitudinal corrections.

Second, for varying local refractive index $n(x)=\sqrt{\epsilon_{\rm rel}(x)}$, the quoted local plane-wave impedance relation gives $Z(x)=Z_0/n(x)$ and hence a flux proportional to $n(x)|E|^2$, not merely $|E|^2$. The scalar [norm](../../../../../../../norm.md) proof alone cannot make this exactly constant for arbitrary $n(x)$. For example a transversely uniform envelope obeying the printed parabolic equation has

$$
U(x)=U(0)\exp\left[\frac{ik}{2}\int_0^x(n(s)^2-1)\,ds\right],
$$

so its intensity is constant while the locally inferred plane-wave flux changes with $n$. This supplies a direct obstruction to the literal exact-flux claim within the supplied scalar assumptions.

The consistent physical statement follows from [Poynting theorem](../../../../../../../poynting-theorem.md): for a lossless Maxwell solution and no lateral energy leakage,

$$
\nabla\cdot\frac12\operatorname{Re}(\mathbf E\times\mathbf H^*)=0,\qquad
\boxed{\frac d{dx}\int S_x\,dy\,dz=0.}
$$

For a slowly varying transverse plane wave, the corresponding forward WKB field has [amplitude](../../../../../../../wave-amplitude.md) proportional to $n^{-1/2}$, making $n|E|^2$ constant. In one dimension this is also encoded in the exact conserved flux $(2\mu_0\omega)^{-1}\operatorname{Im}(E^*E_x)$. Thus the requested physical conservation holds for the corrected lossless Maxwell description, while the given scalar equation proves the reference-normalized paraxial invariant above. The supplied fixed longitudinal polarization and arbitrary local-impedance inference cannot be used to claim more.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 78](../../../../paper-78-split.md)
5. [Iii](../../../../split.md)
6. [2009](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
