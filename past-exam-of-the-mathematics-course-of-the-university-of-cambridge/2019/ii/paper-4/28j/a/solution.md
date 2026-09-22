<h1 id="28j/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For observations $x=(x_1,\ldots,x_n)$, the [likelihood function](../../../../../../likelihood-function.md) is

$$
L(\theta;x)=\prod_{i=1}^nf(x_i;\theta).
$$

A [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) is any measurable choice

$$
\boxed{\widehat\theta_{\mathrm{MLE}}(x)\in\operatorname*{argmax}_{\theta\in\Theta}L(\theta;x).}
$$

For one observation in a regular scalar model, the [score function](../../../../../../informant-function.md) is

$$
S_\theta(X)=\frac{\partial}{\partial\theta}\log f(X;\theta),
$$

and the [Fisher information](../../../../../../fisher-information-matrix.md) is

$$
\boxed{I(\theta)=\mathbb E_\theta[S_\theta(X)^2]
=-\mathbb E_\theta\left[\frac{\partial^2}{\partial\theta^2}\log f(X;\theta)\right],}
$$

where the second identity requires the usual differentiation-under-the-integral regularity. For $n$ independent observations, [Tensorization of Fisher information](../../../../../../tensorization-of-fisher-information.md) gives $I_n(\theta)=nI(\theta)$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [28J](../../28j.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
