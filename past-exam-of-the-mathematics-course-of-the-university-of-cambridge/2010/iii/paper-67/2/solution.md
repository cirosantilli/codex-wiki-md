<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Introduce a constant [filament bending modulus](../../../../../filament-bending-modulus.md) $B$, which sets the mechanical force scale. The filament has [intrinsic curvature of an elastic filament](../../../../../intrinsic-curvature-of-an-elastic-filament.md) $\kappa_0(s)$, and its actual [signed curvature](../../../../../signed-curvature.md) in a small-slope [Monge representation](../../../../../monge-representation.md) is $\kappa\simeq\zeta_{xx}$. To quadratic order one may identify material [arc length](../../../../../arc-length.md) $s$ with $x$ in $\kappa_0$, while

$$
\mathcal L-L=\frac12\int_0^L\zeta_x^2dx+O(\zeta_x^4).
$$

At fixed positive extension force, the mechanical potential is bending energy minus $FL$. Replacing $L$ by $\mathcal L-(\mathcal L-L)$ leaves, up to a force-dependent constant,

$$
\boxed{\mathcal H[\zeta]=\frac12\int_0^L
\left[B(\zeta_{xx}-\kappa_0)^2+F\zeta_x^2\right]dx}.
$$

Its first variation is

$$
\delta\mathcal H=\int_0^L[B(\zeta_{xx}-\kappa_0)_{xx}-F\zeta_{xx}]\delta\zeta\,dx
+\left[B(\zeta_{xx}-\kappa_0)\delta\zeta_x+
\{F\zeta_x-B(\zeta_{xxx}-\kappa_{0,x})\}\delta\zeta\right]_0^L.
$$

The [higher-order Euler-Lagrange equation](../../../../../higher-order-euler-lagrange-equation.md) is therefore

$$
\boxed{B\zeta_{xxxx}-F\zeta_{xx}=B\kappa_{0,xx}}.
$$

For a [Fourier transform](../../../../../fourier-transform.md) relation, take a periodic bulk segment, or a long-filament bulk approximation with negligible endpoint contributions; these are necessary [boundary conditions](../../../../../boundary-condition.md) because the question specifies no filament end conditions. Using $f(x)=\int\widehat f(q)e^{iqx}dq/(2\pi)$, every nonzero [wavenumber](../../../../../wavenumber.md) obeys

$$
(Bq^4+Fq^2)\widehat\zeta(q)=-Bq^2\widehat\kappa_0(q),\qquad
\boxed{\widehat\zeta(q)=-\frac{B\widehat\kappa_0(q)}{F+Bq^2}}.
$$

A zero displacement mode is an arbitrary translation. In a periodic representation a constant intrinsic-curvature mode contributes a constant bending cost but no bulk slope, so it does not contribute to the following deficit. The [Parseval identity](../../../../../parseval-identity.md) gives

$$
\boxed{\mathcal L-L=\frac{B^2}2\int\frac{dq}{2\pi}
\frac{q^2|\widehat\kappa_0(q)|^2}{(F+Bq^2)^2}}.
$$

For clarity about finite normalization, on a periodic interval of length $L$ define $\kappa_n=L^{-1}\int_0^L\kappa_0(x)e^{-iq_nx}dx$, $q_n=2\pi n/L$. Then the equivalent exact quadratic-order formula is

$$
\mathcal L-L=\frac{LB^2}2\sum_{n\ne0}
\frac{q_n^2|\kappa_n|^2}{(F+Bq_n^2)^2}.
$$

This is [force-extension of an intrinsically curved filament](../../../../../force-extension-of-an-intrinsically-curved-filament.md), determined by its particular fixed shape rather than by a thermal orientation entropy.

For an ensemble with [quenched intrinsic curvature](../../../../../quenched-intrinsic-curvature.md), first minimize each realization and then average the last expression, replacing $|\kappa_n|^2$ by its ensemble mean. For stationary bulk disorder, let $S_\kappa(q)$ be the [power spectrum](../../../../../power-spectrum.md), normalized so that its correlation is $\langle\kappa_0(x)\kappa_0(x+r)\rangle=\int S_\kappa(q)e^{iqr}dq/(2\pi)$. The measurable mean deficit per unit projected length is

$$
\boxed{\frac{\langle\mathcal L-L\rangle}{L}
=\frac{B^2}2\int\frac{dq}{2\pi}\frac{q^2S_\kappa(q)}{(F+Bq^2)^2}}.
$$

If the curvature is smooth enough that the second spectral moment is finite, one can take the large-force limit under this integral, obtaining the [smooth-curvature high-force extension law](../../../../../smooth-curvature-high-force-extension-law.md)

$$
\boxed{\langle\mathcal L-L\rangle\sim\frac{B^2}{2F^2}
\int_0^L\langle(\kappa_{0,x})^2\rangle dx}.
$$

For a stationary ensemble the integral is $L\langle(\kappa_{0,x})^2\rangle$. Equivalently, the bulk slope is $\zeta_x\simeq-(B/F)\kappa_{0,x}$; a plot of the mean deficit against $F^{-2}$ measures the mean squared intrinsic-curvature gradient, if $B$ is known. **The $F^{-2}$ law is a smooth-curvature bulk result, not a universal law for every random filament.** For example, ideal white intrinsic-curvature disorder with $S_\kappa(q)=S_0$ has an infinite second spectral moment; retaining the full integral instead gives $\langle\mathcal L-L\rangle/L=S_0\sqrt B/(8\sqrt F)$ in that ideal continuum model.

Endpoint conditions also matter. If each end is moment-free and has no transverse applied force, the natural conditions from the variation are

$$
\zeta_{xx}=\kappa_0,\qquad
B(\zeta_{xxx}-\kappa_{0,x})-F\zeta_x=0
$$

at each end. These can produce a [free-end curvature boundary layer](../../../../../free-end-curvature-boundary-layer.md) of width $\ell=\sqrt{B/F}$. For a constant [intrinsic filament curvature](../../../../../intrinsic-curvature-of-an-elastic-filament.md) $\kappa$, integration of the [higher-order Euler-Lagrange equation](../../../../../higher-order-euler-lagrange-equation.md) with zero transverse force gives $B(\zeta_x)_{xx}-F\zeta_x=0$ and hence

$$
\zeta_x=\kappa\ell\frac{\sinh[(x-L/2)/\ell]}{\cosh[L/(2\ell)]},\qquad
\mathcal L-L=\frac{\kappa^2\ell^3}2\left[\tanh a-a\operatorname{sech}^2a\right],\quad a=\frac{L}{2\ell}.
$$

The last formula follows by integrating $\sinh^2[(x-L/2)/\ell]$, and tends to $\kappa^2\ell^3/2\propto F^{-3/2}$, despite the vanishing bulk curvature gradient. Thus a finite free-ended measurement must include or suppress endpoint bending before interpreting a bulk $F^{-2}$ fit.

For the [freely jointed chain](../../../../../ideal-chain.md), rigid links have independent orientations, so the restoring force is entropic. Let $T$ now denote absolute [temperature](../../../../../temperature.md), and $\beta=1/(k_BT)$ with [Boltzmann constant](../../../../../boltzmann-constant.md) $k_B$. In the usual three-dimensional chain, a segment at polar angle $\theta$ has force energy $-Fb\cos\theta$. Its angular [canonical partition function](../../../../../canonical-partition-function.md) and the full chain [partition function](../../../../../canonical-partition-function.md) are

$$
Z_1=2\pi\int_{-1}^1e^{\xi\mu}d\mu
=4\pi\frac{\sinh\xi}{\xi},\qquad
Z_N=Z_1^N,\qquad \xi=\beta Fb.
$$

Differentiating $\log Z_N$ with respect to $\beta F$ yields the exact mean projected displacement

$$
\boxed{\langle L\rangle=Nb\left(\coth\xi-\frac1\xi\right)
=Nb\mathscr L(\xi)}.
$$

Here $\mathscr L$ is the [Langevin function](../../../../../langevin-function.md); this is [force-extension of a three-dimensional freely jointed chain](../../../../../force-extension-of-a-three-dimensional-freely-jointed-chain.md), in the fixed-force [canonical ensemble](../../../../../canonical-ensemble.md). At high extension, $\coth\xi=1+2e^{-2\xi}+\cdots$, so

$$
\boxed{Nb-\langle L\rangle\sim\frac{Nk_BT}{F},\qquad
F\sim\frac{Nk_BT}{Nb-\langle L\rangle}}.
$$

Thus the smooth quenched-curvature bulk deficit falls as $F^{-2}$, whereas the three-dimensional [freely jointed chain](../../../../../ideal-chain.md) deficit falls as $F^{-1}$ and depends explicitly on [temperature](../../../../../temperature.md). The distinction is mechanical straightening of a fixed intrinsic shape versus orientational [entropy](../../../../../entropy.md); thermal bending fluctuations of a stiff filament have not been included in the first calculation.

If the comparison chain is also restricted to two dimensions, it is a [planar freely jointed chain](../../../../../planar-freely-jointed-chain.md) rather than the three-dimensional model. In this case,

$$
Z_1=\int_0^{2\pi}e^{\xi\cos\theta}d\theta=2\pi I_0(\xi),\qquad
\boxed{\frac{\langle L\rangle}{Nb}=\frac{I_1(\xi)}{I_0(\xi)}}.
$$

The last identity follows directly by differentiating the integral defining $I_0$; $I_0$ and $I_1$ are [Modified Bessel functions of the first kind](../../../../../modified-bessel-function-of-the-first-kind.md). At large $\xi$ the angular weight is proportional to $e^{-\xi\theta^2/2}$, giving $\langle\cos\theta\rangle\simeq1-\langle\theta^2\rangle/2=1-1/(2\xi)$. Consequently $Nb-\langle L\rangle\sim Nk_BT/(2F)$: the same inverse-force exponent, with half the three-dimensional coefficient. Both versions assume inextensible links and forces below the regime where the links themselves stretch.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
