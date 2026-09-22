<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

In the [Rational map approximation for Skyrmions](../../../../../rational-map-approximation-for-skyrmions.md), stereographic coordinate $z$ describes the direction $\widehat{\mathbf x}\in S^2$, and a degree-$B$ rational map $R(z)=p(z)/q(z)$ defines a unit vector $\mathbf n_R$. The [Skyrme model](../../../../../skyrme-model.md) field is approximated by

$$
U(r,z)=\exp[i f(r)\mathbf n_R(z)\mathbin\cdot\boldsymbol\tau],
\qquad f(0)=\pi,\quad f(\infty)=0.
$$

Its [baryon number](../../../../../baryon-number.md) is the degree $B$ of $R$. Angular integration reduces the energy to a radial variational problem,

$$
E=4\pi\int_0^\infty\left[
r^2f'^2+2B(1+f'^2)\sin^2f
+\mathcal I\frac{\sin^4f}{r^2}\right]dr
$$

up to the conventional overall normalization, where the angular functional $\mathcal I$ depends only on $R$. One first minimizes $\mathcal I$ among degree-$B$ maps and then minimizes over the profile $f$. This efficiently captures the topology, energy, and polyhedral symmetries of many Skyrmions.

Let $\omega=e^{2\pi i/5}$. Since $\omega^5=1$,

$$
R(\omega z)=\omega^2R(z),
$$

which is a fivefold spatial rotation accompanied by a target-space rotation. The real coefficients also give $R(\bar z)=\overline{R(z)}$, while direct substitution gives

$$
R(-1/z)=-\frac1{R(z)}.
$$

Together these transformations extend the cyclic symmetry to the stated $D_{5d}$ symmetry.

For $p=z^7-7z^2$ and $q=7z^5+1$, the [Wronskian](../../../../../wronskian.md) is

$$
\boxed{W=p'q-pq'=14z(z^{10}+11z^5-1)}.
$$

Besides $z=0$, put $y=z^5$. Then

$$
y^2+11y-1=0,
\qquad
y_\pm=\frac{-11\pm5\sqrt5}{2}.
$$

Thus five zeros lie on the circle

$$
|z|=\left(\frac{5\sqrt5-11}{2}\right)^{1/5}
$$

at arguments $2\pi k/5$, and five lie on the reciprocal circle at arguments $(2k+1)\pi/5$. The polynomial has degree eleven, so the twelfth zero lies at $z=\infty$. On the Riemann sphere, the zeros therefore form two opposite poles and two staggered pentagonal rings: the twelve vertices of an icosahedron.

The angular baryon-density factor is proportional to $|dR/dz|^2$ and vanishes at these critical directions. The Wronskian zeros therefore point toward twelve holes in the baryon-density surface. They are the face centers of the dodecahedral $B=7$ Skyrmion, equivalently the vertices of its dual icosahedron, and make its icosahedral symmetry visible directly in the rational map.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 308](../../paper-308-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
