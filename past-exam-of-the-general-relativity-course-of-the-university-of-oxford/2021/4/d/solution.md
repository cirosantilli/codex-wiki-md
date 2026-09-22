<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

For monotonically expanding [scale factor](../../../../scale-factor-cosmology.md) $R$, $dt=dR/(RH)$, so the elapsed [cosmic time](../../../../cosmic-time.md) is

$$
\boxed{t_0-t_i=\int_{R_i}^{R_0}\frac{dR}{R\,H(R)}
=\int_0^{z_i}\frac{dz}{(1+z)H(z)}.}
$$

The second expression uses [cosmological redshift](../../../../cosmological-redshift.md) $1+z=R_0/R$; the [age of the universe](../../../../age-of-the-universe.md) is the limit to its earliest specified state, if that limit is finite.

An [age comparison for an initial vacuum-dominated phase](../../../../age-comparison-for-an-initial-vacuum-dominated-phase.md) needs a common normalization. Match the two histories at the end of S1, with $R=R_1$ and $H=H_1>0$, and give them identical subsequent S2 and S3 evolution, including transition radii and today's state. Below $R_1$, the history with S1 has constant $H=H_1$. The comparison history extends S2 backwards, so $\rho\propto R^{-4}$ and $H=H_1(R_1/R)^2$. Starting both at $R_i=\epsilon R_1$, where $0<\epsilon<1$, their early durations are

$$
\Delta t_{\rm S1}=\frac1{H_1}\ln\frac1\epsilon,\qquad
\Delta t_{\rm S2}=\int_{\epsilon R_1}^{R_1}\frac{R\,dR}{H_1R_1^2}
=\frac{1-\epsilon^2}{2H_1}.
$$

The difference is positive because

$$
\boxed{\Delta t_{\rm S1}-\Delta t_{\rm S2}
=\frac1{H_1}\int_\epsilon^1\left(\frac1x-x\right)dx>0.}
$$

The common later evolution adds the same time to both histories. Thus S1 makes this matched universe older. More strongly, as $R_i\to0$, the exact S1 duration diverges logarithmically, whereas a radiation beginning has finite duration $1/(2H_1)$ to the match. The exact [de Sitter spacetime](../../../../de-sitter-spacetime.md) expanding patch reaches $R=0$ only as $t\to-\infty$ for its [comoving observers](../../../../comoving-observer.md); a finite “age since $R=0$” does not exist in this ideal model. This does not establish past [geodesic completeness](../../../../geodesic-completeness.md) of the patch.

The matching assumption is essential for a finite cutoff or realistic finite period of [cosmic inflation](../../../../cosmic-inflation-split.md): arbitrary changes of the present [Hubble parameter](../../../../hubble-parameter.md) or transition densities prevent a universal age comparison. The literal zero-size limit in this question is instead the infinite-duration idealization just derived.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the general relativity course of the University of Oxford](../../../split.md)
5. [General relativity course of the University of Oxford](../../../../general-relativity-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
