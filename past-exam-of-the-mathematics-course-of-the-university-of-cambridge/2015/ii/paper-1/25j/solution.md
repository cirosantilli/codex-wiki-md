<h1 id="25j/solution">Solution</h1>

↑ **Parent:** [25J](../25j.md)

The [James–Stein estimator](../../../../../james-stein-estimator.md) in the specified unit-variance model is

$$
\boxed{\hat\theta_{\rm STEIN}(X)=\left(1-\frac{p-2}{\|X\|^2}\right)X},
$$

with an arbitrary value at $X=0$, a probability-zero event. The risk of $X$ is $p$. [Gaussian Stein identity](../../../../../stein-s-lemma-probability.md) states $E_\theta[(X_i-\theta_i)g_i(X)]=E_\theta[\partial_i g_i(X)]$ for suitably integrable differentiable functions; it extends to the present singular function by truncation, since $p>2$ makes $E\|X\|^{-2}$ finite.

Put $c=p-2$ and $g(x)=-cx/\|x\|^2$. Then $\|g\|^2=c^2/\|x\|^2$ and $\operatorname{div}g=-c(p-2)/\|x\|^2$. Expanding the [quadratic risk](../../../../../quadratic-risk.md) and applying Stein's lemma yields

$$
\boxed{R(\theta,\hat\theta)=p-(p-2)^2E_\theta\frac1{\|X\|^2}<p=R(\theta,X)}.
$$

Thus domination is strict for every finite $\theta$.

To identify the worst-case risk, let $r=\|\theta\|\to\infty$. On $\|X\|>r/2$, the reciprocal square is at most $4/r^2$. On the complementary ball, the Gaussian density is at most $(2\pi)^{-p/2}e^{-r^2/8}$, so its reciprocal-square integral is bounded by a constant times $e^{-r^2/8}r^{p-2}$, tending to zero. Therefore $E_\theta\|X\|^{-2}\to0$, and $R(\theta,\hat\theta)\to p$ from below. Hence

$$
\boxed{\sup_\theta R(\theta,X)=\sup_\theta R(\theta,\hat\theta)=p}.
$$

The second supremum is approached at infinity and need not be attained at a finite parameter.

## ↑ Ancestors (10)

1. [25J](../25j.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
