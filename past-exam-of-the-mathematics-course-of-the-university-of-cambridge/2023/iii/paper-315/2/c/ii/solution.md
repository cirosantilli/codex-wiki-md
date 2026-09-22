<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Convection begins when the [radiative temperature gradient](../../../../../../../radiative-temperature-gradient.md) equals the [adiabatic temperature gradient](../../../../../../../adiabatic-temperature-gradient.md) $\nabla_{\rm ad}$. To convert optical depth into pressure, assume a pressure-law opacity $\kappa=\kappa_0P^n$ and constant gravity. Hydrostatic balance gives

$$
\tau(P)=\frac{\kappa_0P^{n+1}}{(n+1)g},
\qquad
\frac{d\log\tau}{d\log P}=n+1.
$$

Hence

$$
\nabla_{\rm rad}
=\frac{d\log T}{d\log P}
=\frac{(n+1)\tau[B-\beta Ce^{-\beta\tau}]}
{4[A+B\tau+Ce^{-\beta\tau}]}.
$$

The exact [radiative-convective boundary](../../../../../../../radiative-convective-boundary.md) is the positive solution of

$$
\boxed{
\frac{(n+1)\tau_{\rm rc}[B-\beta Ce^{-\beta\tau_{\rm rc}}]}
{4[A+B\tau_{\rm rc}+Ce^{-\beta\tau_{\rm rc}}]}
=\nabla_{\rm ad},
\qquad
P_{\rm rc}=\left[
\frac{(n+1)g\tau_{\rm rc}}{\kappa_0}
\right]^{1/(n+1)}}.
$$

Deep enough that the exponential term is negligible,

$$
\tau_{\rm rc}\simeq
\frac{4\nabla_{\rm ad}A}
{B(n+1-4\nabla_{\rm ad})},
$$

which requires $n+1>4\nabla_{\rm ad}$. This exposes why constant opacity is inadequate for a molecular atmosphere: its limiting radiative gradient is $1/4$, below $\nabla_{\rm ad}\simeq2/7$.

In a grey scaling, $A\sim T_{\rm eq}^4$ measures irradiation and $B\sim T_{\rm int}^4$ measures intrinsic flux. Thus

$$
P_{\rm rc}\propto(A/B)^{1/(n+1)}.
$$

For a hot Jupiter with $T_{\rm eq}\sim1500\,{\rm K}$ and $T_{\rm int}\sim100\,{\rm K}$, irradiation pushes the boundary to hundreds of bars for typical increasing opacity. Jupiter has $T_{\rm eq}$ and $T_{\rm int}$ both of order $10^2\,{\rm K}$ and becomes convective near the bar scale. The estimate is order-of-magnitude because real opacities depend on both pressure and temperature.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [Paper 315](../../../../paper-315-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
