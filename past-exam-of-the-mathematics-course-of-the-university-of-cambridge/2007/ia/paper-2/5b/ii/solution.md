<h1 id="5b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $z\ne0$, division by $4z$ gives $p(z)=1/(2z)$ and $q(z)=1/(4z)$. Thus zero is singular, but $zp=1/2$ and $z^2q=z/4$ are analytic. **Zero is a regular singular point.**

Apply the [Frobenius method](../../../../../../frobenius-method.md) with $y=z^r\sum_{n=0}^\infty a_nz^n$, $a_0\ne0$. The lowest power $z^{r-1}$ has coefficient $[4r(r-1)+2r]a_0$, so the [indicial equation](../../../../../../indicial-equation.md) is $2r(2r-1)=0$. Its [characteristic exponents at a regular singular point](../../../../../../characteristic-exponent-at-a-regular-singular-point.md) are $0$ and $1/2$. At the next powers,

$$
2(n+r)(2(n+r)-1)a_n+a_{n-1}=0,\qquad n\geq1.
$$

With $a_0=1$, the two [Frobenius solutions](../../../../../../frobenius-solution.md) are therefore

$$
y_1(z)=\sum_{n=0}^{\infty}\frac{(-1)^nz^n}{(2n)!},
\qquad
y_2(z)=z^{1/2}\sum_{n=0}^{\infty}\frac{(-1)^nz^n}{(2n+1)!}.
$$

Both analytic power-series factors converge everywhere by the [ratio test](../../../../../../ratio-test.md). Recognizing the trigonometric series gives

$$
\boxed{y(z)=A\cos\sqrt z+B\sin\sqrt z.}
$$

On a punctured neighbourhood choose a consistent square-root branch for the second solution; the first is entire in $z$. These solutions are independent, since their leading orders are $1$ and $z^{1/2}$. A direct [square-root reduction of a regular-singular differential equation](../../../../../../square-root-reduction-of-a-regular-singular-differential-equation.md) also verifies the closed forms: for $s=\sqrt z$ and $Y(s)=y(s^2)$, $4zy''=Y_{ss}-Y_s/s$ and $2y'=Y_s/s$, so the equation reduces to $Y_{ss}+Y=0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5B](../../5b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
