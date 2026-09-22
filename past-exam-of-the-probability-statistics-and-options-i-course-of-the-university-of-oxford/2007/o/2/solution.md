<h1 id="o/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [statistical power](../../../../statistical-power.md) of a test $\varphi$ is $\beta(\theta)=\mathbb E_\theta\varphi(X)$, its rejection [probability](../../../../probability.md) at parameter $\theta$. Its size is $\sup_{\theta\in H_0}\beta(\theta)$; for a simple null this is just $\beta(\theta_0)$.

The [Neyman-Pearson lemma](../../../../neyman-pearson-lemma.md) states that for testing a simple null [probability density function](../../../../probability-density-function.md) $f_0$ against a simple alternative [probability density function](../../../../probability-density-function.md) $f_1$, a test rejecting where $f_1/f_0>k$, accepting where it is below $k$, and if needed randomizing on equality to attain the desired size is most powerful among all tests of that size. It follows by integrating $(\varphi-\varphi_*)(f_1-kf_0)\leq0$ and using the size constraint.

The proposed [probability density function](../../../../probability-density-function.md) is nonnegative, and

$$
\int_0^\infty f(x;\theta)dx
=\frac{\theta^2}{\theta+1}
\left(\frac1{\theta^2}+\frac1\theta\right)=1.
$$

For an independent sample, cancellation of the factors $(x_i+1)$ in the [likelihood ratio](../../../../likelihood-ratio.md) gives

$$
\frac{L(\theta_1)}{L(\theta_0)}
=\left[\frac{\theta_1^2/(\theta_1+1)}
{\theta_0^2/(\theta_0+1)}\right]^n
\exp\left((\theta_0-\theta_1)\sum_i x_i\right).
$$

For $\theta_1<\theta_0$ this is increasing in $S=\sum_iX_i$. The most powerful test therefore has [rejection region](../../../../rejection-region.md)

$$
\boxed{S>c_\alpha,\qquad
\mathbb P_{\theta_0}(S>c_\alpha)=\alpha.}
$$

The sum has a continuous positive [probability density function](../../../../probability-density-function.md) on $(0,\infty)$, so no boundary randomization is required. The threshold depends on the null and chosen size, but not on which $\theta_1<\theta_0$ was specified. The same test is therefore **a [uniformly most powerful test](../../../../uniformly-most-powerful-test.md) for the composite alternative $0<\theta<\theta_0$**.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [O](../../o.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
