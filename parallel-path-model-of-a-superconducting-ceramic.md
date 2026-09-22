# Parallel-path model of a superconducting ceramic

↑ **Parent:** [Transport and magnetic tests of superconducting ceramics](transport-and-magnetic-tests-of-superconducting-ceramics.md)

Consider an original [electrical circuit](electrical-circuit-split.md) model between two equipotential cross-sections. A normal path has [electrical resistance](electrical-resistance.md) $R_n>0$. Let $b\in\{0,1\}$ indicate whether an additional path connects those same cross-sections; when connected it has [electrical resistance](electrical-resistance.md) $r\geq0$. Ideal voltage contacts measure those cross-sections. This collapses a spatial network to two parallel branches; it is not a fit to the [Bednorz-Müller experiment](bednorz-muller-experiment.md).

For $r>0$, both branches have the same [electric potential difference](electric-potential-difference.md) $V$. [Ohm's law](ohm-s-law.md) and the [Kirchhoff node law](kirchhoff-node-law.md) give $I=V/R_n+bV/r$, hence

$$
R_{\mathrm{eff}}=\begin{cases}
R_n,&b=0,\\
\dfrac{R_n r}{R_n+r},&b=1,\ r>0,\\
0,&b=1,\ r=0.
\end{cases}
$$

The last case follows directly from the ideal short's constraint $V=0$, provided it can carry the imposed [electric current](electric-current.md) below its [superconducting critical current](superconducting-critical-current.md). It does not follow by substituting $r=0$ into $V/r$. A normal bridge in series with otherwise superconducting pieces belongs in $r$; superconducting grains alone need not short the measured interval.

<a id="image-equal-superconducting-volume-fractions-can-have-different-transport-connectivity"></a>
![](superconducting-ceramic-connectivity-and-volume-fraction.png)

**[Figure 11](#image-equal-superconducting-volume-fractions-can-have-different-transport-connectivity). Equal superconducting volume fractions can have different transport connectivity**. Original chosen geometry and circuit example, not measured data or a historical fit. Top: blue superconducting regions between orange equipotential ends, taken uniform through the thickness, have superconducting [phase fraction](phase-fraction.md) $f=0.08$. Bottom: two stipulated connectivity thresholds, $f_c=0.08$ and $0.60$, produce different apparent [electrical resistance](electrical-resistance.md) drops. Ideal zero values are displayed at a chosen instrument floor; these curves predict neither [magnetic susceptibility](magnetic-susceptibility.md) nor a universal [percolation](percolation-theory-split.md) threshold.

Choose $R_n=1\,\Omega$. A connected bridge with $r=0.01\,\Omega$ gives $R_{\mathrm{eff}}=1/101\,\Omega\simeq9.901\,\mathrm{m\Omega}$, almost a hundredfold drop despite finite [electrical resistance](electrical-resistance.md). An ideal connected superconducting filament instead gives zero in this model even when its volume is a small part of the specimen. Isolated superconducting islands can have the same superconducting [phase fraction](phase-fraction.md) $f$ while leaving $b=0$. For the illustrative disconnected geometry we stipulate that the normal conducting network retains $R_n$.

To plot a chosen connectivity sequence, set $b(f)=0$ for $f<f_c$ and $b(f)=1$ for $f\geq f_c$, with $r=0$ on the connected branch. The two displayed values of $f_c$ describe different chosen architectures. A real [percolation](percolation-theory-split.md) calculation would need an explicit network and spatial distribution; the scalar [phase fraction](phase-fraction.md) $f$ does not determine $b$ by itself.

An instrument with unresolved [electric potential difference](electric-potential-difference.md) bounded by $\delta V$ reports only $R_{\mathrm{eff}}\lesssim\delta V/|I|$. For chosen $I=1\,\mathrm{mA}$ and $\delta V=100\,\mathrm{nV}$ this floor is $10^{-4}\,\Omega$, assuming offsets and noise are included in the bound. The figure clips smaller model values to that floor. Increasing $|I|$ improves this formal bound only while [Joule heating](joule-heating.md) and the path's [superconducting critical current](superconducting-critical-current.md) remain controlled. None of these transport statements determines the superconducting [phase fraction](phase-fraction.md) or establishes complete [Meissner effect](meissner-effect.md) shielding.

## ↑ Ancestors (7)

1. [Transport and magnetic tests of superconducting ceramics](transport-and-magnetic-tests-of-superconducting-ceramics.md)
2. [High-temperature superconductivity](high-temperature-superconductivity.md)
3. [Superconductivity](superconductivity-split.md)
4. [Statistical physics](statistical-physics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [High-temperature superconductivity](high-temperature-superconductivity.md)
