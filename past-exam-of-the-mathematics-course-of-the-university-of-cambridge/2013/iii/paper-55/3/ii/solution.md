<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the supplied cosmological [cosmic baryon fraction](../../../../../../cosmic-baryon-fraction.md) $f_b=\Omega_{\rm bar}/\Omega_{\rm mat}=0.2$, and assume the halo initially has that fraction. Its total baryon mass is then $M_{b,\rm tot}=6\times10^{11}M_\odot$. The selected baryons are the lowest-angular-momentum fraction

$$
f_j=\frac{3\times10^9M_\odot}{6\times10^{11}M_\odot}=0.005.
$$

Here the given cumulative [specific angular momentum](../../../../../../specific-angular-momentum.md) distribution must be normalized separately for the baryon component: equal baryon and dark-matter distributions mean equal normalized fractions, not equal absolute masses.

The [virial velocity](../../../../../../virial-velocity-of-a-spherical-overdensity-halo.md) and the largest specific angular momentum in the selected inner baryon population are

$$
V_{\rm vir}=\sqrt{\frac{G(3\times10^{12}M_\odot)}{53\,\mathrm{kpc}}}\simeq493\,\mathrm{km\,s^{-1}},\qquad
j_{\rm vir}=0.1r_{\rm vir}V_{\rm vir}\simeq2.62\times10^3\,\mathrm{kpc\,km\,s^{-1}},
$$



$$
j_d=f_jj_{\rm vir}\simeq13.1\,\mathrm{kpc\,km\,s^{-1}}.
$$

Estimate the outer radius of the settled low-angular-momentum component using circular rotational support and an enclosed-mass approximation to its self-gravity. With negligible dark matter inside the component, $v_d^2\simeq GM_b/r_d$ and $j_d=r_dv_d$, so

$$
\boxed{r_d\simeq\frac{j_d^2}{GM_b}\simeq0.013\,\mathrm{kpc}\simeq13\,\mathrm{pc},\qquad
v_d\simeq\frac{GM_b}{j_d}\simeq10^3\,\mathrm{km\,s^{-1}}.}
$$

The given rounded gravitational constant produces the same estimate. The very small radius follows from selecting a small low-$j$ fraction, rather than assigning all central baryons the halo-edge angular momentum.

These estimates assume that gas radiates energy, preserves each parcel's [specific angular momentum](../../../../../../specific-angular-momentum.md), and settles with negligible pressure support and no strong redistribution or cancellation of its angular-momentum vectors. They also assume that the phrase “innermost baryons” selects the lowest-$j$ material, the original cosmic baryon supply is retained, and the central gas supplies the dominant gravity. A possible central black hole or an exact flattened disk potential changes the numerical coefficient; the stated baryonic mass is used for this estimate.

The [low-angular-momentum baryonic disk estimate](../../../../../../low-angular-momentum-baryonic-disk-estimate.md) uses a cumulative distribution uniform in $j$ from zero to $j_d$, so its mean is $j_d/2$. The quoted $r_d$ is the outer radius based on the cutoff angular momentum, not a one-zone radius based on the mean. Within the same enclosed-mass approximation, $M(<j)=M_bj/j_d$ and circular balance give $r(j)=jj_d/(GM_b)$: the rotation curve is approximately flat and the half-mass radius is $r_d/2$. Treating every baryon as one shell with the mean $j$ would instead give $r_d/4$ and twice the velocity, a different radius convention rather than the outer edge of the supplied distribution.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 55](../../../paper-55-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
