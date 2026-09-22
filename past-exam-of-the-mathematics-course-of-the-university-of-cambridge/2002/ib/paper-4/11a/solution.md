<h1 id="11a/solution">Solution</h1>

↑ **Parent:** [11A](../11a.md)

Take an admissible variation $y+\varepsilon\eta$ with $\eta=\eta'=0$ at both regular endpoints. Its [first variation](../../../../../first-variation.md) is $\delta I=\int(f_y\eta+f_{y'}\eta'+f_{y''}\eta'')\,dx$. Integrating the second term once and the third twice gives the boundary term $[f_{y'}\eta+f_{y''}\eta'-(d f_{y''}/dx)\eta]_a^b$, which vanishes. The [fundamental lemma of the calculus of variations](../../../../../fundamental-lemma-of-the-calculus-of-variations.md) therefore yields the [higher-order Euler-Lagrange equation](../../../../../higher-order-euler-lagrange-equation.md)

$$
\boxed{f_y-\frac d{dx}f_{y'}+\frac{d^2}{dx^2}f_{y''}=0.}
$$

Here $f_y=8yy'$, $f_{y'}=4y^2$, and $f_{y''}=2x^4y''$. The first two contributions cancel, leaving $(x^4y'')''=0$. For $x>0$, integrate twice to obtain $x^4y''=Ax+B$, and then

$$
y(x)=\frac A{2x}+\frac B{6x^2}+Cx+D.
$$

The two singular-endpoint limits give $B=0$ and $A=2$. The conditions at one give $C=1$ and $D=0$. Hence the unique solution of the stated differential equation and limiting data is

$$
\boxed{y(x)=x+\frac1x\qquad(0<x\le1).}
$$

There is a genuine distinction between solving this equation and stationarity of a finite improper action. Substitution gives $f=4x^2+4-4x^{-4}$, whose [integral](../../../../../integral.md) at zero diverges to $-\infty$. The displayed Euler-Lagrange equation remains valid for compactly supported variations on $(0,1)$, or on regular cut-off intervals, but the literal unregularized action is not a finite stationary functional on this solution. These [singular endpoints in higher-order variational problems](../../../../../singular-endpoints-in-higher-order-variational-problems.md) require a regularization or an admissible-space convention if a global variational claim is intended.

## ↑ Ancestors (10)

1. [11A](../11a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
