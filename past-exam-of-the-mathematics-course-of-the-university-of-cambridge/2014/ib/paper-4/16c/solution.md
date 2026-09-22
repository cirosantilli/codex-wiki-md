<h1 id="16c/solution">Solution</h1>

↑ **Parent:** [16C](../16c.md)

Along a sufficiently smooth stationary curve, differentiation and the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) give the [Beltrami identity](../../../../../beltrami-identity.md):

$$
 \frac d{dx}(f-y'f_{y'})=f_yy'-y'\frac d{dx}f_{y'}=0,
 \qquad\boxed{f-y'f_{y'}=\text{constant}.}
$$

The cancellation uses the absence of explicit $x$ dependence.

For an axisymmetric [surface of revolution](../../../../../surface-of-revolution.md), its area is $I[y]=2\pi\int_{-l}^l y\sqrt{1+y'^2}\,dx$. A smooth positive-radius minimizer is stationary, so the [Beltrami identity](../../../../../beltrami-identity.md), with the constant factor omitted, gives

$$
 \frac{y}{\sqrt{1+y'^2}}=k>0.
$$

Equivalently the [Euler-Lagrange equation](../../../../../euler-lagrange-equation.md) gives $yy''=1+y'^2$, whence $y''=y/k^2$. The first integral selects

$$
 y=k\cosh((x-x_*)/k).
$$

Equal radii at $\pm l$ imply $x_*=0$ (subtract the two cosh values), giving

$$
 \boxed{y(x)=k\cosh(x/k),\qquad r=k\cosh(l/k).}
$$

This is a [catenoid](../../../../../catenoid.md). The conclusion is a necessary form for a smooth connected minimizer; it does not declare every stationary catenoid a minimum.

Put $a=l/k>0$. The boundary equation is $r/l=\cosh a/a$. Its derivative is $(a\sinh a-\cosh a)/a^2$, so its unique critical point solves $a\tanh a=1$. The left side increases strictly from zero to infinity. Thus $\cosh a/a$ decreases to a unique minimum and then increases, diverging as $a\downarrow0$ and $a\to\infty$. There are exactly two positive values of $k$ when

$$
 r/l>\min_{a>0}\frac{\cosh a}{a}\simeq1.50888.
$$

At equality there is one value, and below it there is none.

To match the printed [second variation](../../../../../second-variation.md) convention, write $I[y+\varepsilon\eta]=I[y]+\varepsilon\delta I+\varepsilon^2\delta^2I+o(\varepsilon^2)$; its $\delta^2I$ is the quadratic coefficient, half the second derivative with respect to $\varepsilon$. Expanding the area integrand gives

$$
 \delta^2I=\pi\int_{-l}^l\left[\frac{y}{(1+y'^2)^{3/2}}\eta'^2
 +2\frac{y'}{\sqrt{1+y'^2}}\eta\eta'\right]dx.
$$

On the [catenoid](../../../../../catenoid.md) these coefficients are $k\operatorname{sech}^2(x/k)$ and $2\tanh(x/k)$. Integrate the mixed term by parts; the boundary term is zero because $\eta(\pm l)=0$. Since $(\tanh(x/k))'=\operatorname{sech}^2(x/k)/k$, this yields

$$
 \boxed{\delta^2I=\pi\int_{-l}^l\left(k\eta'^2-\frac{\eta^2}{k}\right)\operatorname{sech}^2(x/k)\,dx.}
$$

This is the [axisymmetric second variation of a catenoid](../../../../../axisymmetric-second-variation-of-a-catenoid.md), with the explicitly stated quadratic-coefficient convention.

## ↑ Ancestors (10)

1. [16C](../16c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
