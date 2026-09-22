<h1 id="37c/solution">Solution</h1>

↑ **Parent:** [37C](../37c.md)

For an isentropic [perfect gas](../../../../../ideal-gas.md), $p=K\rho^\gamma$ and $c^2=dp/d\rho$. The one-dimensional [Euler equations](../../../../../euler-equations-for-an-inviscid-fluid.md) give $D\rho=-\rho u_x$ and $Du=-c^2\rho_x/\rho$, where $D=\partial_t+u\partial_x$. Since $dc/d\rho=(\gamma-1)c/(2\rho)$, these become

$$
Du=-\frac{2c}{\gamma-1}c_x,\qquad Dc=-\frac{\gamma-1}{2}c u_x.
$$

Adding the appropriate $\pm c\partial_x$ terms shows

$$
\boxed{(\partial_t+(u\pm c)\partial_x)\left[u\pm\frac{2(c-c_0)}{\gamma-1}\right]=0.}
$$

These are the [Riemann invariants](../../../../../riemann-invariant.md). A [simple wave](../../../../../simple-wave.md) is a solution in which one invariant is spatially and temporally constant, so all local state variables depend on the other one. For a right-moving wave connected to rest, the minus invariant is zero and $c=c_0+(\gamma-1)u/2$. The plus characteristic then has speed $u+c=c_0+(\gamma+1)u/2$, giving

$$
\boxed{u_t+\left(c_0+\frac{\gamma+1}{2}u\right)u_x=0.}
$$

For the supplied damped equation put $b=(\gamma+1)/2$. Along $\dot x=c_0+bu$, $\dot u=-\alpha u$, so an initial label $x_0$ gives

$$
\boxed{u=v(x_0)e^{-\alpha t},\qquad
x-c_0t=x_0+\frac b\alpha(1-e^{-\alpha t})v(x_0).}
$$

This solves the initial-value problem while the label map remains invertible. Its derivative is $1+(b/\alpha)(1-e^{-\alpha t})v'(x_0)$. Nonnegative slopes cannot cause crossing; for negative slopes, the condition $\alpha>b\sup_{v'<0}|v'|$ keeps that derivative strictly positive. Hence **the stated damping condition prevents [shock](../../../../../shock-wave.md) formation at every finite time**. Equality also avoids a finite-time crossing, although the derivative may tend to zero as time tends to infinity. The strict inequality in the question is sufficient rather than necessary.

## ↑ Ancestors (10)

1. [37C](../37c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
