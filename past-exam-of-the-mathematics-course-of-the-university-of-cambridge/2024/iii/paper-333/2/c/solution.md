<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $D(x,y)=H(x,y)-h(x,y)$ and let $\mathbf u=(u,v)$ be the depth-independent interior velocity. The kinematic boundary conditions on the sloping upper and lower surfaces are

$$
w_t=w_E-\mathbf u\mathbin\cdot\nabla h,
\qquad
w_b=-\mathbf u\mathbin\cdot\nabla H.
$$

Integrating [mass conservation](../../../../../../mass-conservation.md) through the layer gives

$$
\frac{DD}{Dt}+D\nabla_h\mathbin\cdot\mathbf u=-w_E.
$$

The inviscid vertical-vorticity equation is

$$
\frac D{Dt}(f+\zeta)
=-(f+\zeta)\nabla_h\mathbin\cdot\mathbf u,
\qquad
\zeta=v_x-u_y.
$$

Consequently the [shallow-water potential vorticity](../../../../../../shallow-water-potential-vorticity.md)

$$
q=\frac{f+\zeta}{D}
$$

obeys the forced evolution equation

$$
\boxed{
\frac{Dq}{Dt}=\frac{q}{D}w_E}.
$$

Positive upward [Ekman pumping](../../../../../../ekman-pumping.md) removes layer thickness and raises the potential vorticity of the remaining column.

For a steady small-[Rossby number](../../../../../../rossby-number.md) flow, $q\simeq f/D$, so

$$
\mathbf u\mathbin\cdot\nabla\left(\frac fD\right)
=\frac{f}{D^2}w_E.
$$

Equivalently,

$$
\boxed{
\beta Dv-f\mathbf u\mathbin\cdot\nabla D
=fw_E}.
$$

The same result follows from the integrated vortex-stretching balance

$$
\beta Dv=f(w_t-w_b).
$$

When $\nabla D=(c,0)$ with $c>0$,

$$
\beta Dv-fcu=fw_E.
$$

If the upper pumping is absent or weak and the upper surface is locally level, the impermeable-bottom condition is $w_b=-cu$. The stipulated $w_b<0$ then gives $u>0$, and in the Northern Hemisphere

$$
v\simeq\frac{fc}{\beta D}u>0.
$$

The steady interior flow is therefore directed northeastward, along contours of $f/D$ in the unforced limit. As a parcel moves eastward into deeper water, its vortex column stretches; a poleward displacement increases $f$ and preserves [potential vorticity](../../../../../../potential-vorticity.md). Nonzero [Ekman pumping](../../../../../../ekman-pumping.md) drives motion across the $f/D$ contours. This is [topographic potential-vorticity steering](../../../../../../topographic-potential-vorticity-steering.md) and the associated [topographic Sverdrup balance](../../../../../../topographic-sverdrup-balance.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 333](../../../paper-333-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
