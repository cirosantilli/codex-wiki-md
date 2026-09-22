<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Equating the satellite's mean density inside $r_t$ with the host's mean density inside orbital radius $R$ gives

$$
\frac{m}{(4\pi/3)r_t^3}
\simeq\frac{M(<R)}{(4\pi/3)R^3},
\qquad
\boxed{r_t\simeq R\left(\frac m{M(<R)}\right)^{1/3}}.
$$

Thus a measured [tidal radius](../../../../../tidal-radius.md) and independently estimated satellite mass infer $M(<R)\simeq m(R/r_t)^3$. Measurements from satellites over a range of $R$ trace the host's enclosed-mass profile and hence its [gravitational potential](../../../../../newtonian-potential-of-a-point-mass.md). [Globular clusters](../../../../../globular-cluster.md) are more often tidally limited: their stellar extent can approach the Jacobi boundary, whereas [dwarf galaxies](../../../../../dwarf-galaxy.md) commonly occupy extended dark-matter haloes and their observed stars may substantially underfill it. Orbital eccentricity, mass loss, and nonequilibrium structure complicate this inference.

Let the separation vector point from the host to the satellite. Subtracting the two [Newton's second law](../../../../../newton-s-second-law.md) equations gives

$$
\boxed{\ddot{\mathbf d}
=-\frac{G(M+m)}{|\mathbf d|^3}\mathbf d}.
$$

The relative orbit is therefore a one-body [Kepler orbit](../../../../../kepler-orbit.md) with gravitational parameter $G(M+m)$. A circular orbit of separation $R_0$ has

$$
\boxed{\Omega^2=\frac{G(M+m)}{R_0^3}}.
$$

The centre-of-mass condition gives $x_m=MR_0/(M+m)$ for the satellite's distance from the barycentre.

Consider the inner collinear equilibrium a distance $r_J$ toward the host from the satellite. Taking the positive axis from the host toward the satellite, differentiation of the gravitational plus centrifugal [effective potential](../../../../../effective-potential.md) gives

$$
0=\frac{Gm}{r_J^2}
-\frac{GM}{(R_0-r_J)^2}
+\Omega^2(x_m-r_J).
$$

Since $r_J\ll R_0$,

$$
\frac1{(R_0-r_J)^2}
=\frac1{R_0^2}\left(1+\frac{2r_J}{R_0}
+O\left(\frac{r_J^2}{R_0^2}\right)\right).
$$

The constant host-gravity term cancels $\Omega^2x_m=GM/R_0^2$. The remaining equation is

$$
\frac{Gm}{r_J^2}
-\frac{G(3M+m)}{R_0^3}r_J=0.
$$

For a low-mass satellite, the term proportional to $m r_J$ is negligible compared with $3Mr_J$, and the [Jacobi tidal radius](../../../../../jacobi-tidal-radius.md) is

$$
\boxed{r_J=R_0\left(\frac m{3M}\right)^{1/3}}.
$$

The outer collinear point gives the same leading result.

Stars that cross the two nearby [Lagrange points](../../../../../lagrange-point.md) are no longer bound to the satellite. Small energy and angular-momentum offsets place them on slightly different host orbits, producing one leading and one trailing [tidal tail](../../../../../tidal-tail.md). Differential orbital frequency stretches these streams around the host, while epicyclic motion can create density clumps. The tail's position and velocity structure retain information about the satellite orbit and host potential.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 349](../../paper-349-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
