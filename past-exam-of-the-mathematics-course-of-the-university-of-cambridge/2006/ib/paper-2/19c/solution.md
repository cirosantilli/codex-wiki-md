<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

Put $S=\sum_iX_i$, and let $z_{.95}$ be the exact standard-normal 95th percentile. Under parameter $\theta$, $S=n\theta+\sqrt n Z$ with $Z$ standard normal. This distribution can be justified directly: the joint density of the centered observations is proportional to $\exp[-\sum_i(X_i-\theta)^2/2]$. An orthogonal change of coordinates with first row $(1,\ldots,1)/\sqrt n$ has unit absolute Jacobian and preserves the sum of squares. Its density factors into $n$ one-dimensional standard-normal densities, making the first coordinate $Z=(S-n\theta)/\sqrt n$ standard normal.

Consider the test $\phi_*=\boldsymbol1_{\{S>\sqrt n\,z_{.95}\}}$. Its rejection probability is

$$
\Pr_\theta(\phi_*=1)=1-\Phi(z_{.95}-\sqrt n\theta),
$$

increasing in $\theta$. Therefore its maximum rejection probability over the null $\theta\leq0$ is achieved at zero and equals $\alpha=1/20$. This proves it has the required [test size](../../../../../size-of-a-statistical-test.md).

To prove the [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md) property, rather than quote the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md), fix any $\theta_1>0$. The [likelihood ratio](../../../../../likelihood-ratio.md) of the full sample against $\theta=0$ is

$$
\frac{p_{\theta_1}(x)}{p_0(x)}=\exp\left(\theta_1S-\frac{n\theta_1^2}{2}\right),
$$

strictly increasing in $S$. Set $K=\exp(\theta_1\sqrt n z_{.95}-n\theta_1^2/2)$. For any competing possibly randomized test $0\leq\phi\leq1$ with composite-null size at most $\alpha$, we have $\mathbb E_0\phi\leq\alpha=\mathbb E_0\phi_*$. Pointwise,

$$
(\phi_* -\phi)(p_{\theta_1}-Kp_0)\geq0,
$$

because both factors are nonnegative above the threshold and both are nonpositive below it. Integrating gives

$$
\mathbb E_{\theta_1}\phi_*-\mathbb E_{\theta_1}\phi\geq K(\mathbb E_0\phi_*-\mathbb E_0\phi)\geq0.
$$

This comparison proves the likelihood-ratio optimality result needed here in full. Since the same [critical region](../../../../../rejection-region.md) works for every $\theta_1>0$, it proves the [uniformly most powerful test](../../../../../uniformly-most-powerful-test.md) property over the entire alternative.

For $n=9$, the exact [critical region](../../../../../rejection-region.md) and its quoted-table approximation are

$$
\boxed{\sum_{i=1}^9X_i>3z_{.95},\quad\text{equivalently }\overline X>z_{.95}/3\approx0.55.}
$$

Using the supplied rounded percentile $1.65$ gives $\sum X_i>4.95$. The exact cutoff uses $z_{.95}\approx1.644854$ and hence $\overline X>0.548285$; the rounded cutoff is the intended numerical approximation, not a literally exact size-$0.05$ threshold. The Gaussian distribution is continuous, so equality at the cutoff has probability zero and no randomization there is needed.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
