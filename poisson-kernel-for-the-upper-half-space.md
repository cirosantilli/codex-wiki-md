# Poisson kernel for the upper half-space

↑ **Parent:** [Poisson kernel](poisson-kernel.md)

In three dimensions the [Poisson kernel for the upper half-space](poisson-kernel-for-the-upper-half-space.md) is

$$
P_z(u,v)=\frac{z}{2\pi(u^2+v^2+z^2)^{3/2}},\qquad z>0.
$$

It gives the [harmonic function](harmonic-function.md) $\phi(x,y,z)=\int_{\mathbb R^2}P_z(x-\xi,y-\eta)f(\xi,\eta)\,d\xi\,d\eta$ for compatible boundary data. The [method of images](method-of-images.md) constructs the zero-boundary [Dirichlet Green function](dirichlet-green-function.md) by subtracting the reflected-source [Green function of the Laplacian](green-function-of-the-laplacian.md) from the source kernel. On the boundary plane the outward [unit normal](unit-normal.md) is $-e_z$, and $-\partial_nG=P_z$, giving the integral formula through [Green's second identity](green-second-identity.md).

The kernel is positive and has integral one: in [polar coordinates](polar-coordinates.md) this is $z\int_0^\infty r(r^2+z^2)^{-3/2}dr=1$. Its mass outside any fixed disk tends to zero as $z\downarrow0$. It is therefore an [approximate identity](approximate-identity.md), recovering bounded boundary data at continuity points. At a jump across a smooth curve, the vertical limit gives the average of the two adjacent values; assigning a different value only on that curve does not change the harmonic extension.

**Table of contents**

- [Axial Poisson extension of a circular boundary patch](axial-poisson-extension-of-a-circular-boundary-patch.md)
- [Poisson kernel for the upper half-plane](poisson-kernel-for-the-upper-half-plane.md)
- [Poisson integral](poisson-integral.md)
  - [Poisson extension of interval boundary data](poisson-extension-of-interval-boundary-data.md)
  - [Dirichlet Poisson integral in a quadrant](dirichlet-poisson-integral-in-a-quadrant.md)
    - [Bounded Dirichlet uniqueness in a quadrant](bounded-dirichlet-uniqueness-in-a-quadrant.md)
    - [Zero-boundary harmonic growth in a quadrant](zero-boundary-harmonic-growth-in-a-quadrant.md)
    - [Holomorphic derivative of a quadrant Dirichlet solution](holomorphic-derivative-of-a-quadrant-dirichlet-solution.md)
  - [Schwarz integral formula](schwarz-integral-formula.md)
    - [Schwarz integral on the unit disk](schwarz-integral-on-the-unit-disk.md)
    - [Harmonic quadrant solution from tangential boundary derivatives](harmonic-quadrant-solution-from-tangential-boundary-derivatives.md)

## ↑ Ancestors (7)

1. [Poisson kernel](poisson-kernel.md)
2. [Poisson's equation](poisson-s-equation.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (12)

- [Axial Poisson extension of a circular boundary patch](axial-poisson-extension-of-a-circular-boundary-patch.md)
- [Neumann point source on a half-space boundary](neumann-point-source-on-a-half-space-boundary.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-7/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2003/paper-2/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2006/paper-2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2014/paper-2/3/ii/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/3/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2015/paper-2/3/e/solution.md)
- [Poisson kernel](poisson-kernel.md)
- [Poisson kernel for the upper half-space](poisson-kernel-for-the-upper-half-space.md)
- [Poisson representation of harmonic h1 by finite measures](poisson-representation-of-harmonic-h1-by-finite-measures.md)
- [Radial decreasing kernel domination by the maximal function](radial-decreasing-kernel-domination-by-the-maximal-function.md)
