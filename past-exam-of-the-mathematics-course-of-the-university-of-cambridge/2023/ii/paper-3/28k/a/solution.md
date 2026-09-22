<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $f_i$ be the [multivariate normal density](../../../../../../multivariate-normal-density.md) of $N_p(\mu_i,\Sigma_i)$. Under zero-one loss, the [Bayes classifier](../../../../../../bayes-classifier.md) chooses the class with the larger posterior probability. Thus

$$
\boxed{
\delta_{\pi_0}(x)
=\mathbf1\{\pi_1f_1(x)\geq\pi_0f_0(x)\},
\qquad \pi_1=1-\pi_0.}
$$

Equivalently, it chooses class one when the log posterior odds

$$
\begin{aligned}
D_{\pi_0}(x)
={}&\log\frac{\pi_1}{\pi_0}
+\frac12\log\frac{\det\Sigma_0}{\det\Sigma_1}\\
&-\frac12(x-\mu_1)^T\Sigma_1^{-1}(x-\mu_1)
+\frac12(x-\mu_0)^T\Sigma_0^{-1}(x-\mu_0)
\end{aligned}
$$

is nonnegative. The decision boundary is $D_{\pi_0}(x)=0$.

If $\Sigma_0=\Sigma_1=\Sigma$, the $x^T\Sigma^{-1}x$ terms cancel, leaving

$$
D_{\pi_0}(x)
=(\mu_1-\mu_0)^T\Sigma^{-1}x+C,
$$

an affine function. This is the linear boundary of [linear discriminant analysis](../../../../../../linear-discriminant-analysis.md). If $\Sigma_0\ne\Sigma_1$, the quadratic part is

$$
\frac12x^T(\Sigma_0^{-1}-\Sigma_1^{-1})x,
$$

which is nonzero, so the boundary is a possibly degenerate quadratic hypersurface, as in [quadratic discriminant analysis](../../../../../../quadratic-discriminant-analysis.md). This is the [Gaussian Bayes classifier](../../../../../../gaussian-bayes-classifier.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
