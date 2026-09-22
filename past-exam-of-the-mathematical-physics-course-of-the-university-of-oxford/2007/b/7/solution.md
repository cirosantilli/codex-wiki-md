<h1 id="b/7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

The coordinate [derivatives](../../../../derivative.md) of the smooth two-parameter map commute. With a torsion-free [Levi-Civita connection](../../../../levi-civita-connection.md),

$$
\frac{DY^a}{Ds}=\frac{\partial^2x^a}{\partial s\partial\tau}+\Gamma^a{}_{bc}V^bY^c
=\frac{DV^a}{D\tau},
$$

because $\Gamma^a{}_{bc}$ is symmetric in its lower indices. Each member of the family is a [geodesic](../../../../geodesic.md), so $DV/Ds=0$. Consequently

$$
\frac{D^2Y^d}{Ds^2}=\frac D{Ds}\frac D{D\tau}V^d
=\left(\frac D{Ds}\frac D{D\tau}-\frac D{D\tau}\frac D{Ds}\right)V^d.
$$

The [commutator](../../../../commutator.md) of [covariant derivatives](../../../../covariant-derivative.md) is the action of the [Riemann curvature tensor](../../../../riemann-curvature-tensor-split.md). With the source's index and sign convention this gives

$$
\boxed{\frac{D^2Y^d}{Ds^2}=R_{abc}{}^dV^aY^bV^c.}
$$

This is [geodesic deviation](../../../../geodesic-deviation.md): [free fall](../../../../free-fall.md) relative acceleration measures [curvature](../../../../curvature.md), even where an individual observer can eliminate the connection at one point.

For Earth's exterior Newtonian field, $\phi=-GM/r$ and acceleration is $a_i=-\partial_i\phi$. Nearby freely falling particles have relative acceleration $\delta a_i=-\phi_{,ij}Y^j$. At the observation point align $z$ radially upward and $x,y$ horizontally. Since $GM/R_E^2=g$,

$$
-\phi_{,ij}=\frac g{R_E}\operatorname{diag}(-1,-1,2).
$$

The weak-field [geodesic](../../../../geodesic.md)-deviation equation therefore identifies

$$
\boxed{R_{010}{}^1\simeq-\frac g{R_E},\quad R_{020}{}^2\simeq-\frac g{R_E},\quad
R_{030}{}^3\simeq\frac{2g}{R_E}.}
$$

In these units time is measured in seconds as in the stated Newtonian comparison; if the zeroth coordinate is $ct$ instead, the [curvature](../../../../curvature.md) components acquire the corresponding $c^{-2}$ factor. A small freely falling cloud is squeezed in the two horizontal directions and stretched radially. These are tidal effects, not the uniform acceleration removed by a freely falling frame.

Their characteristic inverse-square time is $g/R_E$, so $\boxed{t_{\rm tide}=\sqrt{R_E/g}\simeq8.1\times10^2\ {\rm s}\simeq13.4\ {\rm min}}$. One concrete thought experiment is an ideal satellite moving in a [circular orbit](../../../../circular-orbit.md) just above a spherical Earth, ignoring atmosphere and terrain. Its orbital [angular frequency](../../../../angular-frequency.md) is $\sqrt{GM/R_E^3}=\sqrt{g/R_E}$ and its period is $2\pi t_{\rm tide}\simeq84$ minutes. Equivalently, initially nearby [free fall](../../../../free-fall.md) trajectories develop order-one tidal changes on this characteristic scale. This is the [surface tidal time scale of a spherical gravitating body](../../../../surface-tidal-time-scale-of-a-spherical-gravitating-body.md).

## ↑ Ancestors (12)

1. [7](../7.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the mathematical physics course of the University of Oxford](../../../split.md)
5. [Mathematical physics course of the University of Oxford](../../../../mathematical-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
