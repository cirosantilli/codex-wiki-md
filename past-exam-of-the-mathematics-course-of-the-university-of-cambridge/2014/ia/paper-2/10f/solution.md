<h1 id="10f/solution">Solution</h1>

↑ **Parent:** [10F](../10f.md)

For $\lambda\geq0$, a [Poisson distribution](../../../../../poisson-distribution.md) has mass $\mathbb P(X=k)=e^{-\lambda}\lambda^k/k!$ for $k=0,1,\ldots$; at $\lambda=0$ it is concentrated at zero. Its [moment-generating function](../../../../../moment-generating-function.md) is

$$
\boxed{M_X(s)=\sum_{k\ge0}e^{sk}e^{-\lambda}\frac{\lambda^k}{k!}=\exp[\lambda(e^s-1)],\qquad s\in\mathbb R.}
$$

For independent $X,Y$, the [moment-generating function](../../../../../moment-generating-function.md) of their sum is the product, $\exp[(\lambda+\mu)(e^s-1)]$. Uniqueness of the [moment-generating function](../../../../../moment-generating-function.md) near zero therefore gives **$X+Y\sim\operatorname{Poisson}(\lambda+\mu)$**. Repeating the argument gives **$S_n=\sum_{i=1}^nX_i\sim\operatorname{Poisson}(n)$** when every parameter is one.

The displayed sequence is $a_n=\mathbb P(S_n\leq n)$. The classical [central limit theorem](../../../../../central-limit-theorem.md) states that independent identically distributed variables with finite mean $m$ and nonzero finite [variance](../../../../../variance-split.md) $\sigma^2$ have standardized sum $(S_n-nm)/(\sigma\sqrt n)$ converging in distribution to the standard [normal distribution](../../../../../normal-distribution.md). Here $m=\sigma^2=1$, so

$$
\boxed{a_n=\mathbb P\left(\frac{S_n-n}{\sqrt n}\leq0\right)\longrightarrow\Phi(0)=\frac12.}
$$

Convergence of the distribution functions at the continuity point zero justifies the last step. This is the [Poisson cumulative probability at its growing mean](../../../../../poisson-cumulative-probability-at-its-growing-mean.md).

## ↑ Ancestors (10)

1. [10F](../10f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ia](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
