<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $S>0$ denote volume loss per unit downstream length and take $Q_0>0$. Mass balance gives $Q_x=-S$, so

$$
\boxed{Q(x)=Q_0-Sx.}
$$

Assume fluid is removed carrying its local axial [velocity](../../../../../../velocity.md), with no additional axial force on the retained flow. Under this inviscid seepage approximation, the horizontal momentum equation and its Bernoulli head are unchanged. On the flat bed, [hydraulic control with prescribed seepage](../../../../../../hydraulic-control-with-prescribed-seepage.md) therefore uses

$$
\boxed{E(h;x)=h+\frac{(Q_0-Sx)^2}{2gb_0^2[1+(x/L)^2]^2h^2}=\mathcal B.}
$$

The calculation applies on a reach with positive remaining discharge. Constant loss cannot be extended indefinitely past $x=Q_0/S$ while preserving this positive-flow model.

At a regular control, $F=1$ and the same differentiated energy condition requires $q_x=0$, where $q=(Q_0-Sx)/b(x)$. Differentiating gives

$$
q_x=\frac{Sx^2-2Q_0x-SL^2}{b_0L^2[1+(x/L)^2]^2}.
$$

Write $D=\sqrt{Q_0^2+S^2L^2}$. The two algebraic roots are $(Q_0\pm D)/S$. At the plus root $Q=-D<0$, so it is outside the stipulated positive-flow branch. The admissible control candidate is

$$
\boxed{x_c=\frac{Q_0-D}{S}=-\frac{SL^2}{Q_0+D}<0.}
$$

It lies upstream of the geometric throat. At this point $Q(x_c)=D$ and

$$
b(x_c)=\frac{2b_0D}{Q_0+D},\qquad q_c=\frac{Q_0+D}{2b_0}.
$$

It is a maximum of positive $q$: differentiating the numerator of $q_x$ at $x_c$ gives $2Sx_c-2Q_0=-2D<0$. Consequently

$$
\boxed{h_c=\left[\frac{(Q_0+D)^2}{4gb_0^2}\right]^{1/3}.}
$$

A control exists only if the reach includes this point and boundary conditions supply the critical conserved head $\mathcal B=3h_c/2$ and a suitable transcritical connection. Merely prescribing $Q_0$ and $S$ does not force that head. At $S=0$ the limiting location is zero and the usual throat depth is recovered.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 83](../../../paper-83-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
