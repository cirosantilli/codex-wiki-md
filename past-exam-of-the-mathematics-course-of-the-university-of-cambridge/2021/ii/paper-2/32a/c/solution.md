<h1 id="32a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\sinh(x\Phi)=(e^{x\Phi}-e^{-x\Phi})/2$. The global maximum of $\Phi$ is the nonstationary endpoint $t=1$, where

$$
\Phi(1)=1,\qquad \Phi'(1)=6.
$$

Endpoint [Laplace's method](../../../../../../laplace-s-method.md) therefore gives

$$
\frac12\int_0^1e^{x\Phi(t)}dt\sim\frac{e^x}{12x}.
$$

The second exponential has its maximum at $t=1/2$ and is only of order $x^{-1/2}e^{x/8}$, exponentially smaller. Hence

$$
\boxed{J(x)\sim\frac{e^x}{12x}}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [32A](../../32a.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
