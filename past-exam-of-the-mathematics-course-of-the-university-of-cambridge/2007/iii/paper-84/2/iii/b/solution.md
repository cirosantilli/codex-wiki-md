<h1 id="2/iii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Split the solitary-wave energy into longitudinal, transverse and interaction contributions,

$$
E=E_z+E_\perp+E_{\rm pot},\quad
E_z=\frac12\int|\psi_z|^2dV,\quad
E_\perp=\frac12\int(|\psi_x|^2+|\psi_y|^2)dV.
$$

Consider the longitudinal dilation $\psi_\lambda(x,y,z)=\psi(x,y,\lambda z)$ for $\lambda>0$. Changing variables to $Z=\lambda z$ gives

$$
E[\psi_\lambda]=\lambda E_z+\lambda^{-1}(E_\perp+E_{\rm pot}).
$$

The [renormalized momentum of a condensate](../../../../../../../renormalized-momentum-of-a-condensate.md) is unchanged: its single $z$ derivative contributes $\lambda$, cancelling the measure factor $\lambda^{-1}$. Since the wave is a critical point of $E-Up$, differentiating this admissible scaling variation at $\lambda=1$ gives

$$
0=E_z-E_\perp-E_{\rm pot}.
$$

Therefore the [longitudinal scaling identity for a condensate solitary wave](../../../../../../../longitudinal-scaling-identity-for-a-condensate-solitary-wave.md) yields

$$
\boxed{E=2E_z=\int|\partial_z\psi|^2dV}.
$$

This directional [Pohozaev identity](../../../../../../../pohozaev-identity.md) assumes the finite energy and sufficient decay to justify the dilation variation; it can equivalently be obtained with cutoffs followed by a limit. It is an identity for solitary-wave critical points, not for arbitrary localized fields.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Iii](../../iii.md)
3. [2](../../../2.md)
4. [Paper 84](../../../../paper-84-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
