<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

The origin is a [regular singular point](../../../../../regular-singular-point.md) of this [Kummer differential equation](../../../../../kummer-differential-equation.md). Apply the [Frobenius method](../../../../../frobenius-method.md), writing $y=\sum_{n=0}^\infty a_nx^{n+r}$ with $a_0\ne0$. The lowest power gives the [indicial equation](../../../../../indicial-equation.md)

$$
r(r+c-1)=0,\qquad r=0,\ 1-c.
$$

For $n\geq1$, comparison of the coefficient of $x^{n+r-1}$ gives

$$
(n+r)(n+r+c-1)a_n-(n+r)a_{n-1}=0,\qquad
a_n=\frac{a_{n-1}}{n+r+c-1}.
$$

Since $0<c<1$, both roots give valid independent branches. Normalize $a_0=1$:

$$
\boxed{y_1(x)=\sum_{n=0}^\infty\frac{\Gamma(c)}{\Gamma(c+n)}x^n
=\sum_{n=0}^\infty\frac{x^n}{(c)_n},\qquad
y_2(x)=x^{1-c}\sum_{n=0}^\infty\frac{x^n}{n!}=x^{1-c}e^x.}
$$

Here $(c)_n$ is the [rising factorial](../../../../../rising-factorial.md), and the first series is the [confluent hypergeometric function of the first kind](../../../../../confluent-hypergeometric-function-of-the-first-kind.md) $M(1,c,x)$. The two leading powers are distinct, proving [linear independence](../../../../../linear-independence.md). We describe real solutions on $x>0$, with their one-sided behavior at zero.

For the inhomogeneous equation a particular solution is $-(x+c)/2$, verified by direct substitution. Thus $y=Ay_1+By_2-(x+c)/2$. Since $y_2'\sim(1-c)x^{-c}$, a finite derivative at zero forces $B=0$. Then $y(0)=0$ forces $A=c/2$, and the required solution is

$$
\boxed{y(x)=\frac c2\left[M(1,c,x)-1-\frac xc\right]
=\frac c2\sum_{n=2}^\infty\frac{x^n}{(c)_n}.}
$$

In particular $y'(0)=0$. The singular homogeneous branch cannot be added without violating the derivative condition.

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
