<h1 id="33c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For one bound state at $-\kappa^2$ and no reflection, write

$$
F(s,t)=C(t)e^{-\kappa s},
\qquad
C(t)=C_0e^{8\kappa^3t}.
$$

The [rank-one Gelfand-Levitan-Marchenko kernel](../../../../../../rank-one-gelfand-levitan-marchenko-kernel.md) has the form $K(x,y;t)=-A(x,t)e^{-\kappa y}$. Substitution into the integral equation gives

$$
A=C(t)e^{-\kappa x}
-A\,C(t)\frac{e^{-2\kappa x}}{2\kappa},
$$

and hence

$$
K(x,x;t)
=-\frac{C(t)e^{-2\kappa x}}
{1+\dfrac{C(t)}{2\kappa}e^{-2\kappa x}}.
$$

Choose $x_0$ by $C_0/(2\kappa)=e^{2\kappa x_0}$. Then

$$
\frac{C(t)}{2\kappa}e^{-2\kappa x}
=e^{-2\kappa(x-x_0-4\kappa^2t)}.
$$

Differentiating the reconstruction formula gives the one-soliton solution

$$
\boxed{
u(x,t)
=-2\kappa^2
\operatorname{sech}^2\!\left[
\kappa(x-x_0-4\kappa^2t)
\right]
}.
$$

It is a negative [soliton](../../../../../../soliton.md) of amplitude $2\kappa^2$ travelling to the right with speed $4\kappa^2$, as required by this sign convention for KdV.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [33C](../../33c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
