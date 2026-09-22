<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

Assume a common support, a differentiable likelihood, and dominated differentiation under the integrals. The [score function](../../../../../informant-function.md) $S_\theta=\partial_\theta\log f(X;\theta)$ has mean zero. Its second moment is the [Fisher information](../../../../../fisher-information-matrix.md) $I(\theta)$. If $T$ is unbiased, differentiation of $\mathbb E_\theta T=\theta$ gives $\mathbb E_\theta(TS_\theta)=1$, hence $\operatorname{Cov}_\theta(T,S_\theta)=1$. The [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md) yields

$$
\boxed{\operatorname{Var}_\theta(T)\geq I(\theta)^{-1},}
$$

the [Cramér-Rao lower bound](../../../../../cramer-rao-bound.md), assuming positive finite information.

Equality holds precisely when the centred estimator and score are linearly dependent almost surely. The covariance fixes the factor, giving $S_\theta=I(\theta)(T-\theta)$. If the same unbiased estimator is efficient for every parameter on a regular interval, integrate this identity in $\theta$:

$$
\log f(x;\theta)=A(\theta)T(x)-B(\theta)+C(x),
\qquad A'=I,\quad B'=\theta I.
$$

Exponentiation gives $f(x;\theta)=h(x)\exp(A(\theta)T(x)-B(\theta))$, an [exponential family](../../../../../exponential-family-split.md). This proves [efficient unbiased estimator implies exponential family](../../../../../efficient-unbiased-estimator-implies-exponential-family.md) under the stated common-support regularity, rather than asserting it for nonregular support-dependent models.

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
