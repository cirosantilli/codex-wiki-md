<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Multiply the equation by $x^2$. Its left side is an exact derivative, yielding the [first integral](../../../../../first-integral.md)

$$
\epsilon x^2y'+(x^2-2\epsilon^3)y=C.
$$

For a solution continuous at the singular endpoint, the limiting value is $C=-2\epsilon^3\gamma$. This can also be established from the exact integrating-factor formula below, without assuming uniform bounds on derivatives near zero.

Away from zero, the [outer expansion](../../../../../outer-expansion.md) has leading term $y\sim C/x^2$. The endpoint value at one requires $C\sim\epsilon^3$ if an exponentially amplified homogeneous term is to be avoided. It follows already that

$$
\boxed{\gamma\sim-\frac12.}
$$

To exhibit the matching and explain the required boundedness, first set $x=\epsilon X$, $y=\epsilon Y(X)$ for a representative without an order-one homogeneous contribution. The leading [inner expansion](../../../../../inner-expansion.md) obeys

$$
Y''+\left(1+\frac2X\right)Y'+\frac{2Y}X=0,\qquad X^2(Y'+Y)=1.
$$

Integration gives

$$
Y=-\frac1X+e^{-X}\left[\operatorname{Ei}(X)+B\right],
$$

where $\operatorname{Ei}$ is the [exponential integral](../../../../../exponential-integral.md). For $X\to\infty$, $Y\sim X^{-2}$, matching the outer term $\epsilon^3/x^2$. For $X\to0$, $Y\sim-1/X$, so the intermediate solution behaves as $-\epsilon^2/x$ and reaches order one on a second scale $x=\epsilon^2\xi$.

On this second scale, the [first integral](../../../../../first-integral.md) becomes, at leading order, $\xi^2Y_0'-2Y_0=1$. Equivalently its differentiated equation is $Y_0''+(2/\xi-2/\xi^2)Y_0'=0$, as in the hint. The matching solution that tends to zero as $\xi\to\infty$ is

$$
\boxed{Y_0(\xi)=\frac12\left(e^{-2/\xi}-1\right).}
$$

It has $Y_0\sim-1/\xi$ at large $\xi$, matching the intermediate region, and $Y_0(0)=-1/2$. Thus the [nested layers at an essential singular endpoint](../../../../../nested-layers-at-an-essential-singular-endpoint.md) connect an order-$\epsilon^3$ outer solution to an order-one endpoint value without an unbounded overshoot.

The issue of uniqueness is clarified by exact integration. Put

$$
\mu(x)=e^{x/\epsilon+2\epsilon^2/x},\qquad h(x)=\mu(x)^{-1}.
$$

For every fixed $\epsilon>0$ and every prescribed exact value of $\gamma$, the solution satisfying the right endpoint is

$$
y(x)=h(x)\left[\epsilon^3\mu(1)+2\epsilon^2\gamma\int_x^1\frac{\mu(s)}{s^2}\,ds\right].
$$

As $x\to0$, the integral is asymptotic to $\mu(x)/(2\epsilon^2)$, proving $y(0)=\gamma$. Since $h(1)>0$, the two exact endpoint values fix the two constants: **for a prescribed exact $\gamma$, this finite-$\epsilon$ boundary-value problem is unique**.

However, specifying only the leading value $\gamma\sim-1/2$ and uniform order-one size does not select a unique asymptotic family. To see this constructively, choose $x_m=\sqrt2\,\epsilon^{3/2}$ and an arbitrary bounded real constant $A$. Write

$$
y(x)=h(x)\left[A+\frac C\epsilon\int_{x_m}^x\frac{\mu(s)}{s^2}\,ds\right],\qquad
I=\int_{x_m}^1\frac{\mu(s)}{s^2}\,ds.
$$

The right endpoint fixes

$$
C=\frac{\epsilon[\epsilon^3\mu(1)-A]}{I},\qquad\gamma=-\frac{C}{2\epsilon^3}.
$$

Endpoint [Laplace's method](../../../../../laplace-s-method.md) gives $I=\epsilon\mu(1)[1+2\epsilon+O(\epsilon^2)]$. Therefore every bounded choice of $A$ has

$$
\gamma=-\frac12+\epsilon+O(\epsilon^2),
$$

with changes in $A$ affecting $\gamma$ only by $O(\epsilon^{-3}e^{-1/\epsilon})$. These solutions are uniformly order one: near zero their particular part has the finite limit $\gamma$, near one it follows the small outer solution, and the freely chosen value at $x_m$ is $Ah(x_m)=O(1)$. The inner-layer homogeneous contribution is also bounded. Indeed $h$ vanishes at zero, is order one near $x_m$, and is exponentially small at one.

Consequently **the order-one selected value is $-1/2$, but algebraic asymptotic endpoint data leave an order-one interior freedom**. This is [beyond-all-orders boundary-value sensitivity](../../../../../beyond-all-orders-boundary-value-sensitivity.md). If “constant” were interpreted as fixing $\gamma=-1/2$ exactly and independently of $\epsilon$, the omitted algebraic corrections would excite an exponentially large interior homogeneous term; a genuinely uniformly bounded exact family requires the higher-order tuning of $\gamma$. Constancy in $x$ does not preclude that parameter dependence.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 79](../../paper-79-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
