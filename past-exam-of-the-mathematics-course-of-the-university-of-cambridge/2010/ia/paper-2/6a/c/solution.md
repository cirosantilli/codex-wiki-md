<h1 id="6a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Multiply the equation by $x$ to obtain $xy''-P(x)y'-Q(x)y=0$. The leading terms after a [Frobenius method](../../../../../../frobenius-method.md) trial $y=x^r$ are

$$
\bigl(r(r-1)-P_0r\bigr)x^{r-1};
$$

the term involving $Q_0$ first appears at order $x^r$. The [indicial equation](../../../../../../indicial-equation.md) is therefore

$$
r(r-1-P_0)=0,\qquad \boxed{r=0,\ P_0+1.}
$$

To obtain the [first correction to a regular singular solution by reduction of order](../../../../../../first-correction-to-a-regular-singular-solution-by-reduction-of-order.md), start from the assumed solution $y_1=1+\beta x+O(x^2)$ and use the [Abel identity](../../../../../../abel-s-identity.md):

$$
W=C\exp\left(\int\frac{P(x)}x\,dx\right)
=Cx^{P_0}\bigl(1+P_1x+O(x^2)\bigr).
$$

We work initially on $x>0$ near zero; since $P_0$ is a positive integer, the resulting expansion is an ordinary [power series](../../../../../../power-series.md). Also $y_1^{-2}=1-2\beta x+O(x^2)$, so the [reduction of order](../../../../../../reduction-of-order.md) integral has integrand

$$
\frac{W}{y_1^2}=Cx^{P_0}\bigl(1+(P_1-2\beta)x+O(x^2)\bigr).
$$

Choose its integration constant to be zero, eliminating an added multiple of $y_1$. Integrating and multiplying by $y_1$ gives

$$
y_2=C\left[\frac{x^{P_0+1}}{P_0+1}
+\left(\frac{\beta}{P_0+1}+\frac{P_1-2\beta}{P_0+2}\right)x^{P_0+2}
+O(x^{P_0+3})\right].
$$

With $C=P_0+1$ the requested normalized answer is

$$
\boxed{y_2=x^{P_0+1}
+\frac{(P_0+1)P_1-P_0\beta}{P_0+2}x^{P_0+2}
+O(x^{P_0+3}).}
$$

Its nonzero [Wronskian](../../../../../../wronskian.md) makes it independent of $y_1$. The existence of the asserted $y_1$ also forces $P_0\beta+Q_0=0$; there is no need to introduce $Q_0$ into the normalized second coefficient.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6A](../../6a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
