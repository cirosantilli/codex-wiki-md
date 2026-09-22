<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Let $X_i=Y_i-\theta_0$. Under the symmetric continuous [null hypothesis](../../../../../null-hypothesis.md), positive and negative signs have probability $1/2$ and zeros have probability zero. For the [sign test](../../../../../sign-test.md), take $N_+=\sum_i\mathbf1_{\{X_i>0\}}$ and reject for small values: $N_+\sim\operatorname{Bin}(n,1/2)$ under the null. Choose $k$ with $\mathbb P_0(N_+\leq k)\leq\alpha$; randomization at the next value attains exact size if desired. The lower tail is appropriate for $\theta<\theta_0$.

For the [Wilcoxon signed-rank test](../../../../../wilcoxon-signed-rank-test.md), rank $|X_i|$ increasingly and put $W_+=\sum_iR_i\mathbf1_{\{X_i>0\}}$. Continuous observations have no absolute-value ties almost surely. Conditional on the absolute values, the signs are [independent](../../../../../independent-random-variables.md) fair signs because symmetry makes the sign [independent](../../../../../independent-random-variables.md) of magnitude. Hence $W_+$ has the distribution of $\sum_{r=1}^nrB_r$ for [independent](../../../../../independent-random-variables.md) [Bernoulli random variables](../../../../../bernoulli-distribution.md) $B_r$ with parameter $1/2$. Again reject in the lower tail, using this exact subset-sum distribution or a [normal approximation](../../../../../normal-approximation.md). [Independence](../../../../../independent-random-variables.md) gives the requested null moments:

$$
\boxed{\mathbb E_0W_+=\frac12\sum_{r=1}^nr=\frac{n(n+1)}4,\qquad
\operatorname{Var}_0W_+=\frac14\sum_{r=1}^nr^2=\frac{n(n+1)(2n+1)}{24}.}
$$

For a symmetric kernel $h$ of fixed order $m$, a one-sample [U-statistic](../../../../../u-statistic.md) is $U_n=\binom nm^{-1}\sum_{i_1<\cdots<i_m}h(X_{i_1},\ldots,X_{i_m})$. State the [U-statistic central limit theorem](../../../../../u-statistic-central-limit-theorem.md): if $\mathbb Eh^2<\infty$, $\eta=\mathbb Eh$, and $\zeta_1=\operatorname{Var}(\mathbb E[h\mid X_1])>0$, then $\sqrt n(U_n-\eta)\Rightarrow N(0,m^2\zeta_1)$. The nondegeneracy condition is important.

For $h(x,y)=\mathbf1_{\{x+y>0\}}$, its order-two [U-statistic](../../../../../u-statistic.md) satisfies the exact [Wilcoxon signed-rank statistic](../../../../../wilcoxon-signed-rank-statistic.md) identity

$$
W_+=N_++\binom n2U_n.
$$

To prove it, in an unordered pair the sign of the sum is the sign of whichever observation has larger absolute value. Counting the pairs for which a positive observation is larger contributes its rank minus one; its own positive-sign indicator supplies the remaining one.

Write $F_0$ for the distribution function of $X$ under the null. Symmetry gives $\eta=1/2$ and

$$
\mathbb E[h(x,X_2)]-\frac12=1-F_0(-x)-\frac12=F_0(x)-\frac12.
$$

The [probability integral transform](../../../../../probability-integral-transform.md) makes $F_0(X_1)$ uniform on $(0,1)$, so $\zeta_1=1/12$. Therefore $\sqrt n(U_n-1/2)\Rightarrow N(0,1/3)$. The centred $N_+$ is $O_p(\sqrt n)$ and is negligible on the scale $n^{3/2}$ of $W_+$. Combining the exact decomposition and its mean gives

$$
\boxed{\frac{W_+-n(n+1)/4}{\sqrt{n(n+1)(2n+1)/24}}\Rightarrow N(0,1).}
$$

The lower-tail approximate level-$\alpha$ rejection rule compares this standardized statistic with $\Phi^{-1}(\alpha)$; a half-unit continuity correction can refine discrete-tail calculations.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
