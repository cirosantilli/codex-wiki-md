<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

This is a symmetric [Beta distribution](../../../../../../beta-distribution.md) with parameters $(2,2)$, so its mean and [median](../../../../../../median.md) are both $1/2$. At the [median](../../../../../../median.md) its [probability density function](../../../../../../probability-density-function.md) is $f(1/2)=3/2$, giving [asymptotic variance](../../../../../../asymptotic-variance.md) $1/9$ for the [sample median](../../../../../../sample-median.md). Direct integration gives

$$
\mathbb EX=\frac12,\qquad \mathbb EX^2=6\int_0^1x^3(1-x)\,dx=\frac3{10},\qquad \operatorname{Var}(X)=\frac1{20}.
$$

Consequently $\sqrt n(\bar X_n-1/2)\xrightarrow{d}N(0,1/20)$. **The [sample median](../../../../../../sample-median.md) has $20/9$ times the [asymptotic variance](../../../../../../asymptotic-variance.md) of the [sample mean](../../../../../../sample-mean.md)**, with [asymptotic relative efficiency](../../../../../../asymptotic-relative-efficiency.md)

$$
\boxed{\operatorname{ARE}(\text{median},\text{mean})=\frac9{20}.}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
