<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For stable shear-driven [turbulence](../../../../../../turbulence-split.md), let $P$ be the rate of production of [turbulent kinetic energy](../../../../../../turbulent-kinetic-energy.md) by mean shear and $B_m>0$ the rate consumed by buoyancy work. The [Flux Richardson number](../../../../../../flux-richardson-number.md) is

$$
\boxed{\mathrm{Ri}_f=\frac{B_m}{P}.}
$$

With an upward coordinate and [vertical turbulent buoyancy flux](../../../../../../vertical-turbulent-buoyancy-flux.md) $\overline{w'b'}$, $B_m=-\rho_l\int\overline{w'b'}\,d\mathcal V$, while shear production is $P=-\rho_l\int\overline{u'w'}\,\partial_zU\,d\mathcal V$. In a locally steady balance without net turbulent-energy transport or storage, $P=B_m+\mathcal D$, so $0\leq\mathrm{Ri}_f\leq1$ and the dissipation-normalized mixing coefficient is $B_m/\mathcal D=\mathrm{Ri}_f/(1-\mathrm{Ri}_f)$. A global ratio $C_W=\dot E_P/P_I$ need not equal this local production-normalized [Flux Richardson number](../../../../../../flux-richardson-number.md) when energy transport, storage, or bulk acceleration is important.

The [interfacial Richardson number](../../../../../../interfacial-richardson-number.md) in this tank is

$$
\mathrm{Ri}_I=\frac{g'd_I}{u_I^2}=\frac{Bd_I}{hu_I^2}.
$$

In model S,

$$
\boxed{\mathrm{Ri}_I=\frac{Bd_I}{\Omega^2R^2h}\propto h^{-1}.}
$$

Thus the relative importance of interface stratification changes continually. If mixing efficiency depends on [interfacial Richardson number](../../../../../../interfacial-richardson-number.md), constant $C_W$ is not generally self-consistent over substantial deepening; it can at best describe a regime where that dependence is weak. In model K,

$$
\boxed{\mathrm{Ri}_I=\frac{Bd_I}{C_I^2C_K^2\Omega^2R^2h_0}=\text{constant}.}
$$

A local efficiency depending only on this ratio can therefore remain constant, provided the fixed interface thickness and the other empirical coefficients remain appropriate.

The energetic reason to expect intermediate behavior is that entrainment must both lift and homogenize dense fluid and mobilize it. The whole upper-layer [kinetic energy](../../../../../../kinetic-energy.md) budget has the form $P_{\rm lid}=\dot K+\dot E_P+\mathcal D$, apart from additional boundary losses. Keeping the characteristic speed constant makes $K\propto h$ and requires a continuing power supply to accelerate new fluid, together with dissipation in an ever larger layer. Keeping $K$ constant instead forces the speed to decline as $h^{-1/2}$. A finite lid forcing plausibly produces an initial regime near the former and a deeper regime near the latter, rather than indefinite constant-speed entrainment.

One can make this expected bracket quantitative after matching the models' initial interface speed $u_0$. Suppose the actual speed lies between $u_0\sqrt{h_0/h}$ and $u_0$, and the same local coefficients are used. Set $D_0=2C_Wc_Du_0^3/B$. Then

$$
D_0(h_0/h)^{3/2}\leq\dot h\leq D_0.
$$

Integrating these inequalities gives

$$
\boxed{h_0\left(1+\frac{5D_0t}{2h_0}\right)^{2/5}\leq h(t)\leq h_0+D_0t.}
$$

Equivalently, if $K\propto h^q$ with $0\leq q\leq1$, the local power closure yields a late-time depth exponent $2/(5-3q)$ between $2/5$ and $1$. **This is the intended energetic interpolation between K and S**, not a universal bound following from the printed assumptions alone. Different efficiencies or unmatched initial coefficients can invalidate pointwise ordering; quantitative prediction requires the lid-to-interface power transfer and the actual energy budget.

## ↑ Ancestors (11)

1. [D](../d.md)
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
