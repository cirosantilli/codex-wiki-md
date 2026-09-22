<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For fixed $x>0$, set $y=y_0+\varepsilon y_1+\varepsilon^2y_2+\cdots$ and impose the data at one at each order. The leading equation gives $y_0'=0$, hence $y_0=1$. At the next two orders,

$$
x^2y_1'=1,\qquad x^2y_2'=2-\frac3x.
$$

The [boundary conditions](../../../../../../boundary-condition.md) $y_1(1)=y_2(1)=0$ give the three-term [outer expansion](../../../../../../outer-expansion.md)

$$
\boxed{y_{\rm out}=1+\varepsilon\left(1-\frac1x\right)
+\varepsilon^2\left(\frac12-\frac2x+\frac{3}{2x^2}\right)+\cdots}.
$$

Its ordering fails when $\varepsilon/x=O(1)$, locating a [boundary layer](../../../../../../boundary-layer.md) of thickness $O(\varepsilon)$ at zero. Put $x=\varepsilon\xi$ and $y=Y_0(\xi)+\varepsilon Y_1(\xi)+\cdots$. The rescaled equation is

$$
(1+\varepsilon)\xi^2y_\xi=y^3+
\varepsilon[\xi(y^2-1)+2y^2]-\varepsilon^2\xi(y^2+1).
$$

Its leading equation is $\xi^2Y_0'=Y_0^3$. Matching to the positive outer value one fixes the sign and integration constant:

$$
Y_0=\left(\frac\xi{\xi+2}\right)^{1/2}.
$$

At the next order the bracket $\xi(Y_0^2-1)+2Y_0^2$ vanishes identically, leaving

$$
\xi^2Y_1'-\frac{3\xi}{\xi+2}Y_1
=-\left(\frac\xi{\xi+2}\right)^{3/2}.
$$

The general solution is $Y_1=(1+k\xi)\xi^{1/2}/(\xi+2)^{3/2}$. In the overlap its expansion is

$$
Y_0=1-\frac1\xi+\frac{3}{2\xi^2}+\cdots,\qquad
Y_1=k+\frac{1-3k}{\xi}+\cdots.
$$

The outer solution re-expressed on this scale has the corresponding terms $1-1/\xi+3/(2\xi^2)+\varepsilon(1-2/\xi)+\cdots$. Thus [matched asymptotic expansion](../../../../../../matched-asymptotic-expansion.md) determines $k=1$, consistently in both displayed orders, and the two-term [inner expansion](../../../../../../inner-expansion.md) is

$$
\boxed{y_{\rm in}(\xi)=\left(\frac\xi{\xi+2}\right)^{1/2}
+\varepsilon\frac{(1+\xi)\xi^{1/2}}{(\xi+2)^{3/2}}+\cdots}.
$$

This positive branch tends continuously to zero at $x=0$, with a square-root cusp. An infinite endpoint [derivative](../../../../../../derivative.md) is compatible with the degeneracy of the original equation's $x^2y'$ coefficient.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
