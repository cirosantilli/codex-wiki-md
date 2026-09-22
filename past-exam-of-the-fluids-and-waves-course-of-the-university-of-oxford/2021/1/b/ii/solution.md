<h1 id="1/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $F_x,F_y$ denote the [force per unit length](../../../../../force-per-unit-length.md) exerted by the fluid on the [cylinder](../../../../../cylinder-geometry.md), and let $\rho$ be the constant [mass density](../../../../../density.md). For a counterclockwise contour $C$ around the unit [circle](../../../../../circle.md), the [Blasius force theorem](../../../../../blasius-force-theorem.md) gives

$$
F_x-iF_y=\frac{i\rho}{2}\oint_C q(z)^2\,dz,
\qquad
q(z)=U-\frac U{z^2}+\frac1{z-b}+\frac1{z-a}-\frac1z,
\quad a=\frac1b.
$$

An efficient use of the [residue theorem](../../../../../residue-theorem.md) finds the sum of the enclosed [residues](../../../../../residue.md) by subtracting the external [pole](../../../../../pole.md) at $b$ from the sum of all finite [residues](../../../../../residue.md). At large $z$,

$$
q(z)=U+\frac1z+O(z^{-2}),\qquad
q(z)^2=U^2+\frac{2U}{z}+O(z^{-2}).
$$

The sum of all finite [residues](../../../../../residue.md) of $q^2$ is therefore $2U$. At $b$, write $q=(z-b)^{-1}+H(z)$, with $H$ a [holomorphic function](../../../../../holomorphic-function-split.md) near $b$. Then

$$
\operatorname{Res}_{z=b}q^2=2H(b),\qquad
H(b)=U-\frac U{b^2}+\frac1{b-a}-\frac1b.
$$

Thus

$$
\oint_Cq^2\,dz=2\pi i\,[2U-2H(b)],
\qquad
F_x-iF_y=2\pi\rho[H(b)-U].
$$

Using $a=1/b$ and $1/(b-a)-1/b=1/[b(b^2-1)]$ gives

$$
\boxed{F_x=2\pi\rho\left(\frac1{b(b^2-1)}-\frac U{b^2}\right),
\qquad F_y=0}.
$$

The vanishing vertical [force](../../../../../force-split.md) also follows from [reflection symmetry](../../../../../reflection-symmetry.md) about the real axis. This [force on a unit cylinder due to a uniform flow and an external source](../../../../../force-on-a-unit-cylinder-due-to-a-uniform-flow-and-an-external-source.md) uses the counterclockwise orientation in the [Blasius force theorem](../../../../../blasius-force-theorem.md) to fix the sign of the horizontal [force](../../../../../force-split.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the fluids and waves course of the University of Oxford](../../../../split.md)
6. [Fluids and waves course of the University of Oxford](../../../../../fluids-and-waves-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
