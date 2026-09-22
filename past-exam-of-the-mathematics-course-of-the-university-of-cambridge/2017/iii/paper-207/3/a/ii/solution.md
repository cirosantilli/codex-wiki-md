<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $A_2(t)=\int_0^t\mathbf1\{X(s)=2\}\,ds$ be the [occupation time of a continuous-time Markov chain](../../../../../../../occupation-time-of-a-continuous-time-markov-chain.md) in the symptoms state. [Tonelli theorem](../../../../../../../tonelli-theorem.md) permits exchanging the nonnegative integral and [expectation](../../../../../../../expected-value.md). Starting from state 1, put $q=\lambda+\mu>0$. Then

$$
\mathbb E_1A_2(t)=\int_0^tp_{12}(s)\,ds=\frac{\lambda}{q}\int_0^t(1-e^{-qs})\,ds,
$$

so

$$
\boxed{\mathbb E_1A_2(t)=\frac{\lambda}{\lambda+\mu}\left(t-\frac{1-e^{-(\lambda+\mu)t}}{\lambda+\mu}\right).}
$$

For small $t$ the answer is $\lambda t^2/2+O(t^3)$, as expected when onset must first occur. It is between zero and $t$. If $\lambda=\mu=0$, no transition can occur and the answer is zero; the displayed quotient is interpreted separately in that degenerate case.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 207](../../../../paper-207-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
