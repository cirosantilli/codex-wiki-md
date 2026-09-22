# Paper 354

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_354.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2021/paper_354.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)

## 1

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

Four distinct points in a conformal field theory with $d>2$ possess two independent [conformal cross-ratios](../../../string-theory.md#conformal-cross-ratio), conventionally

$$
u=\frac{x_{12}^2x_{34}^2}{x_{13}^2x_{24}^2},
\qquad
v=\frac{x_{14}^2x_{23}^2}{x_{13}^2x_{24}^2}.
$$

Translations, rotations, dilations, and [special conformal transformations](../../../general-relativity.md#special-conformal-transformation) can map three points to canonical positions $0$, a point on one chosen axis, and the point at infinity in a [conformal completion](../../../general-relativity.md#conformal-completion). The fourth point retains one radial coordinate and one angle relative to that axis. Those two quantities are equivalent to $u$ and $v$; the stabilizer rotations remove all its remaining angular coordinates.

For identical [scalar primary operators](../../../string-theory.md#scalar-primary-operator) of dimension $\Delta$, conformal covariance fixes a kinematic prefactor and leaves an arbitrary function $\mathcal G(u,v)$:

$$
F(x_1,x_2,x_3,x_4)
=\frac{\mathcal G(u,v)}{(x_{12}^2x_{34}^2)^\Delta}
$$

for one common convention. Since a generic conformal field theory has unrestricted dynamical dependence on both cross-ratios, no lower-dimensional set determines the function. Therefore

$$
\boxed{\dim\mathcal S=2}.
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

For a scalar operator of dimension $\Delta=2$ in a boundary theory of dimension $d=3$, the [AdS scalar mass--dimension relation](../../../string-theory.md#ads-scalar-mass-dimension-relation) gives

$$
m^2=\Delta(\Delta-d)=-2
$$

in unit-radius $\operatorname{AdS}_4$. In Poincare coordinates,

$$
ds^2=\frac1{z^2}(\eta_{\mu\nu}dx^\mu dx^\nu+dz^2),
$$

so the free [Klein-Gordon equation](../../../wave-equation.md#klein-gordon-equation) is

$$
\boxed{\left[z^2(\partial_z^2+\Box_{2+1})
-2z\partial_z+2\right]\phi=0}.
$$

This mass is exactly that of a [conformally coupled scalar field](../../../quantum-field-theory.md#conformally-coupled-scalar-field) in four-dimensional anti-de Sitter spacetime. The [Weyl transformation](../../../string-theory.md#weyl-transformation)

$$
\boxed{\phi(x,z)=z\,\psi(x,z)}
$$

therefore maps the equation to the flat half-space wave equation

$$
\boxed{(\partial_z^2+\Box_{2+1})\psi=0,
\qquad z>0}.
$$

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

The [AdS scalar-field boundary asymptotics](../../../string-theory.md#ads-scalar-field-boundary-asymptotics) are

$$
\phi(x,z)=z^{3-\Delta}J(x)+z^\Delta A(x)+\cdots
=zJ(x)+z^2A(x)+\cdots.
$$

Thus the [holographic dictionary](../../../string-theory.md#holographic-dictionary) becomes especially simple for the flat field $\psi=\phi/z$:

$$
\boxed{J(x)=\lim_{z\to0}\frac{\phi(x,z)}z
=\psi(x,0)},
$$



$$
\boxed{\langle\mathcal O(x)\rangle
=(2\Delta-d)A(x)=A(x)
=\lim_{z\to0}\partial_z\left(\frac{\phi(x,z)}z\right)}
$$

up to the overall normalization chosen for the bulk action and possible local counterterms. The leading mode is the source and the normalizable subleading mode is the response.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

The flat four-dimensional [retarded Green function](../../../quantum-field-theory.md#retarded-green-function) is

$$
G_{\rm ret}^{(4)}(t,\mathbf X)
=\frac{\theta(t)}{2\pi}
\delta(t^2-|\mathbf X|^2).
$$

For a [Dirichlet boundary condition](../../../differential-equation.md#dirichlet-boundary-condition) at $z=0$, the [method of images](../../../mathematics.md#method-of-images) gives

$$
G_D(X;X')=G_{\rm ret}^{(4)}(x-x',z-z')
-G_{\rm ret}^{(4)}(x-x',z+z').
$$

The boundary-to-bulk kernel for $\psi$ is its inward boundary derivative. For a source at the spacetime origin,

$$
G_\psi(x,z|0)
=\left.\partial_{z'}G_D(x,z;0,z')\right|_{z'=0}
=\frac{2z}{\pi}\theta(t)
\delta'\left(t^2-x^2-y^2-z^2\right).
$$

Multiplying by the Weyl factor $z$ gives the requested kernel for the original bulk field:

$$
\boxed{G(x,z|0)
=\frac{2z^2}{\pi}\theta(t)
\delta'\left(t^2-x^2-y^2-z^2\right)}.
$$

It is causal and supported on the future bulk light cone of the boundary insertion. Its distributional boundary limit satisfies $\phi/z\to\delta^3(x)$, while the source-free initial term vanishes for the CFT vacuum in this response calculation.

## 2

↑ **Parent:** [Paper 354](paper-354.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

On the $t=0$ slice, rotational symmetry lets the surface be written $z=z(r)$. The inversion symmetry fixing the boundary circle extends to an isometry of the Poincare half-space whose fixed set is

$$
r^2+z^2=R^2.
$$

The unique extremal surface anchored at $r=R,z=0$ must be invariant under that isometry. Hence the [Ryu–Takayanagi surface for a disk](../../../string-theory.md#ryu-takayanagi-surface-for-a-disk) is the hemisphere

$$
\boxed{\gamma_D:\quad z(r)=\sqrt{R^2-r^2},
\qquad 0\leq r\leq R}.
$$

One may verify directly that it extremizes the area functional $2\pi\int r z^{-2}\sqrt{1+z'^2}\,dr$.

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

Regulate the surface at $z=\epsilon$, so $r_{\max}=\sqrt{R^2-\epsilon^2}$. On the hemisphere, $\sqrt{1+z'^2}=R/z$, and its area is

$$
\begin{aligned}
\operatorname{Area}(\gamma_D)
&=2\pi R\int_0^{r_{\max}}
\frac{r\,dr}{(R^2-r^2)^{3/2}}\\
&=2\pi\left(\frac R\epsilon-1\right).
\end{aligned}
$$

The [Ryu–Takayanagi formula](../../../string-theory.md#ryu-takayanagi-formula) therefore gives

$$
\boxed{S_D=\frac{\pi}{2G}
\left(\frac R\epsilon-1\right)}.
$$

The first term is the ultraviolet area-law divergence proportional to the boundary circle's length; the finite constant is universal for the vacuum of a three-dimensional conformal field theory.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

Translation invariance in $y$ lets the surface be written $z=z(x)$. Per unit $y$ length, its area and entropy functionals are

$$
\boxed{\frac AL=\int_{-R}^{R}
\frac{\sqrt{1+z'(x)^2}}{z(x)^2}\,dx,
\qquad
\frac SL=\frac1{4G}\frac AL}.
$$

The boundary conditions are $z(\pm R)=0$, understood with an ultraviolet cutoff, and reflection symmetry gives $z'(0)=0$ at $z(0)=z_{\max}$.

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The Lagrangian $\mathcal L=z^{-2}\sqrt{1+z'^2}$ has no explicit $x$ dependence, so its [Beltrami identity](../../../analysis.md#beltrami-identity) is conserved:

$$
\mathcal L-z'\frac{\partial\mathcal L}{\partial z'}
=\frac1{z^2\sqrt{1+z'^2}}
=\text{constant}.
$$

At the turning point $z=z_{\max}$ and $z'=0$, the constant is $z_{\max}^{-2}$. Rearrangement gives

$$
1+z'^2=\frac{z_{\max}^4}{z^4},
\qquad
\boxed{\frac{dz}{dx}
=\pm\sqrt{\frac{z_{\max}^4}{z^4}-1}}.
$$

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

For the disk, the hemisphere reaches

$$
z_{\max,D}=R.
$$

For half of the strip surface, invert the first-order equation and integrate from the midpoint to the boundary:

$$
R=\int_0^{z_{\max,T}}
\frac{z^2\,dz}{\sqrt{z_{\max,T}^4-z^4}}
=z_{\max,T}\int_0^1
\frac{u^2\,du}{\sqrt{1-u^4}}.
$$

The [beta function](../../../complex-analysis.md#beta-function) integral is

$$
\int_0^1\frac{u^2\,du}{\sqrt{1-u^4}}
=\frac{\sqrt\pi\,\Gamma(3/4)}{\Gamma(1/4)}
\simeq0.59907.
$$

Therefore

$$
\boxed{z_{\max,T}
=\frac{\Gamma(1/4)}{\sqrt\pi\,\Gamma(3/4)}R
\simeq1.669R>R=z_{\max,D}}.
$$

The strip's holographic entropy surface lies deeper in the bulk than that of a disk with the same half-width or radius.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2021](../../2021.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
