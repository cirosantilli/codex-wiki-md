<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For two neighboring comoving points separated along the zeroth-order direction $\widehat{\mathbf n}$ by coordinate distance $\delta\chi$, the [synchronous gauge](../../../../../../synchronous-gauge-in-cosmology.md) spatial metric gives the [cosmological proper distance](../../../../../../proper-distance-in-cosmology.md)

$$
\delta r=a(t)\delta\chi
\sqrt{(\delta_{ij}-h_{ij})\widehat n_i\widehat n_j}
=a(t)\delta\chi\left(1-\frac12h_{ij}\widehat n_i\widehat n_j\right)
+O(h^2).
$$

Differentiate with respect to [cosmic time](../../../../../../cosmic-time.md) at fixed coordinate separation. To first order,

$$
\frac{d\,\delta r}{dt}
=\left(H-\frac12\dot h_{ij}\widehat n_i\widehat n_j\right)\delta r.
$$

A [photon](../../../../../../photon.md) crosses this neighboring interval in $\delta t=\delta r$ when $c=1$, so its local relative recession velocity is

$$
\boxed{\Delta v\simeq
\left(\frac{\dot a}{a}-\frac12\dot h_{ij}\widehat n_i\widehat n_j\right)\delta t.}
$$

At each infinitesimal step, the local [Doppler effect](../../../../../../doppler-effect.md) gives $d\log\nu=-\Delta v$. Therefore

$$
d\log\nu=-H\,dt+\frac12\dot h_{ij}\widehat n_i\widehat n_j\,dt.
$$

The first term integrates to the homogeneous [cosmological redshift](../../../../../../cosmological-redshift.md), $\bar\nu\propto a^{-1}$. Subtracting it isolates the metric contribution to the fractional frequency shift. A shifted [blackbody radiation](../../../../../../black-body-radiation.md) spectrum has its [temperature](../../../../../../temperature.md) shifted by the same fraction as its [photon](../../../../../../photon.md) frequencies, giving

$$
\boxed{\left.\frac{\delta T}{T}\right|_{\rm metric}
=\frac{\delta\nu}{\bar\nu}
=\frac12\int_{t_{\rm dec}}^{t_0}
\dot h_{ij}\bigl(t,\mathbf x(t)\bigr)
\widehat n_i\widehat n_j\,dt.}
$$

The dot denotes a partial time derivative at fixed comoving position, evaluated along the zeroth-order [null geodesic](../../../../../../null-geodesic.md). It is not the total derivative of $h_{ij}$ along the ray, so the integral cannot in general be replaced by a difference of $h_{ij}$ at the endpoints. Deflection of the ray or its direction multiplies an already first-order metric perturbation and is second order here. This is the metric part of the [Sachs-Wolfe effect](../../../../../../sachs-wolfe-effect.md) in the negative-spatial-perturbation convention; an intrinsic emission [temperature](../../../../../../temperature.md) fluctuation or an emitter velocity would add separate boundary terms. The time derivative is present in the original PDF, although missing from the converted TeX's displayed integral.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 67](../../../paper-67-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
