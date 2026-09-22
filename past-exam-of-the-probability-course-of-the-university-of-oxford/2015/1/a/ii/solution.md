<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Put $Z_n=n(1-M_n)$. Its [survival function](../../../../../survival-function.md) is

$$
\mathbb P(Z_n>z)=\begin{cases}
1,&z<0,\\
(1-z/n)^n,&0\leq z\leq n,\\
0,&z>n.
\end{cases}
$$

For each fixed $z\geq0$, eventually $n\geq z$, and the [exponential limit](../../../../../exponential-limit.md) gives $(1-z/n)^n\to e^{-z}$. Thus its [cumulative distribution function](../../../../../cumulative-distribution-function.md) tends to $0$ for $z<0$ and to $1-e^{-z}$ for $z\geq0$. This continuous limiting [cumulative distribution function](../../../../../cumulative-distribution-function.md) identifies the [exponential distribution](../../../../../exponential-distribution.md) with rate one:

$$
\boxed{n(1-M_n)\xrightarrow{\mathrm d}\operatorname{Exp}(1).}
$$

This is the [exponential endpoint limit of a uniform maximum](../../../../../exponential-endpoint-limit-of-a-uniform-maximum.md): the gap from the upper endpoint is typically of order $1/n$, although the maximum itself approaches a constant.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
