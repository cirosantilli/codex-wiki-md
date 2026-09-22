<h1 id="12e/solution">Solution</h1>

↑ **Parent:** [12E](../12e.md)

Choose a branch of $t=1-z$ with $|\arg t|<\pi$ and write $d=c-a-b\notin\mathbb Z$. The [Gauss hypergeometric equation](../../../../../gauss-hypergeometric-equation.md) is

$$
z(1-z)y''+[c-(a+b+1)z]y'-aby=0.
$$

Changing to $t$ turns this into the same equation with third parameter $a+b+1-c=1-d$. Its solution regular at $t=0$ is $y_1=F(a,b,1-d;t)$. Substitution of $y=t^dv$ gives the [Gauss hypergeometric equation](../../../../../gauss-hypergeometric-equation.md) for $v$ with parameters $c-a,c-b,1+d$. Thus $y_2=t^dF(c-a,c-b,1+d;t)$ is also a solution. Their distinct nonintegrally separated [characteristic exponents at a regular singular point](../../../../../characteristic-exponent-at-a-regular-singular-point.md) $0,d$ imply [linear independence](../../../../../linear-independence.md) near $z=1$, so

$$
F(a,b,c;z)=Ay_1(z)+By_2(z).
$$

This also follows from the exponent transformation in the [Papperitz symbol](../../../../../papperitz-symbol.md).

Initially assume $\Re c>\Re b>0$, so the [Euler integral for the hypergeometric function](../../../../../euler-integral-for-the-hypergeometric-function.md) applies. If $\Re d>0$, taking $z\to1$ gives an integral evaluated by the [beta function](../../../../../beta-function.md) and determines

$$
A=\frac{\Gamma(c)\Gamma(d)}{\Gamma(c-a)\Gamma(c-b)}.
$$

Indeed $y_1\to1$ and $y_2\to0$ there. To find $B$, instead work in the nonempty parameter region $\Re d<0$, put $z=1-\epsilon$ and scale the integration variable by $1-s=\epsilon u$. The singular contribution is

$$
\frac{\Gamma(c)}{\Gamma(b)\Gamma(c-b)}\epsilon^d
\int_0^\infty u^{c-b-1}(1+u)^{-a}\,du.
$$

The defining integral of the [beta function](../../../../../beta-function.md) evaluates this [integral](../../../../../integral.md) to $\Gamma(c-b)\Gamma(-d)/\Gamma(a)$. Since $\epsilon^{-d}y_1\to0$ and $\epsilon^{-d}y_2\to1$, it determines $B$. [Analytic continuation](../../../../../analytic-continuation.md) in the parameters then yields the [hypergeometric connection formula](../../../../../hypergeometric-connection-formula-at-one.md)

$$
\boxed{A=\frac{\Gamma(c)\Gamma(c-a-b)}{\Gamma(c-a)\Gamma(c-b)},\qquad
B=\frac{\Gamma(c)\Gamma(a+b-c)}{\Gamma(a)\Gamma(b)}.}
$$

The usual power-series definition requires $c\notin\{0,-1,-2,\ldots\}$; exceptional parameters need a separately specified analytic [limit](../../../../../limit-of-a-function.md). Reciprocal [gamma functions](../../../../../gamma-function.md) make vanishing coefficients at denominator poles meaningful. The branch must remain fixed when continuing in $z$.

## ↑ Ancestors (10)

1. [12E](../12e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
