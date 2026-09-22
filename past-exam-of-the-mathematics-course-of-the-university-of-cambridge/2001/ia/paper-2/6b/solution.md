<h1 id="6b/solution">Solution</h1>

↑ **Parent:** [6B](../6b.md)

Where $y_1$ is nonzero, the [Wronskian](../../../../../wronskian.md) identity $W=y_1y_2'-y_1'y_2$ becomes the first-order equation

$$
y_2'-\frac{y_1'}{y_1}y_2=\frac W{y_1}.
$$

Its [integrating factor](../../../../../integrating-factor.md) is $1/y_1$, giving $(y_2/y_1)'=W/y_1^2$. Integration proves the [reduction of order](../../../../../reduction-of-order.md) formula

$$
\boxed{y_2(x)=y_1(x)\left[C_0+\int_{x_0}^x\frac{W(t)}{y_1(t)^2}\,dt\right].}
$$

Taking $C_0=0$ gives the displayed representative in the question, with $y_2(x_0)=0$ when $y_1(x_0)\ne0$. Changing the lower limit adds a multiple of $y_1$ and does not change the [linearly independent](../../../../../linear-independence.md) solution modulo the known one. The scale of $W$ separately fixes the normalization of $y_2$.

Differentiate the [determinant](../../../../../determinant.md) and use the original second-order equation for each solution:

$$
W'=y_1y_2''-y_1''y_2
=y_1(-py_2'-qy_2)-(-py_1'-qy_1)y_2=-pW.
$$

This proves [Abel's identity](../../../../../abel-s-identity.md) **$W'+pW=0$** rather than merely quoting it.

For the specific equation, substituting $y_1=1-x$, $y_1'=-1$, $y_1''=0$ leaves $(1-x^2)-(1+x)(1-x)=0$. Away from zero its normalized first-derivative coefficient is $p(x)=x-1/x$, so

$$
W(x)=Cx e^{-x^2/2}.
$$

Although the equation is singular at zero, this expression extends analytically there. Near zero, $y_1$ is nonzero and the [reduction of order](../../../../../reduction-of-order.md) integrand is regular. With the prescribed lower limit,

$$
y_2(x)=C(1-x)\int_0^x\frac{t e^{-t^2/2}}{(1-t)^2}\,dt.
$$

The integrand through degree three is

$$
\frac{t e^{-t^2/2}}{(1-t)^2}
=t\bigl(1-t^2/2+O(t^4)\bigr)\bigl(1+2t+3t^2+O(t^3)\bigr)
=t+2t^2+\frac52t^3+O(t^4).
$$

After integrating and multiplying by $1-x$,

$$
y_2(x)=C\left(\frac{x^2}{2}+\frac{x^3}{6}-\frac{x^4}{24}+O(x^5)\right).
$$

The condition $y_2''(0)=1$ fixes $C=1$, and the lower limit already gives $y_2(0)=0$. Therefore the first three nonzero terms are

$$
\boxed{y_2(x)=\frac{x^2}{2}+\frac{x^3}{6}-\frac{x^4}{24}+O(x^5).}
$$

The representation genuinely solves the second-order equation: writing $L[y]=y''+py'+qy$, differentiating its [Wronskian](../../../../../wronskian.md) gives $W'+pW=y_1L[y_2]-y_2L[y_1]=y_1L[y_2]$. Its left-hand side is zero and $y_1\ne0$ near zero. Analyticity then extends the original unnormalized equation to zero itself. Its [Wronskian](../../../../../wronskian.md) with $y_1$ is nonzero for sufficiently small $x\ne0$, proving [linear independence](../../../../../linear-independence.md). The vanishing [Wronskian](../../../../../wronskian.md) at the singular point zero does not contradict [linear independence](../../../../../linear-independence.md) on a regular interval. The integral representation is used locally near zero, before the zero of $y_1$ at one.

## ↑ Ancestors (10)

1. [6B](../6b.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
