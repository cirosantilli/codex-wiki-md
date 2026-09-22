<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let $B$ be the [Hilbert-Schmidt operator](../../../../../hilbert-schmidt-operator.md) with kernel $\beta$, so the [function-on-function linear model](../../../../../function-on-function-linear-model.md) is $Y=BX+\varepsilon$. Independence and centering give $\mathbb E[Y\mid X]=BX$. Let

$$
C_X\phi_j=\lambda_j\phi_j,
\qquad
C_Y\psi_k=\gamma_k\psi_k,
$$

and define the [functional principal component scores](../../../../../functional-principal-component-score.md)

$$
\xi_j=\langle X,\phi_j\rangle,
\qquad
\eta_k=\langle Y,\psi_k\rangle.
$$

The [cross-covariance operator](../../../../../cross-covariance-operator.md) identity $C_{YX}=BC_X$ gives, for every $\lambda_j>0$,

$$
\mathbb E[\eta_k\xi_j]
=\langle C_{YX}\phi_j,\psi_k\rangle
=\lambda_j\langle B\phi_j,\psi_k\rangle.
$$

Since $BX$ is centered, the requested integrated variance is $\mathbb E\lVert BX\rVert^2$. Applying the [Karhunen–Loève expansion](../../../../../karhunen-loeve-expansion.md) to $X$ and the [Parseval identity](../../../../../parseval-identity.md) in the $\psi_k$ basis yields

$$
\begin{aligned}
\int_0^1\operatorname{Var}(\mathbb E[Y(t)\mid X])dt
&=\mathbb E\lVert BX\rVert^2\\
&=\sum_{j:\lambda_j>0}\lambda_j\lVert B\phi_j\rVert^2\\
&=\sum_{j:\lambda_j>0}\sum_{k\geq1}
\frac{\{\mathbb E(\xi_j\eta_k)\}^2}{\lambda_j}.
\end{aligned}
$$

Equivalently, if $\rho_{jk}=\operatorname{Corr}(\xi_j,\eta_k)$, the expression is $\sum_k\gamma_k\sum_{j:\lambda_j>0}\rho_{jk}^2$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 225](../../paper-225-split.md)
3. [Iii](../../split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
