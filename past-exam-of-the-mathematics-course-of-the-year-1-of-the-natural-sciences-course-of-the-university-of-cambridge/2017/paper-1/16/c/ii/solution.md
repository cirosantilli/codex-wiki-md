<h1 id="16/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $s>0$, integrate the [probability density function](../../../../../../probability-density-function.md) to obtain the [cumulative distribution function](../../../../../../cumulative-distribution-function.md)

$$
F_X(x)=\frac12\left[1+\tanh\!\left(\frac{x-\mu}{2s}\right)\right].
$$

If $\mu>0$, the requested [probability](../../../../../../probability.md) is $F_X(\mu)-F_X(0)$. Since the [hyperbolic tangent](../../../../../../hyperbolic-tangent.md) is odd, this gives

$$
\boxed{\mathbb P(0<X<\mu)=
\begin{cases}
\dfrac12\tanh\!\left(\dfrac{\mu}{2s}\right),&\mu>0,\\
0,&\mu\leq0.
\end{cases}}
$$

The second case matters because the question places no sign restriction on $\mu$: the event is empty when its upper endpoint is nonpositive. Using an oriented [integral](../../../../../../integral-split.md) from $0$ to a negative $\mu$ would give a negative number, not a [probability](../../../../../../probability.md).

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [16](../../../16.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
