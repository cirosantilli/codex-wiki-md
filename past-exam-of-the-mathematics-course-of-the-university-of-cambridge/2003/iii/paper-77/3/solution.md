<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Take an attractive nonretarded molecular potential $U(R)=-\beta/R^6$, with molecular number densities $n_1,n_2$. Its force magnitude is $6\beta/R^7$. For one molecule at height $z$ above a half-space, integration over cylindrical radius and depth gives

$$
U_2(z)=-n_2\beta\int_0^\infty\!\int_0^\infty
\frac{2\pi r\,dr\,ds}{[r^2+(z+s)^2]^3}
=-\frac{\pi n_2\beta}{6z^3}.
$$

Its downward force is $\pi n_2\beta/(2z^4)$. A sphere's horizontal cross-section a distance $y$ above its bottom has area $\pi(2ay-y^2)$, so its total attractive force is

$$
F_{12}=\frac{\pi^2n_1n_2\beta}{2}\int_0^{2a}
\frac{2ay-y^2}{(d_0+y)^4}\,dy.
$$

For $d_0\ll a$ the near-bottom region dominates. Replacing its area by $2\pi ay$ and extending the upper limit gives

$$
F_{12}\sim\pi^2n_1n_2\beta a\int_0^\infty\frac{y\,dy}{(d_0+y)^4}
=\boxed{\frac{A_{12}a}{6d_0^2}},\qquad A_{12}=\pi^2n_1n_2\beta.
$$

This derives the [sphere-plane dispersion force](../../../../../sphere-plane-dispersion-force.md) from the pairwise [Van der Waals force](../../../../../van-der-waals-force.md). Hereafter $A>0$ denotes the magnitude of the effective _repulsive_ interaction across water, rather than the signed attractive [Hamaker constant](../../../../../hamaker-constant.md). Its planar [pressure](../../../../../pressure.md) magnitude is $\Pi(d)=A/(6\pi d^3)$.

For a nearly planar freezing front, the spherical gap is $d(r)=d_0+r^2/(2a)$. In the particle frame the incoming normal motion has speed $V$. Axisymmetric [mass conservation](../../../../../mass-conservation.md) gives the outward gap flux per circumference $q_r=Vr/2$. The [lubrication](../../../../../lubrication-theory.md) flux law therefore gives

$$
\frac{dp}{dr}=-\frac{6\mu Vr}{d(r)^3},\qquad
p(r)=\frac{3\mu Va}{d(r)^2},\quad p(\infty)=0.
$$

Integrating its axial force gives

$$
F_\mu=2\pi\int_0^\infty p(r)r\,dr=\frac{6\pi\mu Va^2}{d_0}.
$$

Steady [particle pushing by a freezing front](../../../../../particle-pushing-by-a-freezing-front.md) requires $F_\mu=Aa/(6d_0^2)$, and hence

$$
\boxed{V=\frac{A}{36\pi\mu a d_0}.}
$$

The viscous drag is not the isolated-sphere Stokes drag: its divergence as the gap closes is essential.

For the deformed interface let $c=\cos\theta_0$ and measure $\theta$ from the sphere's downward pole, as in the original geometry. The height below the remote melting isotherm is $a(\cos\theta-c)$. Under the imposed [temperature](../../../../../temperature.md) gradient, the undercooling is $Ga(\cos\theta-c)$. With capillary depression neglected, the local phase-equilibrium [pressure](../../../../../pressure.md) is

$$
\Pi=\frac{\rho LG}{T_m}a(\cos\theta-c)=\frac{A}{6\pi d^3}.
$$

Here $T_m$ is the absolute melting [temperature](../../../../../temperature.md); a constant reference ice [density](../../../../../density.md) is used in the thermomolecular relation. Thus

$$
\boxed{d^3(\theta)=\frac{K}{\cos\theta-c},\qquad
K=\frac{AT_m}{6\pi\rho LGa}.}
$$

The numerical value of $K$ will cancel from the speed relation.

In the thin spherical film, incompressibility and the incoming normal velocity $V\cos\theta$ give

$$
\frac{1}{a\sin\theta}\frac{d}{d\theta}[\sin\theta\,q(\theta)]=V\cos\theta,
\qquad q(\theta)=\frac{Va\sin\theta}{2}.
$$

Symmetry supplies zero pole flux. The tangential Couette contribution is smaller by $d/a$ and is negligible at this order. Applying the pressure-driven flux law along arclength $a\theta$ gives

$$
\frac{dp}{d\theta}=-\frac{6\mu Va^2\sin\theta}{d^3(\theta)},\qquad
p(\theta)=\frac{3\mu Va^2}{K}(\cos\theta-c)^2,
$$

where [pressure](../../../../../pressure.md) is matched to the outer liquid at $\theta_0$.

A cap area element is $2\pi a^2\sin\theta\,d\theta$ and its vertical normal component is $\cos\theta$. Put $y=\cos\theta$. The upward molecular and downward hydraulic forces are therefore

$$
\begin{aligned}
F_A&=\frac{Aa^2}{3K}\int_c^1y(y-c)\,dy
=\frac{Aa^2}{18K}(2-3c+c^3),\\
F_\mu&=\frac{6\pi\mu Va^4}{K}\int_c^1y(y-c)^2\,dy
=\frac{\pi\mu Va^4}{2K}(3-8c+6c^2-c^4).
\end{aligned}
$$

Balancing these forces establishes [premelted-film particle pushing](../../../../../premelted-film-particle-pushing.md):

$$
\boxed{V=\frac{A}{9\pi\mu a^2}
\frac{2-3c+c^3}{3-8c+6c^2-c^4}
=\frac{A}{9\pi\mu a^2}\frac{c+2}{(1-c)(c+3)}.}
$$

The factorizations are $(1-c)^2(c+2)$ and $(1-c)^3(c+3)$. They confirm positivity on the physical cap range and provide a numerically better-conditioned shallow-cap expression. Since $h=a(1-c)$, the shallow-cap limit within $d\ll h$ is $V\sim A/(12\pi\mu ah)$; it is not a limit in which the film can be identified with the flat-front gap $d_0$.

The local film formula diverges right at the rim $\theta_0$. Accordingly the thin-film calculation is an outer approximation away from a small matching fringe, not a claim of a uniformly thin film at its contact with bulk water. Both integrated [stress](../../../../../stress.md) densities vanish at that rim; in the thin-film limit the fringe contributes only a higher-order correction. Surface-tension [curvature](../../../../../curvature.md), altered thermal gradients or appreciable density-change fluxes would require a different balance.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
