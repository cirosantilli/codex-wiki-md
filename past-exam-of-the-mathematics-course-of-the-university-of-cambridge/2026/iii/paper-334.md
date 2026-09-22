# Paper 334

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20334.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20334.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [i](#1/a/i)
      - [Solution](#1/a/i/solution)
    - [ii](#1/a/ii)
      - [Solution](#1/a/ii/solution)
    - [iii](#1/a/iii)
      - [Solution](#1/a/iii/solution)
  - [b](#1/b)
    - [i](#1/b/i)
      - [Solution](#1/b/i/solution)
    - [ii](#1/b/ii)
      - [Solution](#1/b/ii/solution)
    - [iii](#1/b/iii)
      - [Solution](#1/b/iii/solution)
  - [c](#1/c)
    - [i](#1/c/i)
      - [Solution](#1/c/i/solution)
    - [ii](#1/c/ii)
      - [Solution](#1/c/ii/solution)
    - [iii](#1/c/iii)
      - [Solution](#1/c/iii/solution)
- [2](#2)
  - [a](#2/a)
    - [i](#2/a/i)
      - [Solution](#2/a/i/solution)
    - [ii](#2/a/ii)
      - [Solution](#2/a/ii/solution)
    - [iii](#2/a/iii)
      - [Solution](#2/a/iii/solution)
  - [b](#2/b)
    - [i](#2/b/i)
      - [Solution](#2/b/i/solution)
    - [ii](#2/b/ii)
      - [Solution](#2/b/ii/solution)
    - [iii](#2/b/iii)
      - [Solution](#2/b/iii/solution)

## 1

↑ **Parent:** [Paper 334](paper-334.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/i">i</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/i/solution">Solution</h5>

↑ **Parent:** [I](#1/a/i)

[Murray's law](../../../mathematical-biology.md#murray-s-law) minimizes the sum of the power needed to pump a [Newtonian fluid](../../../viscous-fluid-flow.md#newtonian-fluid) and the metabolic power needed to maintain blood volume. For a cylindrical vessel of radius $R$, length $\ell$, and prescribed volume flux $Q$, [Hagen-Poiseuille flow](../../../viscous-fluid-flow.md#hagen-poiseuille-equation) gives

$$
\mathcal P_{\rm pump}
=\Delta p\,Q
=\frac{8\mu\ell Q^2}{\pi R^4}.
$$

If maintenance costs $\alpha$ per unit volume,

$$
\mathcal P_{\rm met}=\alpha\pi R^2\ell.
$$

Setting the derivative of $\mathcal P_{\rm pump}+\mathcal P_{\rm met}$ with respect to $R$ to zero gives

$$
Q=\frac{\pi}{4}\sqrt{\frac{\alpha}{\mu}}\,R^3.
$$

Thus $Q\propto R^3$. Conservation of volume flux at a bifurcation gives

$$
\boxed{R_0^3=R_1^3+R_2^3}.
$$

<h4 id="1/a/ii">ii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/a/ii)

For [plane Poiseuille flow](../../../viscous-fluid-flow.md#plane-poiseuille-flow) between walls $y=\pm h$, let $G=-p_x>0$. Per unit out-of-plane depth,

$$
u(y)=\frac{G}{2\mu}(h^2-y^2),
\qquad
Q=\int_{-h}^h u\,dy
=\frac{2Gh^3}{3\mu}.
$$

For vessel length $\ell$,

$$
\mathcal P_{\rm pump}
=\Delta p\,Q
=\frac{3\mu\ell Q^2}{2h^3}.
$$

The maintained cross-sectional area per unit depth is $2h$, so

$$
\mathcal P_{\rm met}=2\alpha h\ell.
$$

Optimization gives

$$
-\frac{9\mu\ell Q^2}{2h^4}+2\alpha\ell=0,
\qquad
\boxed{Q=\frac23\sqrt{\frac{\alpha}{\mu}}\,h^2}.
$$

The two-dimensional Murray law is therefore

$$
\boxed{h_0^2=h_1^2+h_2^2}.
$$

<h4 id="1/a/iii">iii</h4>

↑ **Parent:** [A](#1/a)

<h5 id="1/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/a/iii)

The wall [shear stress](../../../viscous-fluid-flow.md#shear-stress) in the planar vessel is

$$
\tau_w=\mu|u_y(h)|=Gh
=\frac{3\mu Q}{2h^2}.
$$

The optimized relation $Q\propto h^2$ therefore makes

$$
\boxed{\tau_w=\text{constant}}
$$

throughout an ideal network. Murray's optimization can equivalently be interpreted as selecting a uniform wall shear stress. The familiar three-dimensional law $Q\propto R^3$ has the same interpretation because cylindrical Poiseuille flow has $\tau_w=4\mu Q/(\pi R^3)$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/i">i</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/i/solution">Solution</h5>

↑ **Parent:** [I](#1/b/i)

The [Fahraeus--Lindqvist effect](../../../mathematical-biology.md#fahraeus-lindqvist-effect) is the decrease of blood's apparent or effective viscosity as a microvessel narrows through much of the physiological small-vessel range. Deformable red blood cells migrate away from the wall and concentrate near the centre, creating a [cell-free layer](../../../mathematical-biology.md#cell-free-layer) of relatively low-viscosity plasma beside the vessel wall. Because the largest shear occurs near the wall, replacing cell-rich blood there by plasma reduces hydraulic resistance particularly effectively. At diameters comparable with a red blood cell, confinement eventually invalidates this decreasing trend.

<h4 id="1/b/ii">ii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/b/ii)

Let $b=h-\delta$ be the half-width of the cell-rich core. In fully developed pressure-driven flow the shear stress is fixed by momentum balance, independently of the local viscosity:

$$
\tau(y)=-Gy.
$$

With no slip at $y=h$,

$$
u(y)=\int_y^h\frac{Gs}{\mu(s)}\,ds.
$$

Interchanging the order of integration gives the total flux

$$
Q=2\int_0^h u(y)\,dy
=2G\int_0^h\frac{s^2}{\mu(s)}\,ds
=\frac{2G}{3}
\left[
\frac{b^3}{\mu}
+\frac{h^3-b^3}{\mu_w}
\right].
$$

By definition, the homogeneous effective fluid has

$$
Q=\frac{2Gh^3}{3\mu_{\rm eff}}.
$$

Writing $\varepsilon=\delta/h$ therefore gives

$$
\boxed{
\frac1{\mu_{\rm eff}}
=\frac{(1-\varepsilon)^3}{\mu}
+\frac{1-(1-\varepsilon)^3}{\mu_w}},
$$

or the reciprocal of the right-hand side.

<h4 id="1/b/iii">iii</h4>

↑ **Parent:** [B](#1/b)

<h5 id="1/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/b/iii)

If $\delta=0$, then $\varepsilon=0$, the cell-rich material fills the gap, and

$$
\boxed{\mu_{\rm eff}=\mu}.
$$

If $\delta=h$, then the core disappears and

$$
\boxed{\mu_{\rm eff}=\mu_w}.
$$

For the physical ordering $\mu_w<\mu$, increasing the [cell-free layer](../../../mathematical-biology.md#cell-free-layer) thickness monotonically lowers $\mu_{\rm eff}$ between these limits, exactly as intuition and the [Fahraeus--Lindqvist effect](../../../mathematical-biology.md#fahraeus-lindqvist-effect) suggest.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/i">i</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/i/solution">Solution</h5>

↑ **Parent:** [I](#1/c/i)

The [Zweifach--Fung effect](../../../mathematical-biology.md#zweifach-fung-effect), also called [plasma skimming](../../../mathematical-biology.md#zweifach-fung-effect), is the tendency at an unequal microvascular bifurcation for the high-flow daughter to receive a disproportionately large fraction of the red blood cells. The low-flow daughter consequently has a lower discharge haematocrit than the parent.

<h4 id="1/c/ii">ii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#1/c/ii)

Each daughter has the planar Poiseuille relation

$$
Q_i=\frac{2h^3}{3\mu}G_i,
\qquad
G_i=-\frac{dp_i}{dx}.
$$

Hence

$$
\boxed{
G_i=\frac{3\mu Q_i}{2h^3}
=O\left(\frac{\mu Q_i}{h^3}\right)}.
$$

The higher-flow daughter therefore requires the larger pressure-gradient magnitude:

$$
\boxed{Q_2>Q_1\quad\Longrightarrow\quad G_2>G_1.}
$$

<h4 id="1/c/iii">iii</h4>

↑ **Parent:** [C](#1/c)

<h5 id="1/c/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#1/c/iii)

Across a cell of radius $a$, a pressure gradient $G_i$ changes the viscous shear stress by order

$$
\boxed{
\sigma_i=O(aG_i)
=O\left(\frac{\mu aQ_i}{h^3}\right)}.
$$

In the two-dimensional model, the force per unit out-of-plane depth on one side is $O(\sigma_i a)$ and its lever arm is $O(a)$. The net moment per unit depth is therefore

$$
\boxed{
M=O\left[(\sigma_1-\sigma_2)a^2\right]
=O\left[
\frac{\mu a^3}{h^3}(Q_1-Q_2)
\right]}.
$$

A fully three-dimensional force estimate adds one power of $a$. Since $Q_2>Q_1$, the stronger stress on the high-flow side gives a definite rotation that tips a deformable cell off the ideal point-particle separatrix and into daughter 2. This local finite-size mechanism biases cells toward the higher-flow branch and is consistent with the [Zweifach--Fung effect](../../../mathematical-biology.md#zweifach-fung-effect).

## 2

↑ **Parent:** [Paper 334](paper-334.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/i">i</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/i/solution">Solution</h5>

↑ **Parent:** [I](#2/a/i)

For a unidirectional, $z$-independent velocity

$$
\mathbf u=u_z(r,\theta)\mathbf e_z,
$$

incompressibility holds automatically. The axial [Stokes flow](../../../stokes-flow.md) equation is

$$
0=-p_z+\mu\nabla_\perp^2u_z.
$$

No external pressure gradient is imposed, so $p_z=0$ and

$$
\boxed{\nabla_\perp^2u_z=0}.
$$

**Thus the axial velocity is a [harmonic function](../../../partial-differential-equation.md#harmonic-function) in the disk.**

<h4 id="2/a/ii">ii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/a/ii)

The boundary data are $U\operatorname{sgn}(\sin\theta)$, whose [Fourier series](../../../fourier-series.md) is

$$
\operatorname{sgn}(\sin\theta)
=\frac4\pi\sum_{\substack{n\geq1\\n\ {\rm odd}}}
\frac{\sin(n\theta)}n.
$$

Regular harmonic modes in a disk are $(r/R)^n\sin(n\theta)$ and $(r/R)^n\cos(n\theta)$. Matching the odd boundary data gives

$$
\boxed{
u_z(r,\theta)
=\frac{4U}{\pi}
\sum_{\substack{n\geq1\\n\ {\rm odd}}}
\frac1n\left(\frac rR\right)^n\sin(n\theta)}.
$$

Every term is regular at $r=0$, and the series approaches the prescribed values at every boundary point away from the two jump discontinuities.

<h4 id="2/a/iii">iii</h4>

↑ **Parent:** [A](#2/a)

<h5 id="2/a/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/a/iii)

For $|z|<1$,

$$
\sum_{\substack{n\geq1\\n\ {\rm odd}}}\frac{z^n}{n}
=\frac12\log\frac{1+z}{1-z}.
$$

Set $z=(r/R)e^{i\theta}$ and take the imaginary part. Since $r<R$, the real part of the relevant denominator is positive, and the result is

$$
\boxed{
u_z(r,\theta)
=\frac{2U}{\pi}
\arctan\left(
\frac{2Rr\sin\theta}{R^2-r^2}
\right)}.
$$

As $r\to R^-$ this tends to $U$ for $0<\theta<\pi$ and to $-U$ for $-\pi<\theta<0$.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/i">i</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/i/solution">Solution</h5>

↑ **Parent:** [I](#2/b/i)

The transverse and longitudinal [Péclet numbers](../../../fluid-mechanics.md#peclet-number) are

$$
\boxed{\operatorname{Pe}_h=\frac{Uh}{D}},
\qquad
\boxed{\operatorname{Pe}_L=\frac{UL}{D}
=\frac Lh\operatorname{Pe}_h}.
$$

The [Taylor dispersion](../../../fluid-mechanics.md#taylor-dispersion) regime requires transverse diffusion to act within a longitudinal advection time,

$$
\frac{h^2}{D}\ll\frac LU
\quad\Longleftrightarrow\quad
\operatorname{Pe}_h\ll\frac Lh,
$$

while longitudinal molecular diffusion is slow on that advection time,

$$
\operatorname{Pe}_L\gg1.
$$

Together,

$$
\boxed{
\frac hL\ll\operatorname{Pe}_h\ll\frac Lh},
\qquad
\boxed{
1\ll\operatorname{Pe}_L\ll\left(\frac Lh\right)^2}.
$$

<h4 id="2/b/ii">ii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/ii/solution">Solution</h5>

↑ **Parent:** [Ii](#2/b/ii)

The [advection-diffusion equation](../../../diffusion-equation.md#advection-diffusion-equation) is

$$
c_t+u(y)c_x=D(c_{xx}+c_{yy}),
\qquad
u(y)=\frac Uh y.
$$

Write

$$
c=\bar c(x,t)+c'(x,y,t),
\qquad
\overline{c'}=0,
$$

where the bar is the cross-gap average. In the long, late-time Taylor regime, $c'$ adjusts rapidly across the gap while $\bar c$ varies slowly along the cell. The leading fluctuation balance is

$$
\boxed{
u(y)\bar c_x=Dc'_{yy}}.
$$

Its scaling is

$$
\frac{U\bar c}{L}\sim\frac{Dc'}{h^2},
\qquad
\boxed{
\frac{c'}{\bar c}
\sim\frac{Uh^2}{DL}
=\operatorname{Pe}_h\frac hL\ll1}.
$$

This final inequality is precisely the transverse-equilibration condition from part i.

<h4 id="2/b/iii">iii</h4>

↑ **Parent:** [B](#2/b)

<h5 id="2/b/iii/solution">Solution</h5>

↑ **Parent:** [Iii](#2/b/iii)

Put $c'=\chi(y)\bar c_x$. The balance and reflecting boundary conditions give

$$
D\chi''=\frac Uh y,
\qquad
\chi'(\pm h)=0,
\qquad
\bar\chi=0.
$$

Integration yields

$$
\boxed{
\chi(y)=\frac UD
\left(\frac{y^3}{6h}-\frac{hy}{2}\right)}.
$$

Averaging the full transport equation gives

$$
\bar c_t+\overline{u\chi}\,\bar c_{xx}
=D\bar c_{xx}.
$$

Now

$$
\overline{u\chi}
=\frac{U^2}{D}
\left(\frac{\overline{y^4}}{6h^2}
-\frac{\overline{y^2}}2\right)
=-\frac{2U^2h^2}{15D},
$$

because $\overline{y^2}=h^2/3$ and $\overline{y^4}=h^4/5$. Thus the flow-induced [Taylor dispersion](../../../fluid-mechanics.md#taylor-dispersion) coefficient and total effective diffusivity are

$$
\boxed{
D_T=\frac{2U^2h^2}{15D}},
\qquad
\boxed{
D_{\rm eff}=D+\frac{2U^2h^2}{15D}}.
$$

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
