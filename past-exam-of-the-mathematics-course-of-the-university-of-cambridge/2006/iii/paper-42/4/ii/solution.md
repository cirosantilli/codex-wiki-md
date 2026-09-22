<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For $\theta+t\in\mathcal N$, integrating the exponential tilt gives the [moment-generating function](../../../../../../moment-generating-function.md)

$$
\boxed{M_\theta(t)=\mathbb E_\theta e^{t^TY}=\exp\{\kappa(\theta+t)-\kappa(\theta)\}.}
$$

At an interior [natural parameter](../../../../../../natural-parameter-of-an-exponential-family.md) this is finite in a neighbourhood of $t=0$, so [differentiation under the integral sign](../../../../../../differentiation-under-the-integral-sign.md) is justified by the nearby [exponential moments](../../../../../../exponential-moment.md). Differentiating its logarithm once and twice at zero gives

$$
\boxed{\mathbb E_\theta Y=\nabla\kappa(\theta),\qquad \operatorname{Cov}_\theta(Y)=\nabla^2\kappa(\theta).}
$$

Alternatively the [score function](../../../../../../informant-function.md) is $Y-\nabla\kappa(\theta)$; its mean zero and its [covariance matrix](../../../../../../covariance-matrix.md) give the same [exponential-family derivative identities](../../../../../../exponential-family-derivative-identities.md). For any vector $v$, $v^T\nabla^2\kappa(\theta)v=\operatorname{Var}_\theta(v^TY)\geq0$. In a [minimal exponential family](../../../../../../minimal-exponential-family.md) this [variance](../../../../../../variance-split.md) is strictly positive whenever $v\ne0$, proving [strict convexity](../../../../../../strictly-convex-function.md) of the [cumulant function](../../../../../../cumulant-function-of-an-exponential-family.md). For a general [exponential family](../../../../../../exponential-family-split.md) whose [sufficient statistic](../../../../../../sufficient-statistic.md) is $T(X)$, these identities describe the mean and [covariance matrix](../../../../../../covariance-matrix.md) of $T(X)$, rather than necessarily those of $X$ itself.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
