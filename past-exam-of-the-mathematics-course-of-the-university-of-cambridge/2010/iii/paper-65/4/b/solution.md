<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

To connect the prescribed interfacial [drag coefficient](../../../../../../drag-coefficient.md) to the energy supply, state the lumped [interfacial power model for entrainment](../../../../../../interfacial-power-model-for-entrainment.md) explicitly:

$$
P_I=S\tau u_I=c_D\rho_lS u_I^3,\qquad \dot E_P=C_WP_I.
$$

It estimates the power transmitted by lid-driven flow to the mixing interface. Constant geometric and transfer factors are included in $c_D$ or $C_W$. It is the local stress-power interpretation required for the depth laws in this question, not an identity equating arbitrary lid shaft power to interfacial power. With the [potential energy of two-layer entrainment](../../../../../../potential-energy-of-two-layer-entrainment.md) from (a),

$$
\dot h=\frac{2C_Wc_Du_I^3}{B}.
$$

In model S, $u_I=\Omega R$ and $B$ are constant, so

$$
\boxed{\dot h=\frac{2C_Wc_D\Omega R}{\mathrm{Ri}_B},\qquad
\mathrm{Ri}_B=\frac{B}{\Omega^2R^2}.}
$$

Thus the depth increases at a constant rate proportional to the inverse [bulk Richardson number](../../../../../../bulk-richardson-number.md), with $h=h_0+2C_Wc_D\Omega R\,t/\mathrm{Ri}_B$, until the layer reaches $H$. Here the prescribed $u_I$ must be read as a characteristic speed. Literal pure [solid-body rotation](../../../../../../solid-body-rotation.md) has zero radial velocity, so the PDF's parenthetical description of $u_I$ as radial cannot simultaneously be a strict component statement and the assumption $u_I=\Omega R$.

If the phrase about lid work is taken literally as shaft power $P_{\rm lid}=\Omega\mathcal T_{\rm lid}$, the interfacial stress alone does not specify the lid torque or its energy transfer to the interface. The preceding closure is therefore a visible model assumption, not a hidden consequence of [solid-body rotation](../../../../../../solid-body-rotation.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 65](../../../paper-65-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
