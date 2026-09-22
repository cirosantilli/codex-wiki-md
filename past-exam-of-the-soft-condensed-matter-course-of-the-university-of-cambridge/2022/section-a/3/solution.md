<h1 id="section-a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Treat the [liposome](../../../../liposome.md) using the usual incompressible-tail packing model of a [lipid bilayer](../../../../lipid-bilayer.md): neglect the head-group thickness and let $v$ be the volume filling the hydrophobic part of the [lipid vesicle](../../../../lipid-vesicle.md). Both [membrane leaflets](../../../../membrane-leaflet.md) have area $a$ per head group. Put $d=v/a$, and let $R$ be the unknown outer radius. Counting [molecules](../../../../molecule-split.md) from the inner and outer [surface areas](../../../../surface-area.md) gives

$$
M_i=\frac{4\pi r_i^2}{a},\qquad M_o=\frac{4\pi R^2}{a}.
$$

Equating the total molecular volume to the volume of the [spherical shell](../../../../spherical-shell.md) therefore gives

$$
\frac{4\pi}{3}(R^3-r_i^3)=v(M_i+M_o),\qquad
\boxed{R^3-r_i^3=3d(R^2+r_i^2).}
$$

To prove uniqueness in the physical domain $R>r_i>0$, define

$$
q(R)=\frac{R^3-r_i^3}{R^2+r_i^2}.
$$

Its [derivative](../../../../derivative.md) is

$$
q'(R)=\frac{R^4+3R^2r_i^2+2Rr_i^3}{(R^2+r_i^2)^2}>0.
$$

Also $q(r_i)=0$ and $q(R)\to\infty$ as $R\to\infty$. By [continuity](../../../../continuous-function.md) and strict [monotonicity](../../../../monotonic-function.md), $q(R)=3d$ has **exactly one solution with $R>r_i$**. This proves the required uniqueness without choosing among ambiguous branches of a cubic formula.

The maximum tail length is a physical admissibility bound, not automatically the actual leaflet thickness. If $r_m$ is the radius where the two tail regions meet, separate [membrane leaflet](../../../../membrane-leaflet.md) volume balances give

$$
r_m^3=r_i^3+3d r_i^2,\qquad
R^3-r_m^3=3d R^2.
$$

The unique candidate must satisfy

$$
\boxed{r_m-r_i\leq l,\qquad R-r_m\leq l.}
$$

In particular $R-r_i\leq2l$ is necessary. The premise that a [lipid vesicle](../../../../lipid-vesicle.md) has assembled supplies this compatibility: arbitrary positive choices of $r_i,v,a,l$ need not allow any such [lipid bilayer](../../../../lipid-bilayer.md). For a very large vesicle the two thicknesses tend to $d$, so $R-r_i\simeq2v/a$. Setting the thickness equal to $2l$ for every [molecule](../../../../molecule-split.md) would confuse maximum extension with actual packing. The volume-balance argument and its domain are an example of [uniqueness of the packed spherical bilayer radius](../../../../uniqueness-of-the-packed-spherical-bilayer-radius.md).

## ↑ Ancestors (13)

1. [3](../3.md)
2. [Section A](../../section-a.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the soft condensed matter course of the University of Cambridge](../../../split.md)
5. [Soft Condensed Matter course of the University of Cambridge](../../../../soft-condensed-matter-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
