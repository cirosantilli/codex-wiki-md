<h1 id="3/3/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Apply the [Feynman-Kac formula](../../../../../../../feynman-kac-formula.md) with $V(x)=\sigma x$ and terminal function $1$. The ansatz $u(t,x)=e^{A(t)x+C(t)}$ gives

$$
A'=-\sigma,\qquad C'=\frac12A^2,qquad A(0)=C(0)=0.
$$

Thus $A(t)=-\sigma t$ and $C(t)=\sigma^2t^3/6$, so

$$
\boxed{\mathbb E_x\exp\left(-\sigma\int_0^tB_sds\right)
=\exp\left(-\sigma tx+\frac{\sigma^2t^3}{6}\right).}
$$

Equivalently, the [Integral of Brownian motion](../../../../../../../integral-of-brownian-motion.md) is Gaussian with mean $xt$ and variance $t^3/3$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [3](../../3.md)
3. [3](../../../3.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2019](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
