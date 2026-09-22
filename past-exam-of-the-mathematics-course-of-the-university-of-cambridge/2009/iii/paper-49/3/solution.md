<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $w=u+iv$ and $R=1+u^2+v^2$. Inverting the specified [stereographic projection](../../../../../stereographic-projection.md) gives

$$
\phi=\frac1R(2u,2v,1-u^2-v^2).
$$

The coordinate takes the value infinity at the south pole, so a general map is described using the extended complex plane and a second chart there. A pole of $w$ is not necessarily a singularity of $\phi$.

Differentiate the inverse formulas:

$$
d\phi_1=\frac{2du}{R}-\frac{2u\,dR}{R^2},\quad
d\phi_2=\frac{2dv}{R}-\frac{2v\,dR}{R^2},\quad
d\phi_3=-\frac{2dR}{R^2},\qquad dR=2u\,du+2v\,dv.
$$

On squaring and summing, the terms containing $(dR)^2$ cancel, leaving $|d\phi|^2=4(du^2+dv^2)/R^2$. Thus the [stereographic energy of the O3 sigma model](../../../../../stereographic-energy-of-the-o3-sigma-model.md) is

$$
\boxed{\widetilde V(w)=4\int_{\mathbb R^2}\frac{|\partial_1w|^2+|\partial_2w|^2}{(1+|w|^2)^2}\,d^2x.}
$$

The same derivatives give $\phi\cdot(\partial_u\phi\times\partial_v\phi)=4/R^2$, with positive sign: at $u=v=0$ the ordered tangent vectors are $(2,0,0)$ and $(0,2,0)$ at the north pole. The chain rule therefore gives

$$
\boxed{N=\frac1\pi\int_{\mathbb R^2}\frac{u_{x_1}v_{x_2}-u_{x_2}v_{x_1}}{(1+|w|^2)^2}\,d^2x
=\frac1\pi\int_{\mathbb R^2}\frac{\operatorname{Im}(\overline{w_{x_1}}w_{x_2})}{(1+|w|^2)^2}\,d^2x.}
$$

This is the [topological degree](../../../../../topological-degree.md) for the orientation in the question.

Put $z=x_1+ix_2$, $w_z=(w_{x_1}-iw_{x_2})/2$ and $w_{\bar z}=(w_{x_1}+iw_{x_2})/2$. Expanding the squares gives

$$
\widetilde V=8\int\frac{|w_z|^2+|w_{\bar z}|^2}{(1+|w|^2)^2}\,d^2x,\qquad
N=\frac1\pi\int\frac{|w_z|^2-|w_{\bar z}|^2}{(1+|w|^2)^2}\,d^2x.
$$

For $N\geq0$, subtracting the second expression times $8\pi$ gives

$$
\widetilde V-8\pi N=16\int\frac{|w_{\bar z}|^2}{(1+|w|^2)^2}\,d^2x\geq0;
$$

for $N\leq0$, adding $8\pi N$ gives the analogous square with $w_z$. Consequently

$$
\boxed{\widetilde V\geq8\pi|N|.}
$$

The factor is $8\pi$, not $4\pi$, because the printed energy has no prefactor $1/2$. Equality requires a [holomorphic map](../../../../../holomorphic-map.md) for positive degree, an [antiholomorphic map](../../../../../antiholomorphic-function.md) for negative degree, or a constant map for zero energy.

Explicit examples for every integer degree are

$$
\boxed{w(z)=z^N\ (N>0),\qquad w(z)=\overline z^{\,|N|}\ (N<0),\qquad w(z)=0\ (N=0).}
$$

To verify both degree and finite energy for $w=z^m$, $m>0$, use polar coordinates: $|w_z|^2=m^2r^{2m-2}$ and $w_{\bar z}=0$. Then

$$
N=2m^2\int_0^\infty\frac{r^{2m-1}}{(1+r^{2m})^2}\,dr
=m\int_0^\infty\frac{ds}{(1+s)^2}=m,
$$

where $s=r^{2m}$. Its energy is $8\pi m$. Complex conjugation changes the degree's sign while preserving the energy, and the constant example has degree and energy zero. These [sigma-model lumps](../../../../../sigma-model-lump.md) are smooth sphere-valued maps; the coordinate infinity at spatial infinity is regular in the other target chart.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
