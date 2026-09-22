<h1 id="section-b/11/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the stated $1\,\mathrm{m^2}$ area, the total [electric current](../../../../../../electric-current.md) is $I=200\,\mathrm A$. The known [ohmic polarization](../../../../../../ohmic-polarization.md) is $IR_\Omega=1.20\,\mathrm V$. Applying the supplied anodic [Tafel equation](../../../../../../tafel-equation.md) gives

$$
\eta_a=0.295\log_{10}(200/1)=0.6788\,\mathrm V.
$$

Assume the quoted limiting current uses the same cathodic area convention. A steady diffusion-film model gives $c_s/c_b=1-j/j_L=1/41$. The [Nernst equation](../../../../../../nernst-equation.md) then makes the cathodic [concentration overpotential](../../../../../../concentration-overpotential.md) magnitude

$$
|\eta_{c,\rm conc}|=\frac{RT}{2F}\ln41=0.04765\,\mathrm V.
$$

Relative to the local surface equilibrium potential, the [cathode](../../../../../../cathode.md) also needs an [activation overpotential](../../../../../../activation-overpotential.md). Neglecting anodic [concentration](../../../../../../concentration.md) polarization, the separated-loss accounting is

$$
\boxed{V_{\rm app}\simeq1.9265\,\mathrm V+|\eta_{c,\rm act}|}.
$$

To calculate that activation term, adopt a single effective two-electron [Butler-Volmer equation](../../../../../../butler-volmer-equation.md) with constant transfer coefficients satisfying $\alpha_a+\alpha_c=1$, no anodic [concentration](../../../../../../concentration.md) polarization and [reduction](../../../../../../reduction-chemistry.md) proportional to the surface $\mathrm{Cu}^{2+}$ [concentration](../../../../../../concentration.md). The supplied anodic [Tafel slope](../../../../../../tafel-slope.md) then determines the reverse slope through

$$
\alpha_a=\frac{RT\ln10}{2Fb}\simeq0.10016,\qquad\alpha_c=1-\alpha_a\simeq0.89984.
$$

With $f=2F/(RT)$ and cathodic [overpotential](../../../../../../overpotential.md) $\eta_c$ referenced to bulk equilibrium,

$$
\frac{j_c}{j_0}=\exp(\alpha_a f\eta_c)-\frac{c_s}{c_b}\exp(-\alpha_c f\eta_c).
$$

Solving at $j_c=-200\,\mathrm{A\,m^{-2}}$ gives $\eta_c\simeq-0.12854\,\mathrm V$, including both [concentration](../../../../../../concentration.md) and activation effects. Thus

$$
\boxed{V_{\rm app}\simeq1.20+0.67880+0.12854=2.0073\,\mathrm V\simeq2.01\,\mathrm V.}
$$

The $0.04765$ V [concentration](../../../../../../concentration.md) loss must not be added again. The kinetic assumption matters: the supplied slope is for [copper](../../../../../../copper.md) [oxidation](../../../../../../oxidation.md), and an [exchange current density](../../../../../../exchange-current-density.md) alone does not specify every cathodic current-potential relation. A multistep [copper](../../../../../../copper.md) reaction need not obey the effective single-step relation used for this estimate.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [11](../../11.md)
3. [Section B](../../../section-b.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../split.md)
7. [MPhil in micro- and nanotechnology enterprise course of the University of Cambridge](../../../../../../mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
