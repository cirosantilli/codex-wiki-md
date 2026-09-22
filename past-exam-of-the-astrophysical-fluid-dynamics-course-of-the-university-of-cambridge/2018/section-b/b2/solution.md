<h1 id="section-b/b2/solution">Solution</h1>

↑ **Parent:** [B2](../b2.md)

**Supersonic communication.** A point source moving at speed $V>c_s$ outruns its small [acoustic waves](../../../../acoustic-wave.md). After a time $t$, the source has moved $Vt$, while a disturbance emitted at its old position has radius $c_st$. The envelope of these spherical wavefronts is the [Mach cone](../../../../mach-cone.md), with half-angle $\mu$ satisfying

$$
\boxed{\sin\mu=\frac{c_s}{V}=\frac1{\mathcal M},\qquad
\mathcal M=\frac{V}{c_s}>1.}
$$

Information is restricted to the downstream cone, so upstream gas cannot smoothly anticipate a supersonic obstacle. Finite compressions can also steepen because their characteristics converge. Such disturbances form a [shock wave](../../../../shock-wave.md), across which the fluid variables change rapidly. A perfectly uniform [supersonic flow](../../../../supersonic-flow.md) need not contain a shock: the cone expresses the communication constraint, while a disturbance or compression supplies the reason for a discontinuity.

**Conserved fluxes.** Work in the [shock frame](../../../../shock-frame.md), take velocities normal to the front, and integrate the conservation laws through a thin steady [control volume](../../../../control-volume.md) of unit area. [Mass conservation](../../../../mass-conservation.md) gives constant flux $j=\rho u$, so

$$
\boxed{\rho_2u_2=\rho_1u_1=j.}
$$

The normal [momentum](../../../../momentum-split.md) flux is the advected part $\rho u^2$ plus the pressure stress $p$. With negligible body-force impulse across the thin front,

$$
\boxed{p_2+\rho_2u_2^2=p_1+\rho_1u_1^2.}
$$

For an [ideal gas](../../../../ideal-gas-split.md) with constant [adiabatic index](../../../../heat-capacity-ratio.md) $\gamma$, the [specific internal energy](../../../../specific-internal-energy.md) is $e=p/[(\gamma-1)\rho]$. The energy flux is

$$
j\left(e+\frac12u^2\right)+pu
=j\left(h_{\rm sp}+\frac12u^2\right),
\qquad h_{\rm sp}=e+\frac p\rho=\frac{\gamma p}{(\gamma-1)\rho},
$$

where $h_{\rm sp}$ is the [specific enthalpy](../../../../specific-enthalpy.md). No radiation or other heat flux escapes in this adiabatic shock model. Conservation of the energy flux, divided by the nonzero mass flux, gives

$$
\boxed{\frac{\gamma p_2}{(\gamma-1)\rho_2}+\frac12u_2^2
=\frac{\gamma p_1}{(\gamma-1)\rho_1}+\frac12u_1^2.}
$$

These are the [Rankine-Hugoniot conditions for a perfect gas](../../../../rankine-hugoniot-conditions-for-a-perfect-gas.md). The shock is adiabatic but irreversible: its [entropy](../../../../entropy-split.md) increases, so an isentropic relation cannot be imposed across the discontinuity.

**Strong-shock compression.** Put $\chi=\rho_2/\rho_1=u_1/u_2$ and neglect $p_1$ and the upstream enthalpy compared with $\rho_1u_1^2$ and $u_1^2$. Momentum conservation gives $p_2=\rho_1u_1^2(1-1/\chi)$. Substitute this into energy conservation:

$$
\frac12=\frac{\gamma}{\gamma-1}\frac{\chi-1}{\chi^2}+\frac1{2\chi^2}.
$$

Thus

$$
\chi^2-1=\frac{2\gamma}{\gamma-1}(\chi-1),
\qquad
(\chi-1)\left(\chi+1-\frac{2\gamma}{\gamma-1}\right)=0.
$$

The root $\chi=1$ describes no shock. The compressive branch of the [Strong-shock Rankine-Hugoniot conditions](../../../../strong-shock-rankine-hugoniot-conditions.md) is

$$
\boxed{\frac{\rho_2}{\rho_1}=\frac{u_1}{u_2}
=\frac{\gamma+1}{\gamma-1}.}
$$

It also gives $p_2=2\rho_1u_1^2/(\gamma+1)$. A [monatomic gas](../../../../monatomic-gas.md) has $\gamma=5/3$, hence $\chi=4$.

**The finite slab in its initial rest frame.** Denote the shock's lab speed by $V_s$. The upstream gas is initially stationary, so $u_1=V_s$ and the downstream shock-frame speed is $u_2=V_s/4$. Transforming to the initial slab frame gives

$$
\boxed{v_2=V_s-u_2=\frac34V_s,\qquad L_2=\frac L4.}
$$

This is [planar shock compression of a finite slab](../../../../planar-shock-compression-of-a-finite-slab.md). In the uniform post-shock approximation, breakout occurs at $t_b=L/V_s$. The original front face has then moved $(3V_s/4)t_b=3L/4$, while the shock reaches the originally stationary far face at $L$, leaving thickness $L/4$. Equivalently, the fixed mass per area $\rho L$ becomes $4\rho L_2$. The result assumes a maintained approximately constant shock speed and no important boundary rarefaction during the crossing; an unconfined finite cloud need not remain uniformly compressed.

**Escape estimate and the sound-speed convention.** Let $M_c$ be the slab mass, $W>0$ its binding-energy magnitude in the star's field, and $E_{\rm th}$ its initial [internal energy](../../../../internal-energy-split.md). Treat the potential as nearly uniform across the slab. For the bulk-ballistic escape estimate, require

$$
E_{\rm bulk}=\frac12M_cv_2^2=\frac9{32}M_cV_s^2\gtrsim W,
\qquad
E_{\rm th}=\frac{3}{2}\frac{M_cp}{\rho}.
$$

The [Mach-number convention in shock unbinding estimates](../../../../mach-number-convention-in-shock-unbinding-estimates.md) matters here. With the usual upstream [adiabatic sound speed](../../../../adiabatic-sound-speed.md), $c_{\rm ad}^2=\gamma p/\rho=5p/(3\rho)$, define $\mathcal M_{\rm ad}=V_s/c_{\rm ad}$. Then

$$
\frac{E_{\rm bulk}}{E_{\rm th}}=\frac5{16}\mathcal M_{\rm ad}^2,
\qquad
\boxed{\mathcal M_{\rm ad}^2\gtrsim\frac{16}{5}\frac{W}{E_{\rm th}}.}
$$

If instead the shock speed is normalized by the [isothermal sound speed](../../../../isothermal-sound-speed.md), $c_T^2=p/\rho$, then $\mathcal M_T^2=(5/3)\mathcal M_{\rm ad}^2$ and

$$
\boxed{\mathcal M_T^2\gtrsim\frac{16}{3}\frac{W}{E_{\rm th}}
\simeq5.3\,\frac{W}{E_{\rm th}}.}
$$

The original PDF's “around five” is consistent with the latter convention or an order-of-magnitude sound-speed estimate. It is not the exact coefficient obtained with the conventional adiabatic Mach number and the stated bulk kinetic-energy criterion. Here $W=-E_{\rm grav}$ if the potential is zero at infinity; using negative gravitational energy directly on the right would be incorrect. Subsequent conversion of shock-generated internal energy to expansion, external pressure, or radiative losses would change the physical escape threshold, so this numerical factor is not universal.

## ↑ Ancestors (13)

1. [B2](../b2.md)
2. [Section B](../../section-b.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../split.md)
5. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
