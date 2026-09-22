<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use a [two-sided top-hat line plume](../../../../../two-sided-top-hat-line-plume.md) with full width $w(z)$, upward speed $U(z)$, and [reduced gravity](../../../../../reduced-gravity-split.md) $b(z)$ uniform across the plume. Fluxes are measured per unit span along the line source: the [volume flux](../../../../../volumetric-flow-rate.md) is $V=wU$, the kinematic [momentum flux](../../../../../momentum-flux.md) is $M=wU^2$, and the [buoyancy flux](../../../../../buoyancy-flux.md) is $B=wUb$. If the inward edge speed is $eU$, where $e>0$ is the [entrainment coefficient](../../../../../entrainment-coefficient.md), the two exposed edges give

$$
\frac{dV}{dz}=2eU,\qquad \frac{dM}{dz}=wb=\frac BU,\qquad \frac{dB}{dz}=0.
$$

These are the [volume conservation](../../../../../volume-conservation.md), [momentum conservation](../../../../../momentum-conservation.md), and [buoyancy flux](../../../../../buoyancy-flux.md) balances for a [Boussinesq approximation](../../../../../boussinesq-approximation.md) plume in an unstratified ambient. Entrained ambient fluid supplies neither vertical momentum nor reference [buoyancy](../../../../../buoyancy.md).

A [pure plume](../../../../../pure-plume.md) has no persistent source length scale. Since a line-source $B$ has dimensions $L^3T^{-3}$, [dimensional analysis](../../../../../dimensional-analysis.md) gives constant $U\propto B^{1/3}$, $w\propto z$, and $V\propto z$. Substituting constant $U$ into $M=UV$ and the momentum balance determines the coefficients:

$$
2eU^2=\frac BU,\qquad \boxed{U=(2e)^{-1/3}B^{1/3},\quad w=2ez,\quad V=(2e)^{2/3}B^{1/3}z.}
$$

Thus $\lambda=(2e)^{2/3}$ and $\mu=2e$ when width is full width and velocity and [buoyancy](../../../../../buoyancy.md) have top-hat profiles. If width means half-width, $\mu=e$ instead. Other prescribed profile shapes change these numerical factors; the linear growth laws remain the same. The point-source $B$ in Question 1 has different dimensions, so its $z^{5/3}$ law must not be used here.

Let $C(x,z,t)$ be local contaminant [concentration](../../../../../concentration.md) and let $c(z,t)=\int C(x,z,t)\,dx$ be [horizontally integrated plume concentration](../../../../../horizontally-integrated-plume-concentration.md). Its conserved amount per unit span is $\int_0^\infty c\,dz=V_c$. The dilute contaminant is a [passive scalar](../../../../../passive-scalar.md); the maintained plume is unaffected by its impulsive release. A one-dimensional effective transport closure takes the integrated scalar flux to be

$$
J=a c-K(z)c_z,\qquad a=\alpha B^{1/3},\qquad K(z)=Dz,\qquad D=\beta B^{1/3}.
$$

The constant advective speed and the [eddy diffusivity](../../../../../eddy-diffusivity.md) scaling $K\sim Uw\propto B^{1/3}z$ follow from the line-plume scales. The [entrainment coefficient](../../../../../entrainment-coefficient.md) alone does not determine the scalar dispersion coefficient: this Fickian closure for the integrated variable is an additional modelling assumption. [Mass conservation](../../../../../mass-conservation.md) $c_t+J_z=0$ then gives the displayed transport equation in the PDF. With this effective closure and advective speed chosen as $U$, $\alpha=(2e)^{-1/3}$; if $K=\kappa Uw$, then $\beta=\kappa(2e)^{2/3}$, with independent dimensionless mixing coefficient $\kappa$.

There is a second possible closure convention. If one instead applies local diffusive flux to [horizontally averaged plume concentration](../../../../../horizontally-averaged-plume-concentration.md) $\overline C=c/w$, its integrated diffusive flux is $-Kw\overline C_z=-K(c_z-c/z)$. For $K=Dz$, the total scalar flux is then $(U+D)c-Dzc_z$. The same printed equation is obtained with $a=U+D$, rather than $a=U$. Thus the printed $\alpha$ and $\beta$ should be regarded as effective coefficients unless the averaging and closure conventions are specified; no equality between $\alpha$ and the velocity prefactor is universal.

Assume $a,D>0$, $z>0$, an initial impulse $V_c\delta_0$ at the origin, no further contaminant input, and zero endpoint scalar flux for $t>0$. For a [similarity solution](../../../../../similarity-solution.md), put

$$
r=\frac aD=\frac\alpha\beta,\qquad \eta=\frac z{Dt},\qquad c=\frac{V_c}{Dt}f(\eta).
$$

Substituting into the [advection-diffusion equation](../../../../../advection-diffusion-equation.md) gives

$$
\eta f''+(1-r+\eta)f'+f=0,\qquad [\eta f'+(\eta-r)f]'=0.
$$

Decay at infinity makes the integrated constant zero. Hence $f'/f=r/\eta-1$, and normalization with the [gamma function](../../../../../gamma-function.md) gives $f(\eta)=\eta^re^{-\eta}/\Gamma(1+r)$. The resulting [gamma impulse solution for linearly increasing diffusivity](../../../../../gamma-impulse-solution-for-linearly-increasing-diffusivity.md) is

$$
\boxed{c(z,t)=\frac{V_c}{\beta B^{1/3}t\,\Gamma(1+\alpha/\beta)}\left(\frac z{\beta B^{1/3}t}\right)^{\alpha/\beta}\exp\left(-\frac z{\beta B^{1/3}t}\right).}
$$

Its [integral](../../../../../integral.md) over $z>0$ is $V_c$. Its flux is $J=(z/t)c$, which vanishes at both endpoints for $t>0$. The scale $Dt$ shrinks to zero as $t\downarrow0$, so the normalized solution has [weak convergence of probability measures](../../../../../weak-convergence-of-probability-measures.md) to the required unit source impulse. The mass at the boundary is a full unit impulse on the half-line, not half of a whole-line impulse.

For the integrated quantity, $\partial_z\log c=r/z-1/(Dt)$, and consequently

$$
\boxed{z_{\max,c}=rDt=\alpha B^{1/3}t.}
$$

This verifies the printed location for [horizontally integrated plume concentration](../../../../../horizontally-integrated-plume-concentration.md). It is a maximum because the derivative changes from positive to negative there. The normalized profile is a [gamma distribution](../../../../../gamma-distribution.md) with shape $1+r$: its [expected value](../../../../../expected-value.md) is $(a+D)t$ and its [variance](../../../../../variance-split.md) is $(a+D)Dt$, so neither the mean position nor the spread should be mistaken for the modal position.

The PDF changes from “integral” to “averaged” concentration in its final request. A genuine [horizontally averaged plume concentration](../../../../../horizontally-averaged-plume-concentration.md) divides by the growing width $w=\mu z$, and is therefore

$$
\boxed{\overline C(z,t)=\frac{V_c}{\mu(Dt)^2\Gamma(1+r)}\left(\frac z{Dt}\right)^{r-1}e^{-z/(Dt)}.}
$$

It is normalized by $\int_0^\infty w\overline C\,dz=V_c$, not by $\int\overline C\,dz$. When $a>D$, its interior maximum is

$$
\boxed{z_{\max,\overline C}=(a-D)t=(\alpha-\beta)B^{1/3}t.}
$$

When $a=D$ it decreases from a finite boundary supremum; when $0<a<D$ it is singular at the ideal point source and has no positive interior maximum. A finite source regularizes that singularity. Thus the final printed maximum is correct for the integrated variable $c$, or for an “average” using a fixed reference width, but is not generally the maximum of the local mean $c/w(z)$. Both quantities have been given rather than silently identifying them. If $D=0$, the smooth similarity formula is replaced by the advected impulse $V_c\delta(z-at)$; positive [eddy diffusivity](../../../../../eddy-diffusivity.md) is essential to the gamma profile.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 345](../../paper-345-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
