<h1 id="7a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Here the [indicial equation](../../../../../../indicial-equation.md) has the repeated root $0$. The first [Frobenius method](../../../../../../frobenius-method.md) solution is $y_1=e^{-x}$. Since $p=1+1/x$, the [Abel identity](../../../../../../abel-s-identity.md) gives $W=Ce^{-x}/x$. [Reduction of order](../../../../../../reduction-of-order.md) with $C=1$ produces

$$
y_2=e^{-x}\int\frac{e^x}{x}\,dx=e^{-x}\left(\log x+\sum_{j=1}^{\infty}\frac{x^j}{j\,j!}\right),\qquad x>0,
$$

where the additive constant is absorbed into $y_1$. In particular the logarithmic coefficient is nonzero: an additional independent [real analytic](../../../../../../real-analytic-function.md) solution does not exist.

**The general local form is**

$$
\boxed{y(x)=C_1A(x)+C_2\bigl(A(x)\log x+B(x)\bigr),\quad A(x)=e^{-x},\quad B\text{ analytic at }0.}
$$

This is the repeated-root [Logarithmic Frobenius solution](../../../../../../logarithmic-solution-from-a-repeated-frobenius-exponent.md). On the negative real side one may use $\log|x|$, or use a fixed logarithm branch for a complex solution.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [7A](../../7a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
