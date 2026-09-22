# Magnetic field of a finite straight wire

↑ **Parent:** [Biot-Savart law](biot-savart-law.md)

Take a wire segment on the $y$ axis, with source positions $\mathbf r'=(0,s,0)$ for $s_1\le s\le s_2$, and positive [electric current](electric-current.md) along $+y$. Observe at $\mathbf r=(a,0,0)$, where $a>0$ is the perpendicular distance to the wire's supporting line. Choose $x$ rightward and $y$ upward, so $+z$ points out of the page. Then

$$
d\boldsymbol\ell'=\widehat{\mathbf y}\,ds,\qquad
\mathbf R=a\widehat{\mathbf x}-s\widehat{\mathbf y},\qquad
d\boldsymbol\ell'\times\mathbf R=-a\widehat{\mathbf z}\,ds.
$$

Thus the [magnetic field](magnetic-field-split.md) points into the page by the [right-hand rule](right-hand-rule.md). The [Biot-Savart law](biot-savart-law.md) and an elementary [antiderivative](antiderivative.md) give

$$
\mathbf B=-\frac{\mu_0 I a}{4\pi}\widehat{\mathbf z}
\int_{s_1}^{s_2}\frac{ds}{(a^2+s^2)^{3/2}}
=-\frac{\mu_0I}{4\pi a}
\left[\frac{s}{\sqrt{a^2+s^2}}\right]_{s_1}^{s_2}\widehat{\mathbf z}.
$$

For an original worked example, choose $s_1=-0.12\,\mathrm m$, $s_2=0.12\,\mathrm m$, $a=0.05\,\mathrm m$, and $I=3\,\mathrm A$. Use $\mu_0\approx4\pi\times10^{-7}\,\mathrm{T\,m/A}$ for these rounded calculations. Each endpoint contributes $0.12/0.13=12/13$, so

$$
\mathbf B=-\frac{(10^{-7}\,\mathrm{T\,m/A})(3\,\mathrm A)}{0.05\,\mathrm m}
\frac{24}{13}\,\widehat{\mathbf z}
\approx-11.08\,\mu\mathrm T\,\widehat{\mathbf z}.
$$

These are calculated inputs and output, not laboratory data. The two endpoint [angles](angle.md) measured from the perpendicular each have [sine](sine.md) $12/13$; this recovers the equivalent endpoint-angle formula without depending on a diagram's angle-sign convention.

<a id="image-finite-wire-biot-savart-law-source-geometry-orientation-and-the-long-wire-limit"></a>
![](biot-savart-finite-wire-geometry.png)

**[Figure 18](#image-finite-wire-biot-savart-law-source-geometry-orientation-and-the-long-wire-limit). Finite-wire Biot-Savart law: source geometry, orientation and the long-wire limit**. Original geometry for the $0.24\,\mathrm m$ segment and $0.05\,\mathrm m$ observation distance. The [electric current](electric-current.md) is upward; the [magnetic field](magnetic-field-split.md) at P points into the page. The right panel shows the calculated midpoint ratio $B_{\rm segment}/B_{\rm infinite}=L/\sqrt{a^2+L^2}$ versus half-[length](length.md) divided by distance, with the example marked at $L/a=2.4$.

For a segment centered on the perpendicular foot, $s_1=-L$, $s_2=L$. Its [magnetic field](magnetic-field-split.md) magnitude is

$$
B=\frac{\mu_0I}{2\pi a}\frac{L}{\sqrt{a^2+L^2}}.
$$

The [limit](limit-of-a-function.md) $L/a\to\infty$ gives $B_\infty=\mu_0I/(2\pi a)$, consistent with [Ampère's circuital law](ampere-s-circuital-law.md) for an infinite straight wire. In the example, $B_\infty=12\,\mu\mathrm T$ and $B/B_\infty=12/13$: the infinite-wire value overestimates the segment value by $1/12$, or about $8.33\%$ of the segment value. For $a\gg L$, the isolated segment contribution instead behaves as $B\sim\mu_0I(2L)/(4\pi a^2)$. The complete localized [electrical circuit](electrical-circuit-split.md) has a different far-field behavior: return-path contributions cancel this leading segment term, leaving a [magnetic dipole field](magnetic-dipole-field.md) when its [magnetic dipole moment](magnetic-dipole-moment.md) is nonzero. Segment and whole-circuit limits must be distinguished.

The [SI](international-system-of-units.md) units check directly: $\mu_0I/a$ has units $(\mathrm{T\,m/A})\mathrm A/\mathrm m=\mathrm T$, the [tesla](tesla-unit.md). The apparent divergence as $a\to0$ is a failure of the thin-wire model near the conductor, not a prediction of infinite [magnetic field](magnetic-field-split.md) inside a real wire. This calculation gives only this segment's contribution; include the return wires before comparing with an apparatus.

## ↑ Ancestors (5)

1. [Biot-Savart law](biot-savart-law.md)
2. [Electromagnetism](electromagnetism-split.md)
3. [Branches of physics](branches-of-physics.md)
4. [Physics](physics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Biot-Savart law](biot-savart-law.md)
