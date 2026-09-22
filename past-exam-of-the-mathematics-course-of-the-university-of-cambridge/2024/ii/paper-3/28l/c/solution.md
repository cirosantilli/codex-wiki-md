<h1 id="28l/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Under the uniform prior, the posterior density after $X=x$ is proportional to $\theta^x(1-\theta)^{n-x}$. For $0<x<n$, differentiating posterior risk gives the unique stationary point

$$
a=
\frac{\mathbb E[(1-\theta)^{-1}\mid x]}
     {\mathbb E[(\theta(1-\theta))^{-1}\mid x]}
=\frac{B(x+1,n-x)}{B(x,n-x)}=\frac xn.
$$

Strict convexity makes it the unique minimum. For $x=0$, every $a\ne0$ gives infinite posterior risk at zero and $a=0$ is optimal; symmetrically $a=1$ is optimal for $x=n$. Hence the unique Bayes rule is $\delta(x)=x/n$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [28L](../../28l.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
