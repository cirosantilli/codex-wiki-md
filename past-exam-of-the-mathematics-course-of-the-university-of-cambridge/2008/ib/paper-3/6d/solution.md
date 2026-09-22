<h1 id="6d/solution">Solution</h1>

↑ **Parent:** [6D](../6d.md)

Assume real $k\ne0$, and put $a=|k|$. Away from the source point the [Green function](../../../../../green-s-function.md) solves $G''-a^2G=0$. The two decay conditions select $G=Ae^{a(x-\xi)}$ on $x<\xi$ and $G=Be^{-a(x-\xi)}$ on $x>\xi$. Continuity at $\xi$ requires $A=B$: a jump in $G$ would create a derivative of the [Dirac delta](../../../../../dirac-delta-function.md) that is absent from the equation. Integrating the equation across the source gives $G'(\xi+)-G'(\xi-)=1$, so $-2aA=1$. Thus the negative of the [one-dimensional modified Helmholtz Green function](../../../../../one-dimensional-modified-helmholtz-green-function.md) is

$$
\boxed{G(x;\xi)=-\frac{e^{-|k||x-\xi|}}{2|k|}.}
$$

Its [distributional derivative](../../../../../distributional-derivative.md) verifies the delta equation, including its sign.

For a source for which the integral converges and the resulting function has the required decay, define

$$
\boxed{y(x)=\int_{\mathbb R}G(x;\xi)S(\xi)d\xi.}
$$

Applying the differential operator under the integral, or in the sense of [distributions](../../../../../distribution-mathematical-analysis.md), gives $\mathcal Ly=\int\delta(x-\xi)S(\xi)d\xi=S(x)$. A continuous integrable source, for example, makes this convolution vanish at both infinities and gives a classical solution. If there were two solutions, their difference would be $Ae^{ax}+Be^{-ax}$; decay at positive infinity forces $A=0$, and at negative infinity forces $B=0$. Thus **the decaying solution is unique whenever it exists**.

The assumptions needed for existence should not be dropped: an arbitrary source need not admit a decaying solution, as $S=1$ demonstrates. Also the displayed formula presupposes $k\ne0$; for $k=0$ no Green function for a point source can decay at both infinities, since its derivative must jump by one while both exterior linear pieces would have to be zero.

## ↑ Ancestors (10)

1. [6D](../6d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
