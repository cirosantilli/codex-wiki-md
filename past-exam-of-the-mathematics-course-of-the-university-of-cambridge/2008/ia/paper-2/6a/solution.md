<h1 id="6a/solution">Solution</h1>

↑ **Parent:** [6A](../6a.md)

With the indicated order of the two solutions, define the [Wronskian](../../../../../wronskian.md) by

$$
\boxed{W=y_1y_2'-y_1'y_2
=\det\begin{pmatrix}y_1&y_2\\y_1'&y_2'\end{pmatrix}.}
$$

Where $y_1\ne0$, this gives the first-order [linear differential equation](../../../../../linear-differential-equation.md)

$$
y_2'-\frac{y_1'}{y_1}y_2=\frac{W}{y_1},\qquad
\left(\frac{y_2}{y_1}\right)'=\frac{W}{y_1^2}.
$$

Integrating produces the [reduction of order](../../../../../reduction-of-order.md) formula

$$
\boxed{y_2(x)=y_1(x)\left[C_2+\int_{x_0}^x\frac{W(s)}{y_1(s)^2}\,ds\right].}
$$

This formula is local on an interval where the known solution does not vanish; an arbitrary nonzero scaling of the [linearly independent](../../../../../linear-independence.md) solution changes the normalization of $W$.

Differentiate the [Wronskian](../../../../../wronskian.md) and use the differential equation for each solution:

$$
W'=y_1y_2''-y_1''y_2
=y_1(-py_2'-qy_2)-(-py_1'-qy_1)y_2=-pW.
$$

Thus $\boxed{W'+pW=0}$, proving the [Abel identity](../../../../../abel-s-identity.md), and $W=C\exp(-\int p\,dx)$. For continuous coefficients on a nonsingular interval, [linearly independent](../../../../../linear-independence.md) solutions have $C\ne0$.

For the particular equation, write $s=x-1$. The proposed solution is $y_1=s^2$, with $y_1'=2s$ and $y_1''=2$, so substitution gives $2s^2+2s^2-4s^2=0$. Away from the singular point $x=1$, division by $s^2$ gives $p=1/s$. The [Abel identity](../../../../../abel-s-identity.md) therefore gives

$$
W=\frac Cs
$$

with a separate constant on each interval lying on one side of the singular point. The [reduction of order](../../../../../reduction-of-order.md) integral is $\int W/y_1^2\,dx=C\int s^{-5}\,ds=-C/(4s^4)$, so

$$
y_2=C_2s^2-\frac C4s^{-2}.
$$

Choosing $C_2=0$, $C=-4$ gives

$$
\boxed{y_2(x)=(x-1)^{-2},\qquad W(x)=-\frac4{x-1}.}
$$

The nonzero [Wronskian](../../../../../wronskian.md) proves [linear independence](../../../../../linear-independence.md). Direct substitution also verifies the second solution, since $s^2(6s^{-4})+s(-2s^{-3})-4s^{-2}=0$. These solutions form a [basis](../../../../../basis.md) on either nonsingular interval; the second solution is not defined at $x=1$.

## ↑ Ancestors (10)

1. [6A](../6a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
