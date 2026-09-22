<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $Q(x)=1-\Phi(x)=\int_x^\infty\phi(t)\,dt$, where $\phi(t)=(2\pi)^{-1/2}e^{-t^2/2}$ is the [standard normal density](../../../../../../standard-normal-density.md). For $x>0$, $\phi'(t)=-t\phi(t)$ and [integration by parts](../../../../../../integration-by-parts.md) yield

$$
Q(x)=\int_x^\infty\frac{-\phi'(t)}t\,dt
=\frac{\phi(x)}x-\int_x^\infty\frac{\phi(t)}{t^2}\,dt.
$$

The boundary term at infinity vanishes. The remainder is nonnegative and is at most $Q(x)/x^2$, so

$$
\frac{x\phi(x)}{x^2+1}\leq Q(x)\leq\frac{\phi(x)}x.
$$

Dividing by the positive quantity $\phi(x)/x$ gives lower and upper bounds $x^2/(x^2+1)$ and $1$. The [squeeze theorem](../../../../../../squeeze-theorem.md) proves the [Mills ratio](../../../../../../mills-ratio.md) asymptotic

$$
\boxed{1-\Phi(x)\sim\frac{\phi(x)}x\qquad(x\to\infty).}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
