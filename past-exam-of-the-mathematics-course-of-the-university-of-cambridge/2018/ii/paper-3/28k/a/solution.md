<h1 id="28k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For one observation with density $f(x,\theta)$, the [Fisher information matrix](../../../../../../fisher-information-matrix.md) at $\theta_0$ is

$$
I(\theta_0)
=\mathbb E_{\theta_0}\!\left[
\nabla_\theta\log f(X,\theta_0)
\nabla_\theta\log f(X,\theta_0)^T
\right].
$$

Here

$$
\log f(x,\theta)=\text{constant}-\frac12\lVert x-\theta\rVert^2,
\qquad
\nabla_\theta\log f(x,\theta)=x-\theta.
$$

Since $\operatorname{Cov}_{\theta_0}(X)=I_p$, the [Fisher information of a multivariate normal location model](../../../../../../fisher-information-of-a-multivariate-normal-location-model.md) is

$$
\boxed{I(\theta_0)=I_p.}
$$

The information in the full independent sample is $nI_p$ by [Tensorization of Fisher information](../../../../../../tensorization-of-fisher-information.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28K](../../28k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
