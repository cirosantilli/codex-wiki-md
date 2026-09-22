<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Expand the [radial modified Helmholtz equation](../../../../radial-modified-helmholtz-equation.md) as $Ly=-y''-2y'/x+y$. Setting $y=z/x$ gives $Ly=(-z''+z)/x$, so

$$
y(x)=\frac{Ae^x+Be^{-x}}x.
$$

Boundedness at zero requires $A+B=0$, whereas boundedness at infinity requires $A=0$. The respective adapted [homogeneous solutions](../../../../homogeneous-solution.md) are therefore

$$
\boxed{u(x)=\frac{\sinh x}{x}\quad\text{at zero},\qquad v(x)=\frac{e^{-x}}x\quad\text{at infinity}.}
$$

The first has limit one at zero. Their [Wronskian](../../../../wronskian.md) is $uv'-u'v=-x^{-2}$. Since the highest-derivative coefficient of $L$ is $-1$, the [Green function](../../../../green-s-function-split.md) must have first-derivative jump $-1$. The [radial modified Helmholtz Green function on the half-line](../../../../radial-modified-helmholtz-green-function-on-the-half-line.md) is

$$
\boxed{G(x,\xi)=\frac\xi x\sinh(\min(x,\xi))e^{-\max(x,\xi)},\qquad x,\xi>0.}
$$

It is continuous at the source, and its [derivative](../../../../derivative.md) jump is $-1$, giving $L_xG=\delta(x-\xi)$. For fixed source it tends to $\xi e^{-\xi}$ as $x\downarrow0$ and decays at infinity. This kernel is for the original operator and ordinary measure $d\xi$; multiplying the equation by $x^2$ would change the source normalization.

For the compact source, split the [integral](../../../../integral-split.md) at $\xi=x$ when $x<R$. The needed antiderivatives are

$$
\int\xi\sinh\xi\,d\xi=\xi\cosh\xi-\sinh\xi,\qquad\int\xi e^{-\xi}d\xi=-(\xi+1)e^{-\xi}.
$$

Thus

$$
y(x)=\frac{e^{-x}}x\int_0^x\xi\sinh\xi\,d\xi+\frac{\sinh x}{x}\int_x^R\xi e^{-\xi}d\xi\quad(x<R),
$$

while for $x>R$ the result is $e^{-x}x^{-1}\int_0^R\xi\sinh\xi\,d\xi$. Simplifying gives

$$
\boxed{y(x)=\begin{cases}\displaystyle1-(R+1)e^{-R}\frac{\sinh x}{x},&0\leq x\leq R,\\\displaystyle(R\cosh R-\sinh R)\frac{e^{-x}}x,&x\geq R.\end{cases}}
$$

The continuous value at zero is $1-(R+1)e^{-R}$, and $y'(0)=0$. Both $y$ and $y'$ match at $R$, so no extra [Dirac delta](../../../../dirac-delta-function.md) appears there. The only [homogeneous solution](../../../../homogeneous-solution.md) bounded at both ends is zero, establishing uniqueness.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [Paper 1](../../paper-1-split.md)
3. [2010](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
