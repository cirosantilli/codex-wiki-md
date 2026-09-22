<h1 id="section-b/b6/solution">Solution</h1>

↑ **Parent:** [B6](../b6.md)

Take $m,k,b>0$, and define $\omega_0=\sqrt{k/m}$ and $\gamma=b/(2m)$. Substitution of $e^{rt}$ into the unforced equation gives $r^2+2\gamma r+\omega_0^2=0$. The roots determine whether the return is oscillatory.

For return after a [displacement](../../../../../displacement.md) in this ideal model, **[critical damping](../../../../../critical-damping.md), case (b), is the usual comfort choice**: it removes repeated bouncing while avoiding the slow relaxation mode of strong [overdamping](../../../../../overdamping.md). For release from rest it gives a monotone return with the fastest asymptotic decay available without oscillation. This criterion does not prove optimal comfort for every road profile or initial [velocity](../../../../../velocity.md); actual comfort also depends on [acceleration](../../../../../acceleration.md), road forcing and suspension travel.

For the forced response, set $\Omega=2\pi u/d$ and use $x_{\rm ss}=\operatorname{Re}(\widehat x e^{i\Omega t})$. Then

$$
(k-m\Omega^2+ib\Omega)\widehat x=kA,\qquad
\boxed{x_{\rm ss}(t)=X(\Omega)\cos(\Omega t-\delta),}
$$



$$
X(\Omega)=\frac{kA}{\sqrt{(k-m\Omega^2)^2+b^2\Omega^2}},\qquad
\delta=\operatorname{atan2}(b\Omega,k-m\Omega^2).
$$

The general forced solution adds the appropriate homogeneous transient from (a), (b) or (c). Initial data were not specified, so its constants cannot be fixed. Positive [damping](../../../../../damping.md) removes this transient at long times. This solution uses the particular driving [force](../../../../../force-split.md) in the supplied equation; it does not silently replace it by a different moving-support model.

Maximising $X$ is minimising its squared denominator $D$. Differentiation gives

$$
\frac{dD}{d\Omega}=2\Omega[-2mk+2m^2\Omega^2+b^2],\qquad
\Omega_r^2=\frac{k}{m}-\frac{b^2}{2m^2}.
$$

A nonzero [displacement](../../../../../displacement.md) [resonance](../../../../../resonance.md) exists only if $b^2<2mk$. Here $\Omega_r^2=0.175\,\mathrm{s^{-2}}$, and therefore

$$
\boxed{u_r=\frac{d}{2\pi}\sqrt{0.175}=0.666\,\mathrm{m\,s^{-1}}\simeq2.40\,\mathrm{km\,h^{-1}},}
$$



$$
\boxed{X_{\max}=\frac{kA}{b\sqrt{k/m-b^2/(4m^2)}}=0.0616\,\mathrm m.}
$$

The low-frequency limit is $X(0)=A$, whereas $X\to0$ at large $\Omega$. The parameters give [damping ratio](../../../../../damping-ratio.md) $\zeta=b/(2\sqrt{mk})=0.456$, consistent with an underdamped system and the existence of this amplitude maximum.

## ↑ Ancestors (14)

1. [B6](../b6.md)
2. [Section B](../../section-b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2015](../../../split.md)
5. [Past exam of the physics A course of the University of Cambridge](../../../../split.md)
6. [Physics A course of the University of Cambridge](../../../../../physics-a-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
