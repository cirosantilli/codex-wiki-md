<h1 id="15a/solution">Solution</h1>

↑ **Parent:** [15A](../15a.md)

Interpret the three conditions at zero as an initial-value problem on $x\ge0$, with interior source $\xi>0$. A [causal Green function](../../../../../causal-green-function.md) satisfies $\mathcal L_xG=\delta(x-\xi)$ and vanishes for $x<\xi$. Since the leading coefficient of the third derivative is one, the [jump conditions for a third-order Green function](../../../../../jump-conditions-for-a-third-order-green-function.md) require $G$ and $G'$ continuous and $G''$ to jump by one. For $t=x-\xi>0$, the homogeneous roots are $0,2,-1$. Solving $g(0)=g'(0)=0$, $g''(0)=1$ yields

$$
\boxed{G(x;\xi)=\Theta(x-\xi)\left(\frac{e^{2(x-\xi)}}6+\frac{e^{-(x-\xi)}}3-\frac12\right).}
$$

For $\xi>0$ it vanishes near zero, so all three initial boundary conditions hold. The matching conditions ensure that $\partial_x^3G$ supplies precisely a Dirac delta, without unwanted delta derivatives.

The homogeneous solution carrying the nonzero initial data is $y_h=\tfrac12-\tfrac16e^{2x}+\tfrac23e^{-x}$. The [Green-function representation](../../../../../green-function-representation.md) therefore gives

$$
y(x)=y_h(x)+\int_0^xG(x;\xi)e^\xi\Theta(\xi-1)\,d\xi.
$$

For $x<1$ the integral vanishes. For $x\ge1$, set $t=x-1$ and integrate to obtain $\tfrac e6(e^{2t}-3e^t-e^{-t}+3)$. Thus

$$
\boxed{y(x)=\frac12-\frac16e^{2x}+\frac23e^{-x}+\frac e6\Theta(x-1)\left(e^{2(x-1)}-3e^{x-1}-e^{-(x-1)}+3\right).}
$$

The bracket and its first two derivatives vanish at $x=1$, so $y,y',y''$ match continuously there; its third derivative jumps by the stated forcing. The value assigned to $\Theta(0)$ is immaterial. The source at the initial endpoint $\xi=0$ would need a separate endpoint-delta convention, which is not used in this integral.

## ↑ Ancestors (10)

1. [15A](../15a.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
