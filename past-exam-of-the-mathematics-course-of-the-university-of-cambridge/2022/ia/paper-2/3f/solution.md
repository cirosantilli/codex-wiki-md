<h1 id="3f/solution">Solution</h1>

↑ **Parent:** [3F](../3f.md)

A function $f$ on an interval is a [convex function](../../../../../convex-function.md) if

$$
f(tx+(1-t)y)\leq tf(x)+(1-t)f(y)
\qquad(0\leq t\leq1).
$$

[Jensen inequality](../../../../../jensen-s-inequality.md) states that for an integrable random variable $X$, when all terms are defined,

$$
f(\mathbb E X)\leq\mathbb E[f(X)].
$$

The function $\phi(x)=x\log x$ is convex on $(0,\infty)$ because

$$
\phi''(x)=\frac1x>0.
$$

Applying Jensen's inequality to the uniform distribution on the positive numbers $x_1,\ldots,x_n$ gives

$$
\frac1n\sum_{i=1}^nx_i\log x_i
\geq
\left(\frac1n\sum_{i=1}^nx_i\right)
\log\left(\frac1n\sum_{i=1}^nx_i\right).
$$

Writing $S=\sum_i x_i$ and multiplying by $n/S$ yields

$$
\boxed{
\frac{\sum_{i=1}^nx_i\log x_i}{\sum_{i=1}^nx_i}
\geq\log\left(\frac{\sum_{i=1}^nx_i}{n}\right)}.
$$

## ↑ Ancestors (10)

1. [3F](../3f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
