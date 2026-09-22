<h1 id="12a/solution">Solution</h1>

↑ **Parent:** [12A](../12a.md)

The substitution is nonsingular in the interior $x>0$, $0<y<1$, $0<z<x$. Its inverse is

$$
x=\sqrt{\alpha\beta},\qquad
y=\sqrt{\frac\beta\alpha},\qquad
z=\gamma\sqrt{\frac\alpha\beta}.
$$

Thus $y<1$ is equivalent to $\beta<\alpha$, while $z<x$ is equivalent to $\gamma<xy=\beta$. Positivity gives the full transformed domain

$$
\boxed{0<\gamma<\beta<\alpha<\infty.}
$$

The forward [Jacobian determinant](../../../../../jacobian-determinant.md) is

$$
\frac{\partial(\alpha,\beta,\gamma)}{\partial(x,y,z)}
=\det\begin{pmatrix}
1/y&-x/y^2&0\\
y&x&0\\
0&z&y
\end{pmatrix}
=2x>0.
$$

Therefore $x\,dx\,dy\,dz=\tfrac12\,d\alpha\,d\beta\,d\gamma$. The [boundary](../../../../../boundary-of-a-set.md) faces where the formula fails have measure zero. The [change of variables formula](../../../../../change-of-variables-formula.md) gives

$$
I=\frac12\int_0^\infty d\alpha\int_0^\alpha d\beta\int_0^\beta d\gamma\,
e^{-A\alpha-B\beta-C\gamma}.
$$

The integrand is nonnegative, so [Tonelli's theorem](../../../../../tonelli-theorem.md) permits reordering the [integration](../../../../../integral.md) even before convergence has been established. Integrating first in $\alpha$, then in $\beta$, gives

$$
\begin{aligned}
I
&=\frac12\int_0^\infty e^{-C\gamma}\,d\gamma
\int_\gamma^\infty e^{-B\beta}\,d\beta
\int_\beta^\infty e^{-A\alpha}\,d\alpha\\
&=\frac1{2A}\int_0^\infty e^{-C\gamma}\,d\gamma
\int_\gamma^\infty e^{-(A+B)\beta}\,d\beta\\
&=\frac1{2A(A+B)}
\int_0^\infty e^{-(A+B+C)\gamma}\,d\gamma\\
&=\boxed{\frac1{2A(A+B)(A+B+C)}}.
\end{aligned}
$$

The assumptions $A,B,C>0$ make all three integrals of [exponential functions](../../../../../exponential-function.md) converge. Equivalently, the [ordered-cone substitution by products and ratios](../../../../../ordered-cone-substitution-by-products-and-ratios.md) can be followed by the increment variables $\alpha-\beta$, $\beta-\gamma$, $\gamma$, all independently positive and with [Jacobian determinant](../../../../../jacobian-determinant.md) one; the exponent then separates into three linear terms with coefficients $A$, $A+B$ and $A+B+C$.

## ↑ Ancestors (10)

1. [12A](../12a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
