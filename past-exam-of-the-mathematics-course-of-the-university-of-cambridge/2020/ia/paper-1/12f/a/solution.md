<h1 id="12f/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [standard normal density](../../../../../../standard-normal-density.md) is

$$
\phi(z)=\frac1{\sqrt{2\pi}}e^{-z^2/2},
\qquad z\in\mathbb R.
$$

It is nonnegative, and the [Gaussian integral](../../../../../../gaussian-integral.md) gives $\int_{-\infty}^{\infty}\phi(z)\,dz=1$, so it is a [probability density function](../../../../../../probability-density-function.md). Completing the square gives the [moment-generating function of a standard normal variable](../../../../../../moment-generating-function-of-a-standard-normal-variable.md)

$$
M_Z(\theta)=\int e^{\theta z}\phi(z)\,dz
=e^{\theta^2/2}.
$$

Thus $\mathbb EZ=M_Z'(0)=0$ and

$$
\boxed{\operatorname{var}(Z)=M_Z''(0)-M_Z'(0)^2=1.}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
