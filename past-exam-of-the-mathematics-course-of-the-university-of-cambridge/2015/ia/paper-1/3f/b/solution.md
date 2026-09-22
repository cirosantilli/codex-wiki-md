<h1 id="3f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $x$ sufficiently close to zero, $1+x>0$. Apply the [mean value theorem](../../../../../../mean-value-theorem.md) to the [logarithm](../../../../../../logarithm.md) between $1$ and $1+x$: there is a point $\xi_x$ between these endpoints with

$$
\frac{\log(1+x)}{x}=\frac1{\xi_x}.
$$

As $x\to0$ from either side, $\xi_x\to1$, so this quotient tends to $1$. The [exponential function](../../../../../../exponential-function.md) is continuous, and therefore

$$
\boxed{\lim_{x\to0}(1+x)^{1/x}=\lim_{x\to0}\exp\!\left(\frac{\log(1+x)}x\right)=e.}
$$

The hypotheses of the [mean value theorem](../../../../../../mean-value-theorem.md) hold because $\log t$ is continuous and differentiable for $t>0$, with derivative $1/t$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3F](../../3f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
