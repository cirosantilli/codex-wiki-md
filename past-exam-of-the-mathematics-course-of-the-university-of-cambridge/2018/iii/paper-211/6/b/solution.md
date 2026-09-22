<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $\theta_t$ and $\eta_t$ be the [predictable](../../../../../../predictable-process.md) holdings of the [stock](../../../../../../stock.md) and the [bank account](../../../../../../bank-account.md). With no [consumption](../../../../../../consumption.md), the [self-financing portfolio](../../../../../../self-financing-portfolio.md) has $X=\theta S+\eta B$ and $dX=\theta dS+\eta dB$. The [Itô product rule](../../../../../../ito-product-rule.md), together with the dynamics from part (a), gives

$$
\begin{aligned}
d(X_tY_t)
&=\bigl(Y_t\theta_tS_t\mu_t+Y_t\eta_tB_tr_t-r_tX_tY_t-Y_t\theta_tS_t\sigma_t\lambda_t\bigr)dt\\
&\quad+Y_t(\theta_tS_t\sigma_t-X_t\lambda_t)\,dW_t\\
&=Y_t(\theta_tS_t\sigma_t-X_t\lambda_t)\,dW_t.
\end{aligned}
$$

The [drift](../../../../../../drift-coefficient.md) vanishes because $X=\theta S+\eta B$ and $\sigma\lambda=\mu-r$. Thus $XY$ is a [local martingale](../../../../../../local-martingale.md). It is nonnegative by the assumed nonnegative wealth and strict positivity of $Y$, and hence

$$
\boxed{XY\ \text{is a supermartingale}.}
$$

For example, this last fact follows directly from [Conditional Fatou lemma](../../../../../../conditional-fatou-lemma.md) applied to a [localizing sequence](../../../../../../localizing-sequence.md); the initial capital is assumed finite. As usual, holdings must be integrable against the asset [semimartingales](../../../../../../semimartingale.md) for the [self-financing portfolio](../../../../../../self-financing-portfolio.md) equation to be defined.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
