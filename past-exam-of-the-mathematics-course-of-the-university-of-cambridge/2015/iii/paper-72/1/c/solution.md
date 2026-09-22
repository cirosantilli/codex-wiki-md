<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [stationary points](../../../../../../stationary-point.md) of the exponent are $t=1/3$ and $t=1$, because $\phi'(t)=(3t-1)(t-1)$. The first is a local maximum with $\phi(1/3)=4/27$ and $\phi''(1/3)=-2$; the second is a local minimum. Also

$$
\phi(t)-\frac4{27}=(t-\tfrac13)^2(t-\tfrac43),
$$

so the endpoint overtakes the interior maximum only when $b>4/3$.

For fixed $0<b<1/3$, the upper endpoint is the unique maximum. Linearizing the exponent there gives the [Laplace endpoint estimate](../../../../../../laplace-endpoint-estimate.md) $e^{\lambda\phi(b)}/(\lambda\phi'(b))$. At $b=1/3$, only half of the local [Gaussian integral](../../../../../../gaussian-integral.md) is included. For $1/3<b\leq4/3$, the whole Gaussian near $1/3$ contributes. At $b=4/3$ an endpoint has the same exponential height, but its prefactor is $\lambda^{-1}$, smaller than the interior $\lambda^{-1/2}$ prefactor. For $b>4/3$, the endpoint has strictly greater height and dominates.

Consequently **all fixed-$b$ regimes are**

$$
\boxed{I(\lambda)\sim
\begin{cases}
\dfrac{e^{\lambda b(b-1)^2}}{\lambda(3b^2-4b+1)},&0<b<\tfrac13,\\[6pt]
\dfrac{\sqrt\pi}{2\sqrt\lambda}e^{4\lambda/27},&b=\tfrac13,\\[6pt]
\dfrac{\sqrt\pi}{\sqrt\lambda}e^{4\lambda/27},&\tfrac13<b\leq\tfrac43,\\[6pt]
\dfrac{e^{\lambda b(b-1)^2}}{\lambda(3b^2-4b+1)},&b>\tfrac43.
\end{cases}}
$$

The estimate follows from [Laplace's method](../../../../../../laplace-s-method.md); the tail toward negative infinity is exponentially harmless since the cubic tends to negative infinity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 72](../../../paper-72-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
