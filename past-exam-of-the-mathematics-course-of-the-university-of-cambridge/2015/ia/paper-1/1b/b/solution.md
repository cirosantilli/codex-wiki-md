<h1 id="1b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $q=e^{i\theta}$. Since $q\ne1$, the [finite geometric series](../../../../../../finite-geometric-series.md) gives

$$
\sum_{m=1}^N q^m=\frac{q(1-q^N)}{1-q}=\frac{q-1-q^{N+1}+q^N}{2(1-\cos\theta)},
$$

where the second equality multiplies numerator and denominator by $1-\overline q$. Taking imaginary parts gives the [finite trigonometric sum](../../../../../../finite-trigonometric-sum.md)

$$
\boxed{\sum_{m=1}^N\sin(m\theta)=\frac{\sin\theta+\sin(N\theta)-\sin((N+1)\theta)}{2(1-\cos\theta)}.}
$$

Taking real parts of the same [finite geometric series](../../../../../../finite-geometric-series.md) gives

$$
\boxed{\sum_{m=1}^N\cos(m\theta)=\frac{\cos\theta-1+\cos(N\theta)-\cos((N+1)\theta)}{2(1-\cos\theta)}.}
$$

The denominator is nonzero by the restriction on $\theta$. Equivalently, these [finite trigonometric sums](../../../../../../finite-trigonometric-sum.md) are $\sin(N\theta/2)\sin((N+1)\theta/2)/\sin(\theta/2)$ and $\sin(N\theta/2)\cos((N+1)\theta/2)/\sin(\theta/2)$, respectively.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1B](../../1b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ia](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
