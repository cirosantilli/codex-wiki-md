<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under [Wiener measure](../../../../../../wiener-measure.md), the endpoint has [normal distribution](../../../../../../normal-distribution.md) $N(x,tI_d)$. For $t>0$ and $1+\lambda t>0$, the [Gaussian integral](../../../../../../gaussian-integral.md) is

$$
\mathbb E_{\mathbb Q^x}e^{-\lambda|\omega_t|^2/2}
=(2\pi t)^{-d/2}\int_{\mathbb R^d}
\exp\!\left(-\frac{|z-x|^2}{2t}-\frac\lambda2|z|^2\right)dz.
$$

Complete the square:

$$
-\frac{|z-x|^2}{2t}-\frac\lambda2|z|^2
=-\frac{1+\lambda t}{2t}\left|z-\frac{x}{1+\lambda t}\right|^2
-\frac{\lambda|x|^2}{2(1+\lambda t)}.
$$

Evaluating the centered Gaussian gives $(1+\lambda t)^{-d/2}\exp[-\lambda|x|^2/(2(1+\lambda t))]$. With the preceding prefactor, the [critical quadratic potential for the Ornstein-Uhlenbeck generator](../../../../../../critical-quadratic-potential-for-the-ornstein-uhlenbeck-generator.md) solution is

$$
\boxed{u(t,x)=\frac{e^{\lambda dt/2}}{(1+\lambda t)^{d/2}}
\exp\!\left(\frac{\lambda^2t|x|^2}{2(1+\lambda t)}\right).}
$$

The initial value is one. As a direct PDE check, write $u=a(t)e^{b(t)|x|^2/2}$, where

$$
b(t)=\frac{\lambda^2t}{1+\lambda t},\qquad
\frac{a'(t)}{a(t)}=\frac d2b(t),\qquad
b'(t)=(b(t)-\lambda)^2.
$$

Since $\nabla u=bxu$ and $\Delta u=(db+b^2|x|^2)u$, these identities give precisely the required time derivative and spatial operator.

For $\lambda\ge0$, this is finite for every $t\ge0$; at $\lambda=0$ it reduces to $u=1$. If the parameter is allowed to be negative, the [expectation](../../../../../../expected-value.md) is finite only for $t<-1/\lambda$. At and beyond that time the quadratic coefficient in the endpoint Gaussian integral is nonnegative, so the integral diverges. A nonnegative classical solution on the entire half-line cannot then exist: stopping the Feynman-Kac [martingale](../../../../../../martingale-split.md) in balls and discarding its nonnegative boundary term bounds any such solution below by the truncated path expectations; their limit is infinite. Thus the printed global positive-solution premise implicitly requires the nonnegative parameter convention.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
