<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use downward [optical depth](../../../../optical-depth.md) $t$ measured from the top, with total $D=\tau_\infty$. This is the effective optical-depth/[two-stream](../../../../two-stream-approximation.md) convention that gives an attenuation factor $e^{-t}$. Constant absorption per unit [mass](../../../../mass.md) and constant gravity give $t=Dp/p_s$. Write the locally emitted flux source as $S(t)=\pi B(t)=S_0+bt$.

The atmospheric contribution to upward outgoing longwave flux is

$$
F_{\rm atm}=\int_0^D S(t)e^{-t}\,dt
=S_0(1-e^{-D})+b[1-(D+1)e^{-D}].
$$

Because the source is linear, the [effective emission pressure](../../../../effective-emission-pressure.md) makes this exactly $(1-e^{-D})S(t_{\rm eff})$, where

$$
\boxed{t_{\rm eff}=\frac{1-(D+1)e^{-D}}{1-e^{-D}}
=1-\frac{D}{e^D-1},\qquad
p_{\rm rad}=\frac{p_s}{D}t_{\rm eff}.}
$$

Thus for $D\gg1$, $t_{\rm eff}\to1$ and $p_{\rm rad}\simeq p_s/D$. For $D\ll1$, expansion gives $t_{\rm eff}=D/2-D^2/12+O(D^4)$, so $p_{\rm rad}\simeq p_s/2$. In the thin limit $F_{\rm atm}\simeq D\,\pi B(p_s/2)$: it is the small atmospheric contribution, not the whole outgoing flux, which this level characterizes. Surface radiation transmitted through the column must be added separately.

**Angular convention:** these numerical coefficients use an effective [optical depth](../../../../optical-depth.md). If $t$ instead means literal vertical monochromatic [optical depth](../../../../optical-depth.md) and the angular [integral](../../../../integral-split.md) is retained exactly, the flux weight is $2E_2(t)$, not $e^{-t}$. Its thick-limit mean depth is $2/3$, giving $p_{\rm rad}\simeq2p_s/(3D)$ for a linear source. The coefficient one in the requested expression therefore specifies a [two-stream/diffusivity](../../../../two-stream-approximation.md) convention; it is not an angle-independent identity. The thin-limit half-column result survives to leading order.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the physics of atmospheres and oceans course of the University of Oxford](../../../split.md)
5. [Physics of atmospheres and oceans course of the University of Oxford](../../../../physics-of-atmospheres-and-oceans-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
