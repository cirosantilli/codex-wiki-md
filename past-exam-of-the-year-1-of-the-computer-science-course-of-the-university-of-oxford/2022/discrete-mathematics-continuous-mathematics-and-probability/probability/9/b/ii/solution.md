<h1 id="probability/9/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

First $0\le M_n\le\sum_iE_i$, so [linearity of expectation](../../../../../../../linearity-of-expectation.md) gives $\mathbb E M_n\le n<\infty$. The [tail integral formula for expectation](../../../../../../../tail-integral-formula-for-expectation.md), followed by the finite [binomial theorem](../../../../../../../binomial-theorem.md) expansion, gives

$$
\begin{aligned}
\mathbb E M_n&=\int_0^\infty\left[1-(1-e^{-x})^n\right]dx\\
&=\sum_{k=1}^n(-1)^{k+1}\binom nk\int_0^\infty e^{-kx}dx\\
&=\boxed{\sum_{k=1}^n\binom nk\frac{(-1)^{k+1}}k.}
\end{aligned}
$$

The exchange involves only a finite sum. As a useful check, substitution $t=e^{-x}$ rewrites the integral as $\int_0^1[1-(1-t)^n]/t\,dt=\sum_{j=0}^{n-1}\int_0^1(1-t)^jdt=\sum_{k=1}^n1/k$, the [harmonic number](../../../../../../../harmonic-number.md) $H_n$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [9](../../../9.md)
4. [Probability](../../../../probability.md)
5. [Discrete mathematics, continuous mathematics, and probability](../../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
6. [2022](../../../../../split.md)
7. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../../split.md)
8. [Year 1 of the computer science course of the University of Oxford](../../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
9. [Computer science course of the University of Oxford](../../../../../../../computer-science-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../../split.md)
