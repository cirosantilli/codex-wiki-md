<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The population [survivor function](../../../../../../survival-function.md) is the probability that a randomly selected person, averaging over their unobserved frailty, has not experienced the event by time $t$. Here the conditional hazard $U\theta$ is constant, so the conditional survival is $e^{-U\theta t}$. For $\theta>0$, the uniform frailty density equals one on its interval, giving the [uniform frailty survival mixture](../../../../../../uniform-frailty-survival-mixture.md)

$$
\overline S(t)=\int_{1/2}^{3/2}e^{-u\theta t}\,du
=\boxed{\frac{e^{-\theta t/2}-e^{-3\theta t/2}}{\theta t}},\qquad t>0.
$$

At $t=0$ its continuous extension is $\overline S(0)=1$, since the numerator is $\theta t+O(t^2)$. This is the [Laplace transform](../../../../../../laplace-transform.md) of the uniform frailty density at argument $\theta t$. It is not $e^{-\theta t}$: averaging individual survivor functions does not equal exponentiating the mean hazard. If $\theta=0$, every individual hazard is zero and $\overline S(t)=1$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
