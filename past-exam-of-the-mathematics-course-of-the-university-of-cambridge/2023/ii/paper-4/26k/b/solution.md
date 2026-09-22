<h1 id="26k/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $(Y_n)$ be [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with the standard [Cauchy distribution](../../../../../../cauchy-distribution.md), whose [probability density function](../../../../../../probability-density-function.md) is

$$
f(y)=\frac{1}{\pi(1+y^2)}.
$$

Its first absolute moment diverges since

$$
\mathbb E|Y_1|=\frac{2}{\pi}\int_0^\infty\frac{y}{1+y^2}\,dy=\infty.
$$

On the other hand, its [characteristic function](../../../../../../characteristic-function.md) is $\varphi(t)=e^{-|t|}$. The [characteristic function of a sum of independent variables](../../../../../../characteristic-function-of-a-sum-of-independent-variables.md) therefore gives

$$
\mathbb E\exp\left(it\frac{S_n}{n}\right)
=\varphi(t/n)^n=e^{-|t|}.
$$

Thus the [stability of the Cauchy distribution](../../../../../../stability-of-the-cauchy-distribution.md) implies that $S_n/n$ has the standard Cauchy distribution for every $n$. In particular,

$$
\frac{Y_1+\cdots+Y_n}{n}\xrightarrow{d}Z,
$$

where $Z$ is standard Cauchy and $\xrightarrow d$ denotes [convergence in distribution](../../../../../../convergence-in-distribution.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [26K](../../26k.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
