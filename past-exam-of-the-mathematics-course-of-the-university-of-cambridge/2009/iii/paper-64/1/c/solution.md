<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $ab\ne0$, a [magnetic field line](../../../../../../magnetic-field-line.md) stays at fixed $R$ and satisfies $d\phi/dz=B_\phi/(RB_z)=a/b$. It is therefore a helix with axial pitch $2\pi b/a$; the sign of $a/b$ fixes its handedness. The axial [magnetic flux](../../../../../../magnetic-flux.md) is $\pi bR_0^2$, and the [toroidal magnetic field](../../../../../../toroidal-magnetic-field.md) supplies the twist. If $a=0$ the field is untwisted; if $b=0$ it consists of azimuthal circles rather than helical lines carrying axial flux.

A convenient globally regular [magnetic vector potential](../../../../../../magnetic-vector-potential.md) has $A_R=0$ and

$$
\begin{aligned}
A_\phi&=\begin{cases}bR/2,&R<R_0,\\bR_0^2/(2R),&R>R_0,\end{cases}\\
A_z&=\begin{cases}C-aR^2/2,&R<R_0,\\C-aR_0^2/2,&R>R_0.\end{cases}
\end{aligned}
$$

Indeed, the cylindrical [curl](../../../../../../curl.md) gives $B_z=R^{-1}d(RA_\phi)/dR$ and $B_\phi=-dA_z/dR$, with $B_R=0$. The tangential potential components are continuous at $R_0$, so their derivatives introduce no unwanted delta-function [magnetic field](../../../../../../magnetic-field.md) at the tube boundary. The $C$ term is a constant axial potential.

The most general regular potential is this one plus $\nabla\Lambda(R,\phi,z)$ for an arbitrary single-valued gauge function. A putative extra $C_\phi/R$ term in the inner $A_\phi$ is excluded by regularity at the axis; the exterior $1/R$ circulation is already fixed by the enclosed [magnetic flux](../../../../../../magnetic-flux.md). Since the potential is globally defined across the axis and exterior, any remaining difference is a [curl-free vector field](../../../../../../irrotational-vector-field.md), hence a gradient. The constant $C$ can itself be absorbed into a gauge function proportional to $z$.

For the displayed gauge family, inside the tube

$$
\mathbf A\cdot\mathbf B=\frac{bR}{2}(aR)+b\left(C-\frac{aR^2}{2}\right)=bC,
$$

and hence

$$
\boxed{\frac{H_m}{L}=\int_0^{R_0}2\pi R\,bC\,dR=\pi bCR_0^2.}
$$

For example, requiring $A_z=0$ outside sets $C=aR_0^2/2$ and gives $\boxed{H_m/L=\pi abR_0^4/2}$. The equally regular choice $C=0$ gives zero. More generally, for a length-$L$ segment the [gauge transformation](../../../../../../gauge-transformation.md) contributes

$$
\Delta H_m= b\int_{R<R_0}[\Lambda(R,\phi,L)-\Lambda(R,\phi,0)]\,dS.
$$

In particular, $\Lambda=\Delta C\,z$ shifts $H_m/L$ by $\pi bR_0^2\Delta C$. This [gauge dependence of helicity in an open magnetic flux tube](../../../../../../gauge-dependence-of-helicity-in-an-open-magnetic-flux-tube.md) is possible because field lines penetrate the end caps when $b\ne0$. There is no contradiction with part (b), whose no-penetration condition fails at those caps. A gauge or end-cap convention is needed to give a unique value per unit length. For $b=0$ the ordinary helicity is zero and this end-cap ambiguity disappears.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 64](../../../paper-64-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
