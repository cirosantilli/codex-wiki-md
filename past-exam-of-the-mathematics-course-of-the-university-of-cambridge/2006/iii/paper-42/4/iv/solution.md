<h1 id="4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For independent observations in a [natural exponential family](../../../../../../natural-exponential-family.md), the log [likelihood](../../../../../../likelihood-function.md) is

$$
\ell_n(\theta)=n\{\theta^T\bar Y-\kappa(\theta)\}+\text{constant},\quad U_n(\theta)=n\{\bar Y-\nabla\kappa(\theta)\},\quad j_n(\theta)=n\nabla^2\kappa(\theta).
$$

In a [minimal exponential family](../../../../../../minimal-exponential-family.md) the [Observed Fisher information](../../../../../../observed-fisher-information.md) matrix is positive definite, so the log [likelihood](../../../../../../likelihood-function.md) is [strictly concave](../../../../../../strictly-concave-function.md). Any finite solution of the [likelihood](../../../../../../likelihood-function.md) equation $\nabla\kappa(\widehat\theta)=\bar Y$ is therefore the unique [global maximum](../../../../../../global-maximum.md) [likelihood](../../../../../../likelihood-function.md) estimator. Existence is a separate issue: the observed sufficient-statistic mean must belong to the image of the mean parameter map $\nabla\kappa$.

For a full regular minimal [natural exponential family](../../../../../../natural-exponential-family.md) this image is the interior of the [convex support of an exponential family](../../../../../../convex-support-of-an-exponential-family.md), $C=\overline{\operatorname{conv}(\operatorname{supp}(h\nu))}$. The necessity follows from a supporting hyperplane argument. If a finite parameter had its mean on a boundary face, some nonzero $v$ would satisfy $v^TY\leq b$ [almost surely](../../../../../../almost-sure-convergence.md) and $\mathbb E(v^TY)=b$. Equality of the [expectation](../../../../../../expected-value.md) forces $v^TY=b$ [almost surely](../../../../../../almost-sure-convergence.md). [Exponential tilting](../../../../../../exponential-tilting.md) preserves the base-measure [null sets](../../../../../../null-set.md), so this contradicts minimality.

For sufficiency, let $\bar Y$ be an interior point of $C$. Choose finitely many points $y_1,\ldots,y_m$ of the support whose [convex hull](../../../../../../convex-hull.md) contains a ball about $\bar Y$, say of radius $2\varepsilon$. Such points exist because $\bar Y$ is interior to the [closed convex hull](../../../../../../closed-convex-hull.md); one may approximate the vertices of a small simplex surrounding it by finite [convex combinations](../../../../../../convex-combination.md) of support points. Take support neighbourhoods of radius at most $\varepsilon$ with positive finite base-measure masses $a_j$. These masses can be taken finite by restricting to bounded neighbourhoods and using finiteness of the normalizing integral at any fixed interior parameter. For every vector $\theta$, at least one $j$ has $\theta^T(y_j-\bar Y)\geq2\varepsilon\|\theta\|$. Integrating over that neighbourhood yields

$$
\kappa(\theta)-\theta^T\bar Y\geq\varepsilon\|\theta\|+\min_j\log a_j.
$$

Thus the negative log [likelihood](../../../../../../likelihood-function.md) grows to infinity as $\|\theta\|\to\infty$. At a finite boundary point of the full open [natural parameter space](../../../../../../natural-parameter-space.md), the normalizing integral is infinite, since otherwise that point would itself belong to the full domain. [Fatou's lemma](../../../../../../fatou-s-lemma.md) makes $\kappa(\theta)$ diverge on approach to such a boundary. A [minimizing sequence](../../../../../../minimizing-sequence.md) for $\kappa(\theta)-\theta^T\bar Y$ therefore stays in a bounded subset away from the boundary; it has an interior limit where the minimum is attained. Its [gradient](../../../../../../gradient.md) vanishes, giving the required [likelihood](../../../../../../likelihood-function.md) equation. [Strict convexity](../../../../../../strictly-convex-function.md) gives uniqueness.

Hence, under these full, regular and minimal conventions,

$$
\boxed{\text{a finite unique MLE exists}\ \Longleftrightarrow\ \bar Y\in\operatorname{int}C.}
$$

This is [maximum likelihood existence in a full regular natural exponential family](../../../../../../maximum-likelihood-existence-in-a-full-regular-natural-exponential-family.md). Regularity alone does not make every sample admissible: in a [Bernoulli distribution](../../../../../../bernoulli-distribution.md) an all-zero or all-one sample has its [sample mean](../../../../../../sample-mean.md) on the boundary of $C=[0,1]$, and the canonical maximum is approached only as $\theta\to-\infty$ or $+\infty$. The usual probability parameter then has a boundary maximum in an enlarged model, but no finite canonical maximizer. A regular restriction of the [natural parameter space](../../../../../../natural-parameter-space.md) requires membership in its actual mean-map image, rather than merely in $\operatorname{int}C$. Without minimality, affine redundancies may prevent uniqueness of the canonical parameter even when the fitted [probability distribution](../../../../../../probability-distribution.md) is unique.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
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
