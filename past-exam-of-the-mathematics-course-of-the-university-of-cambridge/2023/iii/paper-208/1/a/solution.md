<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

If $X$ is [sub-Gaussian](../../../../../../sub-gaussian-distribution.md) with variance parameter $\nu$, then

$$
\mathbb E e^{\lambda X}\leq e^{\lambda^2\nu/2}
$$

for every $\lambda\in\mathbb R$. Restricting this inequality to $|\lambda|<1/\alpha$ proves that $X$ is [sub-exponential](../../../../../../subexponential-distribution-light-tailed.md) with parameters $(\nu,\alpha)$ for every $\alpha>0$.

Now let $X=Z^2-1$ for a standard [normal distribution](../../../../../../normal-distribution.md) variable $Z$. Its [moment-generating function](../../../../../../moment-generating-function.md) is

$$
\mathbb E e^{\lambda X}
=\frac{e^{-\lambda}}{\sqrt{1-2\lambda}},
\qquad \lambda<\frac12,
$$

and is infinite for $\lambda\geq1/2$. A sub-Gaussian moment-generating function must be finite for every real $\lambda$, so $X$ cannot be sub-Gaussian with any finite parameter. For $|\lambda|<1/4$, the stated inequality gives

$$
\mathbb E e^{\lambda X}
\leq e^{2\lambda^2}
=e^{\lambda^2(4)/2}.
$$

**Thus $X$ is sub-exponential with parameters $(4,4)$.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 208](../../../paper-208-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
