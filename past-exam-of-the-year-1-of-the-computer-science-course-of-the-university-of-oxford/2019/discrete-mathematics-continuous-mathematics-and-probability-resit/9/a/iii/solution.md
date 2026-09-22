<h1 id="9/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $X_1,X_2$ be the two [independent](../../../../../../independent-random-variables.md) [Poisson random variables](../../../../../../poisson-distribution.md). For $k\geq0$, their discrete [convolution](../../../../../../convolution.md) is

$$
\begin{aligned}
\mathbb P(X_1+X_2=k)&=\sum_{j=0}^k\mathbb P(X_1=j)\mathbb P(X_2=k-j)\\
&=\frac{e^{-(\lambda+\mu)}}{k!}\sum_{j=0}^k\binom kj\lambda^j\mu^{k-j}\\
&=e^{-(\lambda+\mu)}\frac{(\lambda+\mu)^k}{k!},
\end{aligned}
$$

where the last equality is the [binomial theorem](../../../../../../binomial-theorem.md). Thus **$X_1+X_2\sim\operatorname{Poisson}(\lambda+\mu)$**.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [9](../../../9.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
