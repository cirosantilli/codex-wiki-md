<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The coordinate-deletion functions from part c show that $Z$ is weakly self-bounding. Its negative centered moment-generating function therefore satisfies the [lower-tail concentration for a weakly self-bounding function](../../../../../../lower-tail-concentration-for-a-weakly-self-bounding-function.md) estimate

$$
\log\mathbb E e^{-\lambda(Z-\mathbb EZ)}
\leq\frac{\lambda^2\mathbb EZ}{2},
\qquad \lambda\geq0.
$$

Applying the [Chernoff bound](../../../../../../chernoff-bound.md), for every $\lambda\geq0$,

$$
\mathbb P(Z-\mathbb EZ<-t)
\leq\exp\left(-\lambda t+\frac{\lambda^2\mathbb EZ}{2}\right).
$$

The exponent is minimized at $\lambda=t/\mathbb EZ$, giving

$$
\boxed{\mathbb P(Z-\mathbb EZ<-t)
\leq\exp\left(-\frac{t^2}{2\mathbb EZ}\right).}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
