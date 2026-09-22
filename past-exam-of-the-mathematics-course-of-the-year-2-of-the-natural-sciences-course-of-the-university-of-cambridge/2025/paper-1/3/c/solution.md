<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $n\ne0$, split the [Green's function](../../../../../green-s-function-split.md) integral at $s=x$. Writing $\ell(x)=x^{-n}-2^n$ and $r(x)=x^{-n}-1$ gives

$$
u(x)=\frac{r(x)\int_{1/2}^{x}(1-2^ns^n)\,ds+\ell(x)\int_x^1(1-s^n)\,ds}{n(2^n-1)}.
$$

For $n\ne-1$, the two [integrals](../../../../../integral-split.md) are

$$
I_1=x-\frac12-\frac{2^n}{n+1}\left(x^{n+1}-2^{-n-1}\right),\qquad I_2=1-x-\frac{1-x^{n+1}}{n+1}.
$$

Substitution and simplification yield

$$
\boxed{u(x)=\frac1{n+1}\left[x-1+\frac{x^{-n}-1}{2(2^n-1)}\right],\qquad n\ne0,-1.}
$$

At $x=1$ both contributions vanish. At $x=1/2$ the bracket is $-1/2+(2^n-1)/[2(2^n-1)]=0$. The [differential operator](../../../../../differential-operator.md) kills $x^{-n}-1$ and sends $x/(n+1)$ to $1/x$, so this also verifies the inhomogeneous equation.

The exceptional integer is $\boxed{n=-1}$, because then the [integrals](../../../../../integral-split.md) contain $s^{-1}$. In this case

$$
I_1=x-\frac12-\frac12\log(2x),\qquad I_2=1-x+\log x,
$$

and the [Green's function](../../../../../green-s-function-split.md) integral becomes

$$
\begin{aligned}
u(x)&=2\left[(x-1)\left(x-\frac12-\frac12\log(2x)\right)+\left(x-\frac12\right)(1-x+\log x)\right]\\
&=\boxed{x\log x+(1-x)\log2}.
\end{aligned}
$$

Here $L=d^2/dx^2$, and $u''=1/x$. Explicitly $u(1)=0$ and $u(1/2)=-(\log2)/2+(\log2)/2=0$. Thus both exceptional and nonexceptional formulas satisfy the required [boundary conditions](../../../../../boundary-condition.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
