<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Briggs-Bers technique](../../../../../../../briggs-bers-criterion.md) starts with a temporal [Laplace transform](../../../../../../../laplace-transform.md) and spatial [Fourier transform](../../../../../../../fourier-transform.md) of a localized disturbance. The temporal inversion contour must initially lie above every temporal singularity. Lower it while deforming the spatial contour away from the [roots of the dispersion relation](../../../../../../../spatial-root-of-a-dispersion-relation.md). A collision of spatial branches originating on opposite sides of that contour can create a [spatial pinch point](../../../../../../../spatial-pinch-point.md). A contributing pinch with $\operatorname{Im}\omega_*>0$ gives [absolute wave-packet instability](../../../../../../../absolute-wave-packet-instability.md): exponential growth at a fixed position. Growth that is transported away while a fixed position decays is [convective wave-packet instability](../../../../../../../convective-wave-packet-instability.md). Solving $D=D_k=0$ finds candidate double roots, but does not by itself establish a pinch.

Substitution of the [normal mode](../../../../../../../normal-mode.md) gives

$$
D(k,\omega)=-i\omega-\alpha k^2-i\beta k^3+\gamma=0,\qquad \boxed{\omega(k)=i\alpha k^2-\beta k^3-i\gamma.}
$$

For real [wavenumber](../../../../../../../wavenumber.md) $k$, the temporal [growth rate](../../../../../../../growth-rate.md) is

$$
\operatorname{Im}\omega(k)=(\operatorname{Re}\alpha)k^2-(\operatorname{Im}\beta)k^3-\operatorname{Re}\gamma.
$$

A nonzero real cubic coefficient in this expression makes it unbounded above on one end of the real axis. Once that coefficient vanishes, a positive quadratic coefficient also makes it unbounded above. Hence the [bounded temporal growth condition for cubic dispersion](../../../../../../../bounded-temporal-growth-condition-for-cubic-dispersion.md) is

$$
\boxed{\operatorname{Im}\beta=0,\qquad \operatorname{Re}\alpha\leq0.}
$$

The maximum is then $-\operatorname{Re}\gamma$, attained at $k=0$ and, when $\operatorname{Re}\alpha=0$, at all real $k$. A finite upper bound is necessary for choosing the initial temporal inversion contour; arbitrarily fast high-[wavenumber](../../../../../../../wavenumber.md) growth prevents the usual [Briggs-Bers criterion](../../../../../../../briggs-bers-criterion.md) from defining that causal inversion for generic localized data.

For $\beta\ne0$, the stationary candidates satisfy

$$
\omega'(k)=k(2i\alpha-3\beta k)=0,
$$

so

$$
k_*=0,\quad \omega_*=-i\gamma;\qquad k_*^{(1)}=\frac{2i\alpha}{3\beta},\quad \omega_*^{(1)}=-i\left(\gamma+\frac{4\alpha^3}{27\beta^2}\right).
$$

Each candidate must pass the spatial-branch pinch test before its imaginary [frequency](../../../../../../../frequency.md) is used. In particular, under the finite-growth conditions the real-[wavenumber](../../../../../../../wavenumber.md) evolution has multiplier modulus at most $e^{-t\operatorname{Re}\gamma}$. For integrable transformed initial data this bounds its fixed-position amplitude by a constant times that exponential. Thus a further necessary condition is

$$
\boxed{\operatorname{Re}\gamma<0.}
$$

The [false complex saddle in dissipative cubic dispersion](../../../../../../../false-complex-saddle-in-dissipative-cubic-dispersion.md) illustrates why the second formal candidate cannot override this bound. For $\operatorname{Re}\alpha<0$, the neighborhood $k=0$ gives a fixed-position impulse response proportional to $e^{-\gamma t}/\sqrt t$: the cubic term is smaller on its $k=O(t^{-1/2})$ scale. It therefore supplies the usual growing pinch when $\operatorname{Re}\gamma<0$. The purely dispersive cases have stationary-phase algebraic prefactors instead. If $\beta=0$, only the quadratic stationary point remains; if both derivative coefficients vanish, the equation is local multiplication and its growth is directly $e^{-\gamma t}$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 79](../../../../paper-79-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
