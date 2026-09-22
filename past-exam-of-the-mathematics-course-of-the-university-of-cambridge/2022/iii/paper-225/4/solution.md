<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let

$$
C_X\phi_k=\lambda_k\phi_k,
\qquad
C_Y\psi_l=\gamma_l\psi_l,
$$

and define the [functional principal component scores](../../../../../functional-principal-component-score.md)

$$
\xi_{ik}=\langle X_i,\phi_k\rangle,
\qquad
\eta_{il}=\langle Y_i,\psi_l\rangle.
$$

Use empirical centered scores $\widehat\xi_{ik},\widehat\eta_{il}$ from the sample covariance eigenfunctions and form

$$
\widehat c_{kl}
=\frac1n\sum_{i=1}^n\widehat\xi_{ik}\widehat\eta_{il}.
$$

The finite-dimensional statistic is

$$
T_{K,L}
=n\sum_{k=1}^K\sum_{l=1}^L
\frac{\widehat c_{kl}^2}{\widehat\lambda_k\widehat\gamma_l}.
$$

Under $H_0$, $Y=\varepsilon$ is independent of $X$. The population cross-covariances vanish, and

$$
\operatorname{Cov}(\xi_k\eta_l,\xi_{k'}\eta_{l'})
=\lambda_k\gamma_l
\mathbf1_{\{k=k'\}}\mathbf1_{\{l=l'\}}.
$$

The multivariate [central limit theorem](../../../../../central-limit-theorem.md), consistency of the empirical eigenpairs, and [Slutsky theorem](../../../../../slutsky-theorem.md) therefore give

$$
T_{K,L}\xrightarrow d\chi_{KL}^2.
$$

Rejecting above the $(1-\alpha)$ quantile gives an asymptotic level-$\alpha$ test.

Under a fixed alternative, $\mathbb E[\eta_l\xi_k]$ is the $(l,k)$ coordinate of the [cross-covariance operator](../../../../../cross-covariance-operator.md) $C_{YX}=BC_X$, where $B$ is the [Hilbert-Schmidt operator](../../../../../hilbert-schmidt-operator.md) with kernel $\beta$. Thus

$$
\frac{T_{K,L}}n\xrightarrow p
\sum_{k=1}^K\sum_{l=1}^L
\frac{\{\mathbb E(\xi_k\eta_l)\}^2}{\lambda_k\gamma_l}.
$$

The test is consistent whenever this retained block contains a nonzero cross-covariance; fixed truncation can miss alternatives outside the selected principal-component subspaces.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 225](../../paper-225-split.md)
3. [Iii](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
