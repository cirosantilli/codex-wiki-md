<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Work in a regular [statistical model](../../../../../statistical-model-split.md), with fixed support, differentiability under the [integral](../../../../../integral.md), and nonsingular [Fisher information](../../../../../fisher-information-matrix.md). Let $U=(U_\psi,U_\lambda)$ be the [score function](../../../../../informant-function.md). The blocks are [orthogonal statistical parameters](../../../../../orthogonal-statistical-parameters.md) at $\theta$ when

$$
\boxed{I_{\psi\lambda}(\theta)
=\mathbb E_\theta[U_\psi U_\lambda^{\mathsf T}]
=-\mathbb E_\theta[\ell_{\psi\lambda}]=0.}
$$

This is global [parameter orthogonality](../../../../../orthogonal-statistical-parameters.md) if it holds throughout the parameter domain; otherwise it is an assertion at a specified point.

For an independent size-$n$ sample, the regular [maximum-likelihood estimator](../../../../../maximum-likelihood-estimator.md) satisfies

$$
\sqrt n\begin{pmatrix}\widehat\psi-\psi\\\widehat\lambda-\lambda\end{pmatrix}
\ \xrightarrow{d}\ N\!\left(0,
\begin{pmatrix}I_{\psi\psi}^{-1}&0\\0&I_{\lambda\lambda}^{-1}\end{pmatrix}\right),
$$

where $I$ is the information in one observation. Thus the fitted blocks are independent to first order in their limiting [normal distribution](../../../../../normal-distribution.md). The efficient information for $\psi$ is generally the [Schur complement](../../../../../schur-complement.md) $I_{\psi\psi}-I_{\psi\lambda}I_{\lambda\lambda}^{-1}I_{\lambda\psi}$; under orthogonality it is just $I_{\psi\psi}$. **Estimating the nuisance block therefore has no first-order [variance](../../../../../variance-split.md) cost for the interest block**, compared with knowing the [nuisance parameter](../../../../../nuisance-parameter.md).

This also reduces local movement of the constrained nuisance fit. If $j=-\ell''$ is the [observed information](../../../../../observed-fisher-information.md), differentiating its nuisance score equation gives

$$
\frac{\partial\widehat\lambda_\psi}{\partial\psi^{\mathsf T}}
=-j_{\lambda\lambda}^{-1}j_{\lambda\psi}.
$$

Under regular independent sampling and orthogonality, $j_{\lambda\lambda}=O_p(n)$ and the centered mixed block is $O_p(\sqrt n)$. Thus this derivative is $O_p(n^{-1/2})$ locally, and an $O_p(n^{-1/2})$ change in $\psi$ changes the nuisance fit by only $O_p(n^{-1})$. Neither exact finite-sample independence nor vanishing observed cross-information follows from expected-information orthogonality.

For the displayed density family, $\lambda$ is scalar and

$$
\ell(\psi,\lambda;y)=\log a(\lambda,y)+\lambda t(y;\psi),\qquad
U_\psi=\lambda\nabla_\psi t(y;\psi).
$$

The [mean-zero score identity](../../../../../mean-zero-score-identity.md) gives $\mathbb E_\theta\nabla_\psi t=0$ for $\lambda\ne0$. But

$$
\ell_{\psi\lambda}=\nabla_\psi t,
$$

so

$$
\boxed{I_{\psi\lambda}=0.}
$$

This is [score factorization implies parameter orthogonality](../../../../../score-factorization-implies-parameter-orthogonality.md). If zero belongs to the parameter domain, the conclusion extends there by continuity of the regular expected derivatives. At zero the density itself has no dependence on $\psi$, so identifiability and nonsingular information for that block must be treated separately.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
