<h1 id="section-a/1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [polymer overlap concentration](../../../../../polymer-overlap-concentration.md) is reached when there is roughly one chain per coil volume. If $M$ is the chain [molar mass](../../../../../molar-mass.md), choose the explicit geometric convention $V_{\mathrm{coil}}=4\pi R_g^3/3$, where $R_g$ is the [radius of gyration](../../../../../radius-of-gyration.md). Then

$$
\boxed{c^*\simeq\frac{M}{N_A(4\pi/3)R_g^3}}.
$$

Here $c^*$ is mass per solution volume and $N_A$ is the [Avogadro constant](../../../../../avogadro-constant.md). A [good solvent](../../../../../good-solvent.md) gives $R_g\propto N^\nu$ with $\nu\simeq0.588$, approximated by $3/5$ in the [Flory approximation](../../../../../flory-approximation.md). With a [polystyrene](../../../../../polystyrene.md) repeat-unit molar mass of about $104.15\,\mathrm{g\,mol^{-1}}$, the chain has approximately $N=960$ repeat units. This fixes the chain length but not the size amplitude: the problem supplies no statistical segment length or measured coil size.

For a numerical estimate, use the [good-solvent size calibration for polystyrene](../../../../../good-solvent-size-calibration-for-polystyrene.md),

$$
\frac{R_g}{\mathrm{nm}}\simeq0.0123\left[\frac{M}{\mathrm{g\,mol^{-1}}}\right]^{0.593}.
$$

This empirical calibration is quoted for benzene or toluene near room temperature at molar masses above $2\times10^5\,\mathrm{g\,mol^{-1}}$; using it here is a modest extrapolation to $M=10^5\,\mathrm{g\,mol^{-1}}$. It gives $R_g\simeq11.3\,\mathrm{nm}$. Thus

$$
c^*\simeq\frac{100\,\mathrm{kg\,mol^{-1}}}{(6.022\times10^{23}\,\mathrm{mol^{-1}})(4\pi/3)(11.3\times10^{-9}\,\mathrm m)^3}
\simeq\boxed{3\times10^1\,\mathrm{kg\,m^{-3}}\simeq3\times10^1\,\mathrm{g\,L^{-1}}}.
$$

The unrounded calibration gives about $27\,\mathrm{g\,L^{-1}}$. This is an estimate under a stated extra material input, not a unique number determined solely by molecular weight and the phrase good solvent. Choosing a different coil-volume convention changes its prefactor. The robust chain-length dependence is $c^*\propto M^{1-3\nu}\simeq M^{-4/5}$ for a flexible good-solvent coil.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [1](../../1.md)
3. [Section A](../../../section-a.md)
4. [2018](../../../../2018-split.md)
5. [Past exam of the soft condensed matter course of the University of Cambridge](../../../../split.md)
6. [Soft Condensed Matter course of the University of Cambridge](../../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
