<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take the current to be dilute, vertically well mixed and [Boussinesq approximation](../../../../../boussinesq-approximation.md), with constant channel width $w$, a horizontal absorbing bed, negligible ambient [fluid entrainment](../../../../../fluid-entrainment.md), negligible bed friction, and no resuspension. The [shallow-water approximation](../../../../../shallow-water-approximation.md) neglects vertical inertia and gives [hydrostatic pressure](../../../../../hydrostatic-pressure.md). Particle loss alters [reduced gravity](../../../../../reduced-gravity-split.md) but does not alter the leading-order carrier-fluid volume or inertia; otherwise additional mass and momentum terms would be necessary. The current occupies depth $h(x,t)$, has depth-uniform speed $u(x,t)$, and has [particle volume fraction](../../../../../particle-volume-fraction.md) $c(x,t)$, with $g'=g_oc$ and constant $g_o>0$.

[Volume conservation](../../../../../volume-conservation.md) of a short channel segment gives $h_t+(uh)_x=0$. Its suspended particle amount per unit bed area is $hc$, and the downward [particle deposition flux](../../../../../particle-deposition-flux.md) is $v_sc$. Thus $(hc)_t+(uhc)_x=-v_sc$, which becomes $(hg')_t+(uhg')_x=-v_sg'$ on multiplying by $g_o$.

At vertical coordinate $y$ above the bed, excess [hydrostatic pressure](../../../../../hydrostatic-pressure.md) divided by reference [mass density](../../../../../density.md) is $g'(h-y)$. Integrating across the depth gives the depth-integrated [force](../../../../../force.md) flux $g'h^2/2$. The horizontal momentum per unit bed area is $hu$ and the advected kinematic [momentum flux](../../../../../momentum-flux.md) is $hu^2$. The resulting [variable-buoyancy shallow water equations](../../../../../variable-buoyancy-shallow-water-equations.md) are

$$
\boxed{h_t+(uh)_x=0,\qquad (hg')_t+(uhg')_x=-v_sg',\qquad (hu)_t+(hu^2+\tfrac12g'h^2)_x=0.}
$$

The derivative of the pressure term acts on both $h$ and $g'$; treating [reduced gravity](../../../../../reduced-gravity-split.md) as horizontally constant while particles settle would lose part of the force.

For a steady interior, let $q=Q/w=uh>0$ denote [volume flux per unit width](../../../../../volume-flux-per-unit-width.md). Then the particle balance is a [first-order linear differential equation](../../../../../first-order-linear-differential-equation.md),

$$
\boxed{\frac{dg'}{dx}=-\frac{v_s}{q}g'=-\frac{v_sw}{Q}g',\qquad g'(x)=g'_0\exp\left(-\frac{v_sw}{Q}x\right).}
$$

Here $g'_0=g'(0)>0$, $v_s\geq0$ is constant, and deposited particles are not returned to the current. In particular the decay length is $q/v_s=Q/(wv_s)$ for $v_s>0$, and the cancellation of depth follows from $uh=q$: dilution and transit time compensate in the deposition balance.

The steady momentum equation also gives

$$
\boxed{K=u^2h+\frac12g'h^2=\frac{q^2}{h}+\frac12g'h^2=\text{constant}.}
$$

The inlet depth selects $K=q^2/h_0+g'_0h_0^2/2$. Depth and speed at every downstream position are determined by the continuous positive [root of a polynomial](../../../../../root-of-a-polynomial.md) in

$$
\boxed{\frac12g'_0e^{-v_sx/q}h^3-Kh+q^2=0,\qquad u=\frac qh.}
$$

This implicit expression also makes clear why the inlet condition is needed: there are generally two possible positive depths.

The [depth branches of a steady depositing gravity current](../../../../../depth-branches-of-a-steady-depositing-gravity-current.md) are distinguished by the [Froude number](../../../../../froude-number.md) $\operatorname{Fr}^2=q^2/(g'h^3)$. Differentiating the momentum invariant, and using the [exponential decay](../../../../../exponential-decay.md) of [reduced gravity](../../../../../reduced-gravity-split.md), gives

$$
\left(g'h-\frac{q^2}{h^2}\right)h_x=\frac{v_sg'h^2}{2q},\qquad \boxed{h_x=\frac{v_sh}{2q(1-\operatorname{Fr}^2)}.}
$$

For $v_s>0$, [supercritical flow](../../../../../supercritical-flow.md) has $\operatorname{Fr}>1$ and decreasing depth, with $h\to q^2/K$ and $u\to K/q$ as $x\to\infty$. [Subcritical flow](../../../../../subcritical-flow.md) has $\operatorname{Fr}<1$ and increasing depth, with $h\sim\sqrt{2K/g'(x)}\propto e^{v_sx/(2q)}$. This indefinitely deepening branch eventually violates the assumed shallow or confined-channel geometry. Hence the depth does not universally decrease: that conclusion needs a supercritical inlet.

For fixed $g'>0$, $q^2/h+g'h^2/2$ has its unique minimum at $h_c=(q^2/g')^{1/3}$, with $K_c=3q^{4/3}(g')^{1/3}/2$. The two positive roots when $K>K_c$ lie below and above $h_c$. Since $K_c$ decreases downstream while $K$ is constant, an initially strict branch remains separate from the other branch and cannot cross a critical point. A critical inlet with $v_s>0$ has no finite depth derivative: at $\operatorname{Fr}=1$ the first differentiated equation would equate zero to a positive value. It requires a singular entrance adjustment or physics beyond this steady model. If $v_s=0$, both [reduced gravity](../../../../../reduced-gravity-split.md) and the continuous depth branch are constant. These steady solutions describe the supplied current interior, not a moving finite-release front.

For two particle populations, write $g'=g'_1+g'_2$ and $g'_i=g_{0i}c_i$, allowing different constant particle-density conversion factors. The bidisperse [particle-laden gravity current](../../../../../particle-laden-gravity-current.md) equations are

$$
\boxed{h_t+(uh)_x=0,\qquad (hg'_i)_t+(uhg'_i)_x=-v_i g'_i\ (i=1,2),\qquad (hu)_t+\bigl(hu^2+\tfrac12h^2(g'_1+g'_2)\bigr)_x=0.}
$$

For the steady case,

$$
g'_i(x)=g'_{i0}e^{-v_ix/q},\qquad c_i(x)=c_{i0}e^{-v_ix/q},\qquad K=\frac{q^2}{h}+\frac12h^2\bigl(g'_{10}e^{-v_1x/q}+g'_{20}e^{-v_2x/q}\bigr).
$$

Thus the depth is obtained from the same cubic [polynomial](../../../../../polynomial-split.md) invariant with the sum of the two exponentially decreasing [reduced gravity](../../../../../reduced-gravity-split.md) contributions.

The local deposit consists of the two [particle deposition fluxes](../../../../../particle-deposition-flux.md) $v_1c_1$ and $v_2c_2$. For a positive total deposition rate, the [bidisperse gravity-current deposition](../../../../../bidisperse-gravity-current-deposition.md) fraction by particle volume is

$$
\boxed{f_1(x)=\frac{v_1c_{10}e^{-v_1x/q}}{v_1c_{10}e^{-v_1x/q}+v_2c_{20}e^{-v_2x/q}}.}
$$

If the particles have a common material density, this is also their local mass fraction. If they have common $g_o$, it can be written in the source's buoyancy notation as

$$
\boxed{f_1(x)=\left[1+\frac{v_2g'_{20}}{v_1g'_{10}}\exp\left(\frac{(v_1-v_2)wx}{Q}\right)\right]^{-1}.}
$$

For unequal $g_{0i}$ replace each $g'_{i0}$ by $g'_{i0}/g_{0i}$. The exponent sign matters: with both populations present and $v_1>v_2>0$, the faster-settling population has decreasing local deposit fraction downstream, since $f_1'=(v_2-v_1)f_1(1-f_1)/q<0$. Equal positive settling speeds give a constant fraction. A nonsettling population contributes no deposit; if the entire local deposition rate is zero the deposit fraction is undefined.

If “fraction of particles” means number fraction rather than particle-volume or mass fraction, let $a_i$ be a single particle's volume in population $i$. The correct weights are then $v_ic_i/a_i$, so

$$
\boxed{f_1^{\mathrm{number}}(x)=\frac{v_1c_{10}e^{-v_1x/q}/a_1}{v_1c_{10}e^{-v_1x/q}/a_1+v_2c_{20}e^{-v_2x/q}/a_2}.}
$$

Settling speeds alone do not determine $a_i$ without particle properties and a drag law. Finally, if the intended deposit is cumulative over the bed from $0$ to $x$, rather than local at $x$, integrating [particle deposition flux](../../../../../particle-deposition-flux.md) gives the species volumes per unit channel width $D_i(x)=q c_{i0}(1-e^{-v_ix/q})$. The cumulative particle-volume fraction is

$$
\boxed{F_1(x)=\frac{c_{10}(1-e^{-v_1x/q})}{c_{10}(1-e^{-v_1x/q})+c_{20}(1-e^{-v_2x/q})}.}
$$

For both $v_i>0$, its limit at infinity is the incoming particle-volume fraction, whereas its limit as $x\downarrow0$ is the local deposition fraction at the inlet. Local sorting and the cumulative inventory are different observables.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 345](../../paper-345-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
