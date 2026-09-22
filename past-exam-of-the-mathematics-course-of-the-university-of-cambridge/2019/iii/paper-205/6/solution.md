<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The term $\gamma\|\beta\|_2^2/2$ is strictly convex, while the remaining terms are convex, so the [elastic net](../../../../../elastic-net-regularization.md) objective is strictly convex and its minimizer is unique. If two columns of $X$ are identical, swapping their coefficients leaves the objective unchanged. Uniqueness then forces those coefficients to be equal.

The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) are

$$
\frac1nX^T(X\widehat\beta-Y)+\gamma\widehat\beta
+\lambda\widehat z=0,
$$

where

$$
\widehat z_j=
\begin{cases}
\operatorname{sgn}(\widehat\beta_j),&\widehat\beta_j\ne0,\\
[-1,1],&\widehat\beta_j=0.
\end{cases}
$$

Assume $Y=X\beta^0$ and $\operatorname{sgn}(\widehat\beta)=\operatorname{sgn}(\beta^0)=s$. The active equations give

$$
(X_S^TX_S+n\gamma I)\widehat\beta_S
=X_S^TX_S\beta_S^0-n\lambda s_S.
$$

The inactive KKT inequalities become

$$
\boxed{\left\|X_N^TX_S(X_S^TX_S+n\gamma I)^{-1}
\left(\frac\gamma\lambda\beta_S^0+s_S\right)
\right\|_\infty\leq1.}
$$

Conversely, define $\widetilde\beta_N=0$ and

$$
\widetilde\beta_S=(X_S^TX_S+n\gamma I)^{-1}
(X_S^TX_S\beta_S^0-n\lambda s_S).
$$

If the displayed inequality holds and $\operatorname{sgn}(\widetilde\beta_S)=s_S$, the active equations and inactive inequalities together satisfy every KKT condition. Convexity and uniqueness imply $\widetilde\beta=\widehat\beta$, proving sign recovery.

The final sign condition printed in the question omits the factor $n$ before $\lambda$. For the objective as stated, the corrected expression above is required; without that correction, the claimed converse does not follow from the KKT equations.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
