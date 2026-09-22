<h1 id="29l/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $y=0,1,\ldots$,

$$
\mathbb P_\theta(Y_i=y)=e^{-\theta y}(1-e^{-\theta}),
$$

so $Y_i$ is geometric with success probability $1-e^{-\theta}$. The log likelihood is

$$
n\log(1-e^{-\theta})-n\theta\overline Y.
$$

Its score equation gives

$$
e^{-\theta}=\frac{\overline Y}{1+\overline Y},
$$

and hence

$$
\widetilde\theta_n=\log\left(\frac{1+\overline Y}{\overline Y}\right).
$$

When $\overline Y=0$, the extended MLE is $+\infty$; this event has probability tending to zero.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [29L](../../../29l.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
