<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

In [resistive-force theory](../../../../../resistive-force-theory.md), the flagellum is slender and moves at a small [Reynolds number](../../../../../reynolds-number.md), so local viscous resistance is linear in its [velocity](../../../../../velocity.md) and fluid and body inertia are neglected. Normal and tangential resistance coefficients are treated as positive constants, usually $\kappa_N>\kappa_T$. The approximation neglects distant hydrodynamic interactions along the filament, head-tail interactions, nearby boundaries and self-contact. The centreline is an [inextensible filament](../../../../../inextensible-filament.md) with prescribed shape. Its local resistance tensor is

$$
K=\kappa_T\mathbf t\mathbf t+\kappa_N(I-\mathbf t\mathbf t).
$$

Since the filament velocity relative to distant fluid is $-\mathbf w$, the fluid force on a filament element is $K\mathbf w\,ds$. The equal and opposite force on the fluid has total axial component $T$. Projecting onto $\mathbf i$ gives

$$
-T=\int_0^L\mathbf i\cdot K\mathbf w\,ds=(\kappa_T-\kappa_N)\int_0^L(\mathbf w\cdot\mathbf t)(\mathbf t\cdot\mathbf i)ds+\kappa_N\int_0^L\mathbf w\cdot\mathbf i\,ds.
$$

This establishes the thrust expression with its force-on-fluid convention.

For a uniform [travelling wave](../../../../../travelling-wave.md), write the moving centreline as $\mathbf r(s,t)=\mathbf r_{\rm wave}(s-ct)+(V-U)t\mathbf i$, where $s$ is material [arc length](../../../../../arc-length.md) and $|\mathbf r_{\rm wave}'|=1$. Differentiating at fixed material label gives $\mathbf r_t=(V-U)\mathbf i-c\mathbf t$. Hence

$$
\boxed{\mathbf w=(U-V)\mathbf i+c\mathbf t.}
$$

Let $q=\mathbf t\cdot\mathbf i=X_s$, $\alpha=\langle q\rangle$ and $\beta=\langle q^2\rangle$, where these brackets are contour-length averages. The axial wavelength divided by contour wavelength is $\alpha=V/c$. For a filament comprising whole wave periods, or after the usual period averaging, $c\int_0^Lq\,ds=VL$. This averaging is needed to avoid end-phase corrections for an arbitrary fraction of a wavelength. Substitution of $\mathbf w$ into the thrust expression now gives

$$
T=(V-U)[(\kappa_T-\kappa_N)\beta L+\kappa_NL]-\kappa_TVL.
$$

For $\gamma=\kappa_T/\kappa_N$ and $r=1-\gamma$, this is $T/(\kappa_NL)=Vr(1-\beta)-U(1-r\beta)$. The swimming body is [force-free](../../../../../force-free.md), so the reaction thrust on the head-tail assembly balances its head drag. Thus $T=\delta\kappa_NLU$, and [linear resistive-force propulsion of a travelling filament](../../../../../linear-resistive-force-propulsion-of-a-travelling-filament.md) gives

$$
\boxed{U=V\frac{(1-\gamma)(1-\beta)}{1+\delta-(1-\gamma)\beta}.}
$$

We henceforth assume $0<\gamma<1$, $\delta\geq0$ and $0<\beta<1$. Isotropic resistance, $\gamma=1$, gives no propulsion in this model.

The flagellar contribution to [viscous dissipation](../../../../../viscous-dissipation.md) is the positive quadratic form $P_f=\int\mathbf w\cdot K\mathbf w\,ds$. Expanding it, and using $c\langle q\rangle=V$, gives

$$
P_f=\kappa_NL\left\{(V-U)^2[1-(1-\gamma)\beta]-2\gamma V(V-U)+\gamma c^2\right\}.
$$

There is also head dissipation $\delta\kappa_NLU^2$. Equivalently, the work of the flagellar deformation relative to the translating head is $P_f+UT$; the force balance makes $UT$ precisely the head dissipation. Consequently, with $\alpha=V/c$,

$$
\boxed{\frac{E}{\kappa_NLU^2}=\left(\frac VU-1\right)^2(\beta\gamma+1-\beta)-2\gamma\frac VU\left(\frac VU-1\right)+\frac{\gamma V^2}{\alpha^2U^2}+\delta.}
$$

This derives the rate of working, rather than merely inferring it from the thrust.

The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) gives $\alpha^2=\langle q\rangle^2\leq\langle q^2\rangle=\beta$. Equality requires $q$ to be constant almost everywhere. For a planar periodic filament this is an ideal sawtooth with alternating transverse tangent and fixed axial tangent, or a limit with negligibly rounded corners. It is not an identity for a general sinusoidal wave, and the ideal calculation omits the elastic cost of sharp corners.

For the stipulated equality $\alpha^2=\beta$, put $d=1+\delta$ and eliminate $V$ at fixed $U$ using $V/U=(d-r\beta)/[r(1-\beta)]$. Direct simplification yields

$$
F(\beta):=\frac{E}{\kappa_NLU^2}=\frac{(d-r\beta)(\gamma d+\delta r\beta)}{r^2\beta(1-\beta)}.
$$

The derivative is

$$
F'(\beta)=\frac{r(\delta^2-\gamma)\beta^2+2\gamma d^2\beta-\gamma d^2}{r^2\beta^2(1-\beta)^2}.
$$

Writing $A=r(\delta^2-\gamma)$ and $B=\gamma d^2$, the numerator is $A\beta^2+2B\beta-B$. It is negative at zero and equals $(\delta+\gamma)^2>0$ at one. Its derivative is positive throughout $(0,1)$: this is immediate if $A\geq0$; if $A<0$, its minimum derivative is $2(A+B)=2(\delta+\gamma)^2>0$. Since $F$ diverges at both endpoints, the unique stationary point is the global [fixed-speed energy optimum for a planar flagellum](../../../../../fixed-speed-energy-optimum-for-a-planar-flagellum.md):

$$
\boxed{\beta_* =\frac{B}{B+\sqrt{B^2+AB}},\qquad A=(1-\gamma)(\delta^2-\gamma),\quad B=\gamma(1+\delta)^2.}
$$

This form includes the case $A=0$, when $\beta_*=1/2$, without a removable division by zero. With no head drag it reduces to $\beta_*=1/(1+\sqrt\gamma)$.

**The printed final optimality formula does not follow from the preceding thrust and power equations.** For a concrete check, $\gamma=1/2$, $\delta=0$ gives $F=(2-\beta)/[\beta(1-\beta)]$. The derived minimum is at $\beta=2-\sqrt2$. The printed formula instead gives $\beta^2=\sqrt6-2$, hence $\beta\approx0.67044$, where $F'\ne0$ and the expenditure is greater. Thus the thrust and working formulas can both be established as above, but the last printed conclusion must be replaced by the derived optimum.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
