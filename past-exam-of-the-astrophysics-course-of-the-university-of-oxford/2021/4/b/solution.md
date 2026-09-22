<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Conservation of the comoving galaxy population gives $n(z)=n_0a^{-3}=n_0(1+z)^3$. Holding the proper galaxy radius fixed, integrate [a](../a.md):

$$
\tau(z_s)=\frac{c\pi r_G^2n_0}{H_0}\int_0^{z_s}(1+z)^{1/2}dz
=\boxed{\frac{2c\pi r_G^2n_0}{3H_0}\left[(1+z_s)^{3/2}-1\right].}
$$

With $r_G=0.015\ \mathrm{Mpc}$, $n_0=0.01\ \mathrm{Mpc^{-3}}$, and $c/H_0=4282.75\ \mathrm{Mpc}$, set $C=c\pi r_G^2n_0/H_0=0.030273$. Consequently

$$
\boxed{\tau(1)=0.0369013.}
$$

For random uncorrelated intersections, the zero-intersection probability is $e^{-\tau}$ from the [Poisson distribution](../../../../poisson-distribution.md), so the fraction of the sky covered by foreground galaxies _out to_ $z=1$ is

$$
\boxed{f=1-e^{-\tau(1)}=0.03623\simeq3.6\%.}
$$

Ignoring overlaps gives $f\simeq\tau\simeq3.7\%$. A literal shell of zero thickness exactly at $z=1$ has zero coverage; the integrated foreground interpretation is needed. Clustering changes the exact overlap probability, although the mean [optical depth](../../../../optical-depth.md) above still follows from the mean [number density](../../../../number-density.md).

Finally,

$$
\boxed{\tau=1\quad\Longrightarrow\quad z_s=\left(1+\frac3{2C}\right)^{2/3}-1=12.67.}
$$

At this [optical depth](../../../../optical-depth.md), the Poisson sky coverage is $1-e^{-1}\simeq63\%$, not $100\%$. The large inferred [cosmological redshift](../../../../cosmological-redshift.md) extrapolates conserved galaxy counts and fixed radii far beyond their plausible physical range; it is the answer within the prescribed toy model.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [4](../../4.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the astrophysics course of the University of Oxford](../../../split.md)
5. [Astrophysics course of the University of Oxford](../../../../astrophysics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
