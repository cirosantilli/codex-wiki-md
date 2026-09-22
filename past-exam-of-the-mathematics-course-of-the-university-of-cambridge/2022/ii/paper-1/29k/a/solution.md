<h1 id="29k/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Continuous differentiability gives the first-order expansion

$$
\Phi(\widehat\theta_n)-\Phi(\theta_0)
=\nabla\Phi(\theta_0)^T(\widehat\theta_n-\theta_0)
+o(\|\widehat\theta_n-\theta_0\|).
$$

The assumed convergence in distribution implies $\sqrt n(\widehat\theta_n-\theta_0)=O_p(1)$, so after multiplication by $\sqrt n$ the remainder is $o_p(1)$. The [Slutsky theorem](../../../../../../slutsky-theorem.md) gives the multivariate [delta method](../../../../../../delta-method.md)

$$
\boxed{\sqrt n\bigl(\Phi(\widehat\theta_n)-\Phi(\theta_0)\bigr)
\xrightarrow d\nabla\Phi(\theta_0)^TZ}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [29K](../../29k.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
