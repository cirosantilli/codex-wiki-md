# Stereographic projection

↑ **Parent:** [Riemann sphere](riemann-sphere.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Stereographic_projection)

Stereographic projection identifies a sphere minus one pole with the plane and supplies the standard charts of the Riemann sphere.

In the equatorial-plane convention of the [Riemann sphere](riemann-sphere.md), draw the straight line through $N=(0,0,1)$ and a point $P=(X,Y,Z)\ne N$ on the [unit sphere](unit-sphere.md). Its intersection with the plane $Z=0$ has [complex coordinate](complex-coordinate.md)

$$
z=\sigma_N(P)=\frac{X+iY}{1-Z}.
$$

The [inverse function](inverse-function.md), for $z=x+iy$ and $r^2=x^2+y^2$, is

$$
P(z)=\left(\frac{2x}{1+r^2},\frac{2y}{1+r^2},\frac{r^2-1}{1+r^2}\right).
$$

Here positive $x$ gives positive $X$, and positive $y$ gives positive $Y$. Thus $1$ and $i$ lie on the positive $X$ and $Y$ ends of the equator. The omitted north pole is assigned $z=\infty$.[Complex Variables with Applications, MIT 18.04, Spring 2018; Topic 2 Notes, section 2.5.2, printed p. 7, projection formula and north pole](complex-variables-with-applications-mit-18-04-spring-2018/topic-2-notes.md)

<a id="image-north-pole-projection-onto-the-equatorial-plane-two-real-points-and-the-positive-complex-axis-convention"></a>
![](stereographic-projection-rays-and-axes.png)

**[Figure 3](#image-north-pole-projection-onto-the-equatorial-plane-two-real-points-and-the-positive-complex-axis-convention). North-pole projection onto the equatorial plane: two real points and the positive complex-axis convention**.

For original worked points, the real numbers $1/2$ and $2$ lift to points with the same $X$ coordinate but opposite $Z$ coordinates:

$$
P(1/2)=(4/5,0,-3/5),\qquad P(2)=(4/5,0,3/5).
$$

Projecting back gives $(4/5)/(1+3/5)=1/2$ and $(4/5)/(1-3/5)=2$. A point off the real axis checks the other sign:

$$
P(2+i)=(2/3,1/3,2/3),\qquad \sigma_N(2/3,1/3,2/3)=2+i.
$$

The coordinates satisfy $4/9+1/9+4/9=1$, as a point on the [unit sphere](unit-sphere.md) must. Also $P(0)=S$, $P(-1)=(-1,0,0)$ and $P(i)=(0,1,0)$.

A short derivation starts with the line $N+t(P-N)=(tX,tY,1+t(Z-1))$. Setting its last coordinate to zero gives $t=1/(1-Z)$, hence the projection formula. Conversely the line from $N$ to $(x,y,0)$ is $(tx,ty,1-t)$. Substitution in the [unit sphere](unit-sphere.md) equation gives

$$
t^2r^2+(1-t)^2=1,\qquad t\bigl(t(1+r^2)-2\bigr)=0.
$$

The root $t=0$ is $N$; the other root $t=2/(1+r^2)$ gives $P(z)$. These line intersections establish both the formula and its [bijection](bijection.md) property without guessing the inverse.

The same algebra explains how large planar distances become small spherical ones:

$$
1-Z=\frac{2}{1+|z|^2},\qquad \|P(z)-N\|=\frac{2}{\sqrt{1+|z|^2}}.
$$

Consequently $|z|\to\infty$ brings $P(z)$ to $N$ independently of direction. The last expression is twice the [chordal metric](chordal-metric.md) distance $\chi(z,\infty)$. A whole unbounded exterior in the [complex plane](complex-plane.md) therefore becomes a small cap on the [unit sphere](unit-sphere.md).

**Table of contents**

- [Circle-plane relation under stereographic projection](circle-plane-relation-under-stereographic-projection.md)
  - [Antipodal equatorial intersection criterion for a great circle](antipodal-equatorial-intersection-criterion-for-a-great-circle.md)
- [Antipodal stereographic coordinate relation](antipodal-stereographic-coordinate-relation.md)
  - [Antipodal cross-ratio and spherical distance](antipodal-cross-ratio-and-spherical-distance.md)
- [Holomorphic stereographic atlas of the sphere](holomorphic-stereographic-atlas-of-the-sphere.md)
  - [Reciprocal chart at infinity](reciprocal-chart-at-infinity.md)
- [Sphere rotations as special-unitary Möbius transformations](sphere-rotations-as-special-unitary-mobius-transformations.md)

## ↑ Ancestors (7)

1. [Riemann sphere](riemann-sphere.md)
2. [Riemann surfaces](riemann-surfaces-split.md)
3. [Complex analysis](complex-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (37)

- [Antipodal cross-ratio and spherical distance](antipodal-cross-ratio-and-spherical-distance.md)
- [Antipodal fixed-point classification of Möbius transformations](antipodal-fixed-point-classification-of-mobius-transformations.md)
- [Antipodal fixed points do not characterize sphere rotations](antipodal-fixed-points-do-not-characterize-sphere-rotations.md)
- [Antipodal stereographic coordinate relation](antipodal-stereographic-coordinate-relation.md)
- [Bogomolny degree bound for the O3 sigma model](bogomolny-degree-bound-for-the-o3-sigma-model.md)
- [Circle-plane relation under stereographic projection](circle-plane-relation-under-stereographic-projection.md)
- [Knot](knot.md)
- [O3 nonlinear sigma model](o3-nonlinear-sigma-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/13b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-9/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ib/paper-3/12a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/ib/paper-3/12h/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-9/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/ii/paper-1/23f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-56/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-2/12g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-1/3f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-49/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-59/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-50/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-15/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-10/4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-56/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-115/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-308/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-3/5g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-309/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-308/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-313/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/ii/paper-1/24g/i/solution.md)
- [Riemann sphere](riemann-sphere.md)
- [Sigma-model lump](sigma-model-lump.md)
- [Sphere rotations as special-unitary Möbius transformations](sphere-rotations-as-special-unitary-mobius-transformations.md)
- [Stationary wave map](stationary-wave-map.md)
- [Stereographic energy of the O3 sigma model](stereographic-energy-of-the-o3-sigma-model.md)
- [Two-chart smooth atlas of an ellipsoid](two-chart-smooth-atlas-of-an-ellipsoid.md)
- [Two stereographic charts on the circle](two-stereographic-charts-on-the-circle.md)
