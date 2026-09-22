<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Introduce $t=\mu y/(2\lambda)\ge0$. Solving the quadratic and using its product of roots gives

$$
\boxed{x_\pm(y)=\mu\left(1+t\pm\sqrt{t(t+2)}\right),
\qquad x_-(y)x_+(y)=\mu^2.}
$$

Both roots are positive, with $x_-\le\mu\le x_+$; equality occurs only for $y=0$. For computation, the smaller root has the equivalent cancellation-free form

$$
\boxed{x_-(y)=\frac{\mu}{1+t+\sqrt{t(t+2)}},
\qquad x_+(y)=\frac{\mu^2}{x_-(y)}.}
$$

This is [stable root evaluation for inverse Gaussian sampling](../../../../../../stable-root-evaluation-for-inverse-gaussian-sampling.md).

Define $h(x)=\lambda(x-\mu)^2/(\mu^2x)$. It decreases from infinity to zero on $(0,\mu)$ and increases from zero to infinity on $(\mu,\infty)$, since

$$
h'(x)=\frac{\lambda}{\mu^2}\left(1-\frac{\mu^2}{x^2}\right).
$$

The two roots are precisely its inverse branches. This supplies the Jacobians needed for the [reciprocal-root inverse Gaussian sampler](../../../../../../reciprocal-root-inverse-gaussian-sampler.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
