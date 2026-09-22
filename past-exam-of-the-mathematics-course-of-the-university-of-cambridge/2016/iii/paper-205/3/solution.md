<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Fix the normalization

$$
\boxed{\widehat\beta=\widehat\beta_\lambda^L\in\mathop{\arg\min}_{\beta\in\mathbb R^p}\left\{\frac{1}{2n}\|Y-X\beta\|_2^2+\lambda\|\beta\|_1\right\}.}
$$

The [Lasso](../../../../../lasso.md) penalty uses the [L1 norm](../../../../../l1-norm.md). All arguments below apply to every minimizer; uniqueness of the coefficient vector is not assumed.

The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) are the [subgradient optimality condition](../../../../../subgradient-optimality-condition.md)

$$
\boxed{\frac1nX^T(Y-X\widehat\beta)=\lambda z,\qquad z_j=\begin{cases}\operatorname{sgn}(\widehat\beta_j),&\widehat\beta_j\ne0,\\\text{some number in }[-1,1],&\widehat\beta_j=0.\end{cases}}
$$

These conditions are necessary and sufficient because the objective is a [convex function](../../../../../convex-function.md). They use the [subgradient of the absolute value](../../../../../subgradient-of-the-absolute-value.md), coordinate by coordinate.

Put $\delta=\widehat\beta-\beta^0$. Centered columns imply $X^T\mathbf1=0$, so the subtraction of $\bar\varepsilon\mathbf1$ in the model contributes nothing to the score. The [Karush-Kuhn-Tucker conditions](../../../../../karush-kuhn-tucker-conditions.md) become

$$
\frac1nX^TX\delta=\frac1nX^T\varepsilon-\lambda z.
$$

Multiply by $\delta^T$. Since $z^T\widehat\beta=\|\widehat\beta\|_1$ and $z^T\beta^0\leq\|\beta^0\|_1$, this gives the [prediction inequality from Lasso stationarity](../../../../../prediction-inequality-from-lasso-stationarity.md):

$$
\boxed{\frac1n\|X\delta\|_2^2\leq\frac1n\varepsilon^TX\delta+\lambda\|\beta^0\|_1-\lambda\|\widehat\beta\|_1.}
$$

This is the desired version of the [Basic inequality for the Lasso](../../../../../basic-inequality-for-the-lasso.md). Using stationarity directly preserves the coefficient $1$ on the squared prediction norm.

For the [Gaussian score event for the Lasso](../../../../../gaussian-score-event-for-the-lasso.md), write $X_j$ for column $j$. The assumed [Euclidean norm](../../../../../euclidean-norm.md) $\|X_j\|_2=\sqrt n$ and the [multivariate normal distribution](../../../../../multivariate-normal-distribution.md) of $\varepsilon$ give

$$
G_j=\frac{X_j^T\varepsilon}{\sigma\sqrt n}\sim N(0,1).
$$

The $G_j$ may be correlated, which does not affect the [union bound](../../../../../boole-s-inequality.md). Use the following [sharp two-sided Gaussian tail bound](../../../../../sharp-two-sided-gaussian-tail-bound.md), valid for $G$ with the [standard normal distribution](../../../../../standard-normal-distribution.md) and every $t\geq0$:

$$
\mathbb P(|G|>t)=2\{1-\Phi(t)\}\leq e^{-t^2/2}.
$$

For completeness, the difference $h(t)=e^{-t^2/2}-2\{1-\Phi(t)\}$ satisfies $h(0)=0$, $h'(t)=e^{-t^2/2}(\sqrt{2/\pi}-t)$, and $h(t)\to0$ as $t\to\infty$. It first increases and then decreases to zero, so it is nonnegative. This bound avoids introducing an unnecessary factor two.

Here $\Phi$ is the [standard normal distribution function](../../../../../standard-normal-distribution-function.md). With $\lambda=A\sigma\sqrt{\log p/n}$, the [union bound](../../../../../boole-s-inequality.md) yields

$$
\begin{aligned}
\mathbb P(\Omega^c)&\leq\sum_{j=1}^p\mathbb P\left(|G_j|>\frac{c\lambda\sqrt n}{\sigma}\right)\\
&\leq p\exp\left(-\frac{A^2c^2\log p}{2}\right)=p^{-(A^2c^2/2-1)}.
\end{aligned}
$$

Consequently

$$
\boxed{\mathbb P(\Omega)\geq1-p^{-(A^2c^2/2-1)}.}
$$

The score event uses the [supremum norm](../../../../../supremum-norm.md) of $X^T\varepsilon/n$; the centering term still vanishes because $X^T\mathbf1=0$.

We next work deterministically on $\Omega$. Let

$$
Q=\frac1n\|X\delta\|_2^2,\qquad a=\|\delta_S\|_1,\qquad b=\|\delta_N\|_1.
$$

By [Holder inequality](../../../../../holder-inequality.md), $\varepsilon^TX\delta/n\leq c\lambda\|\delta\|_1=c\lambda(a+b)$. Since $\beta^0_N=0$, the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
\|\beta^0\|_1-\|\widehat\beta\|_1=\|\beta^0_S\|_1-\|\beta^0_S+\delta_S\|_1-\|\delta_N\|_1\leq a-b.
$$

Substituting both inequalities into the [Basic inequality for the Lasso](../../../../../basic-inequality-for-the-lasso.md) produces

$$
Q+(1-c)\lambda b\leq(1+c)\lambda a.
$$

Because $Q\geq0$, this also proves the relevant [Lasso cone condition](../../../../../lasso-cone-condition.md), $(1-c)b\leq(1+c)a$. The assumed [Compatibility condition for the Lasso](../../../../../compatibility-condition-for-the-lasso.md) therefore applies to $\delta$:

$$
a\leq\frac{\sqrt s}{\phi}\sqrt Q.
$$

Set $D=(1+c)\lambda\sqrt s/\phi$. Combining these inequalities gives

$$
Q+(1-c)\lambda b\leq D\sqrt Q.
$$

If $Q>0$, discarding the nonnegative $b$ term shows $\sqrt Q\leq D$. If $Q=0$, compatibility gives $a=0$, and the preceding inequality then gives $b=0$. In either case $D\sqrt Q\leq D^2$, so

$$
\boxed{\frac1n\|X(\widehat\beta-\beta^0)\|_2^2+(1-c)\lambda\|\widehat\beta_N\|_1\leq(1+c)^2\lambda^2\frac{s}{\phi^2}.}
$$

**This is a fast prediction bound and an inactive-coordinate error bound on the same event.** It is the [fast-rate Lasso prediction bound under compatibility](../../../../../fast-rate-lasso-prediction-bound-under-compatibility.md).

Finally, the same argument bounds the active-coordinate [L1 norm](../../../../../l1-norm.md) by

$$
\|\widehat\beta_S-\beta^0_S\|_1\leq\frac{\sqrt s}{\phi}\sqrt Q\leq\frac{(1+c)\lambda s}{\phi^2}=M.
$$

If $|\beta_k^0|>M$, then $k\in S$, and $|\widehat\beta_k-\beta_k^0|\leq M<|\beta_k^0|$. When $\beta_k^0>0$ this implies $\widehat\beta_k>0$; when $\beta_k^0<0$ it implies $\widehat\beta_k<0$. Thus the [sign function](../../../../../sign-function.md) obeys

$$
\boxed{\operatorname{sgn}(\widehat\beta_{\lambda,k}^L)=\operatorname{sgn}(\beta_k^0)\quad\text{if }|\beta_k^0|>\frac{(1+c)\lambda s}{\phi^2}.}
$$

This is [Lasso sign recovery under compatibility](../../../../../lasso-sign-recovery-under-compatibility.md). It concerns the sufficiently large nonzero coefficients; it does not assert that every estimated inactive coefficient is zero.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 205](../../paper-205-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
