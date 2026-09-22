<h1 id="30c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Rotate the polar axis to $\xi$. Since $W_t$ is a finite sphere measure, its [Fourier transform](../../../../../../fourier-transform.md) is

$$
\widehat W_t(\xi)=\frac{t}{4\pi}\int_{S^2}e^{-it\xi\cdot\omega}\,d\Omega
=\frac t2\int_{-1}^1e^{-it|\xi|s}\,ds
=\boxed{\frac{\sin(t|\xi|)}{|\xi|}},
$$

with value $t$ at $\xi=0$. Fourier transforming the [wave equation](../../../../../../wave-equation-split.md) gives $\widehat u_{tt}+|\xi|^2\widehat u=0$ with initial displacement zero and velocity $\widehat g$. Its solution is this multiplier times $\widehat g$, so inversion gives $u=W_t*g$. Thus the [Kirchhoff formula](../../../../../../kirchhoff-formula.md) is

$$
\boxed{u(t,x)=\frac1{4\pi t}\int_{|y-x|=t}g(y)\,d\Sigma(y)
=\frac t{4\pi}\int_{S^2}g(x+t\omega)\,d\Omega.}
$$

This extends to arbitrary smooth $g$, without any growth restriction: for each finite spacetime neighborhood, multiply $g$ by a compactly supported smooth cutoff equal to one on every sphere occurring in that neighborhood. The formula is unchanged there, so its verified differential equation remains valid locally. Its initial values follow from $u(t,x)=tg(x)+o(t)$ and differentiation under the sphere integral. Since the neighborhood was arbitrary, it is a smooth solution everywhere for $t\geq0$.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [30C](../../30c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
