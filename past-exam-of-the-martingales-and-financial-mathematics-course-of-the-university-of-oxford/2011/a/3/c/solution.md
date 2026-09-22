<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $q=1-\epsilon<1$. The hypothesis implies $\mathbb P(\tau>n+N\mid\mathcal F_n)\leq q$. Since $\{\tau>n\}\in\mathcal F_n$ and survival to $n+N$ implies survival to $n$, the [tower property of conditional expectation](../../../../../law-of-total-expectation.md) gives

$$
\mathbb P(\tau>n+N)=\mathbb E\left[\mathbf1_{\{\tau>n\}}\mathbb P(\tau>n+N\mid\mathcal F_n)\right]
\leq q\,\mathbb P(\tau>n).
$$

Apply this at $n=0,N,2N,\ldots$ and use $\mathbb P(\tau>0)\leq1$ to obtain

$$
\boxed{\mathbb P(\tau>kN)\leq(1-\epsilon)^k.}
$$

This is a [geometric tail bound from a uniform escape probability](../../../../../geometric-tail-bound-from-a-uniform-escape-probability.md). The [tail-sum formula](../../../../../tail-sum-formula.md) for a nonnegative integer-valued variable now gives

$$
\boxed{\mathbb E\tau=\sum_{m\geq0}\mathbb P(\tau>m)
\leq N\sum_{k\geq0}(1-\epsilon)^k=\frac N\epsilon<\infty.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
