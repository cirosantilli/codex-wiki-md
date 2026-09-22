<h1 id="3/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Condition throughout on the training inputs and $x_*$. Interpret $\theta$ here as the fixed [covariance function](../../../../../covariance-function.md) and noise hyperparameters. Assume observation errors $\epsilon_i$ are independent standard [normal random variables](../../../../../gaussian-random-variable.md), independent of the [Gaussian process](../../../../../gaussian-process-split.md) $f$, and write

$$
K_{ij}=k(x_i,x_j),\quad k_*=(k(x_1,x_*),\ldots,k(x_n,x_*))^T,\quad k_{**}=k(x_*,x_*),\quad C=K+\sigma^2I_n.
$$

The independent-error assumption is the standard [Gaussian process regression](../../../../../gaussian-process-regression.md) interpretation of the observation model; the single-observation marginal noise law alone would not specify cross-observation noise correlations. We take $\sigma^2>0$ so that $C$ is a [positive-definite matrix](../../../../../positive-definite-matrix.md). More generally the inverse formulas below apply whenever the indicated noisy [covariance matrices](../../../../../covariance-matrix.md) are invertible.

The [Gaussian process](../../../../../gaussian-process-split.md) prior makes $(f_*,\mathbf f)$ a [Gaussian random vector](../../../../../gaussian-random-vector.md). Adding the independent [Gaussian noise](../../../../../gaussian-noise.md) vector to $\mathbf f$ preserves a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md). Its [mean](../../../../../expected-value-split.md) is zero, its observation [covariance matrix](../../../../../covariance-matrix.md) is $C$, and $\operatorname{Cov}(f_*,y_i)=k(x_*,x_i)$ because the noise is independent of $f_*$. Therefore

$$
\boxed{\begin{pmatrix}f_*\\\mathbf y\end{pmatrix}\biggm|\theta\sim\mathcal N\left(0,\begin{pmatrix}k_{**}&k_*^T\\k_*&C\end{pmatrix}\right)}.
$$

A degenerate latent [variance](../../../../../variance-split.md) is allowed; the displayed [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) then denotes a Gaussian law even if it has no full-dimensional [probability density](../../../../../probability-density.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the advanced topics in statistical machine learning course of the University of Oxford](../../../../split.md)
6. [Advanced topics in statistical machine learning course of the University of Oxford](../../../../../advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics and statistics course of the University of Oxford](../../../../../year-4-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Mathematics and statistics course of the University of Oxford](../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
