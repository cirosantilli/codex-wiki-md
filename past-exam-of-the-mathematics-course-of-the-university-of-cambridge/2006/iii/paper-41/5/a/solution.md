<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The sum of the two [independent](../../../../../../independent-random-variables.md) exponential times has a [hypoexponential distribution](../../../../../../hypoexponential-distribution.md). By [convolution of probability densities](../../../../../../convolution-of-independent-random-variables.md), for $t>0$ and $d=\lambda_1-\lambda_2>0$,

$$
\begin{aligned}
g(t)&=\int_0^t\lambda_1e^{-\lambda_1s}\lambda_2e^{-\lambda_2(t-s)}\,ds\\
&=\lambda_1\lambda_2e^{-\lambda_2t}\int_0^t e^{-ds}\,ds
=\frac{\lambda_1\lambda_2}{d}e^{-\lambda_2t}(1-e^{-dt}).
\end{aligned}
$$

Therefore

$$
\boxed{g(t)=\frac{\lambda_1\lambda_2}{\lambda_1-\lambda_2}
(e^{-\lambda_2t}-e^{-\lambda_1t}),\quad t>0,}
$$

and $g(t)=0$ for $t<0$. This is a nonnegative normalized [probability density function](../../../../../../probability-density-function.md). At the equal-rate boundary it tends to $\lambda^2te^{-\lambda t}$, a shape-two [Gamma distribution](../../../../../../gamma-distribution.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 41](../../../paper-41-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
