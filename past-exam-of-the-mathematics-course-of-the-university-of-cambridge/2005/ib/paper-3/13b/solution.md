<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

For a [homogeneous function](../../../../../homogeneous-function.md), fix $x\in U$ and differentiate $f(\lambda x)=\lambda^cf(x)$ at $\lambda=1$. The [chain rule](../../../../../chain-rule.md) gives

$$
\boxed{Df_x(x)=cf(x)}.
$$

Conversely, assume this derivative identity throughout $U$. Along a positive ray define $h(\lambda)=\lambda^{-c}f(\lambda x)$. The ray stays in $U$ by hypothesis, and linearity of the derivative gives

$$
h'(\lambda)=\lambda^{-c-1}\{Df_{\lambda x}(\lambda x)-cf(\lambda x)\}=0.
$$

Therefore $h$ is constant on the connected interval $(0,\infty)$ and equals $h(1)=f(x)$. Hence $\boxed{f(\lambda x)=\lambda^cf(x)}$ for every positive $\lambda$. This proves [Euler differential identity characterizes homogeneity](../../../../../euler-differential-identity-characterizes-homogeneity.md); no connectedness assumption on the whole domain is needed.

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
