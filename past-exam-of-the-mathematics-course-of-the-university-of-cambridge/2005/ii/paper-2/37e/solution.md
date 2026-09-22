<h1 id="37e/solution">Solution</h1>

↑ **Parent:** [37E](../37e.md)

For a one-dimensional isentropic [perfect gas](../../../../../ideal-gas.md), [continuity](../../../../../continuous-function.md) and momentum are $D\rho=-\rho u_x$ and $Du=-c^2\rho_x/\rho$, where $D=\partial_t+u\partial_x$ and $c^2=\partial P/\partial\rho$. Since $P=K\rho^\gamma$, differentiation gives

$$
Dc=-\frac{\gamma-1}{2}cu_x,\qquad
Du=-\frac{2c}{\gamma-1}c_x.
$$

Thus applying $D+c\partial_x$ to $u+2(c-c_0)/(\gamma-1)$ cancels both terms:

$$
\boxed{(\partial_t+(u+c)\partial_x)\left[u+\frac{2(c-c_0)}{\gamma-1}\right]=0.}
$$

The complementary invariant $u-2(c-c_0)/(\gamma-1)$ is transported along $dx/dt=u-c$. In the right-running piston [simple wave](../../../../../simple-wave.md), those characteristics carry the undisturbed value zero, giving $c=c_0+(\gamma-1)u/2$.

A right-running characteristic emitted by the piston at time $\tau$ has $u=f\tau$ and speed $u+c=c_0+(\gamma+1)f\tau/2$, constant along that characteristic. It starts at $x=f\tau^2/2$, so

$$
x(t;\tau)=\frac12f\tau^2+\left(c_0+\frac{\gamma+1}{2}f\tau\right)(t-\tau).
$$

Neighboring characteristics first intersect when $\partial x/\partial\tau=0$. This derivative is $\frac{\gamma+1}{2}ft-c_0-\gamma f\tau$, so the envelope time is

$$
t(\tau)=\frac{2c_0}{(\gamma+1)f}+\frac{2\gamma}{\gamma+1}\tau.
$$

For $\gamma>1$, it is smallest at $\tau=0$. Consequently the first gradient catastrophe and ensuing [shock](../../../../../shock-wave.md) form at

$$
\boxed{t_* =\frac{2c_0}{(\gamma+1)f},\qquad
x_* =c_0t_* =\frac{2c_0^2}{(\gamma+1)f}.}
$$

This uses the smooth isentropic simple-wave solution up to its first characteristic crossing, not beyond the newly formed [shock](../../../../../shock-wave.md).

## ↑ Ancestors (10)

1. [37E](../37e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
