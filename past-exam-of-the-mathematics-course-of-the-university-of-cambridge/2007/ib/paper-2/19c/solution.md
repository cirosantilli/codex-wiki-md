<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) concerns a [simple hypothesis](../../../../../simple-hypothesis.md) with density $f_0$ against a simple alternative with density $f_1$. Allow a randomized test $0\le\varphi\le1$. Choose a threshold $c\ge0$ and, if necessary, randomize on the equality set so that

$$
\varphi_*=1\quad\text{where }f_1>cf_0,\qquad
\varphi_*=0\quad\text{where }f_1<cf_0,\qquad E_0\varphi_*=\alpha.
$$

Then $\varphi_*$ is a [most powerful test](../../../../../most-powerful-test.md) among all tests of size at most $\alpha$. To prove it, let $E_0\varphi\le\alpha$. Pointwise, $(\varphi_*-\varphi)(f_1-cf_0)\ge0$: above threshold both factors are nonnegative; below threshold both are nonpositive; on the threshold their product vanishes. Therefore

$$
E_1\varphi_*-E_1\varphi
\ge c(E_0\varphi_*-E_0\varphi)\ge0.
$$

This proves the lemma, including regions with $f_0=0$, where a positive alternative density must be rejected. It also shows that ties in the [likelihood ratio](../../../../../likelihood-ratio.md) are the only discretionary region when the inequality is strict off the threshold.

For the stated family, $R=|X|$ has the [Gamma distribution](../../../../../gamma-distribution.md) with shape $\theta$ and unit rate. At $\theta=1$ it has the [exponential distribution](../../../../../exponential-distribution.md), and the [likelihood ratio](../../../../../likelihood-ratio.md) for $\theta=2$ against $\theta=1$ is

$$
\frac{f(x\mid2)}{f(x\mid1)}=|x|,
$$

because $\Gamma(1)=\Gamma(2)=1$. The [most powerful test](../../../../../most-powerful-test.md) therefore rejects for large $|X|$. Since $\Pr_1(|X|>c)=e^{-c}$, its exact size-$\alpha$ critical value and rejection rule are

$$
\boxed{c=-\log\alpha,\qquad\text{reject }H_0\text{ if }|X|>-\log\alpha.}
$$

The distribution is [continuous](../../../../../continuous-function.md), so boundary randomization is unnecessary. Under $\theta=2$, [integration by parts](../../../../../integration-by-parts.md) gives the [power function of a statistical test](../../../../../power-function-of-a-statistical-test.md)

$$
\boxed{\Pr_2(|X|>c)=\int_c^\infty r e^{-r}\,dr
=(c+1)e^{-c}=\alpha(1-\log\alpha).}
$$

For every fixed $\theta>1$, the [likelihood ratio](../../../../../likelihood-ratio.md) against the same null is $|x|^{\theta-1}/\Gamma(\theta)$, strictly increasing in $|x|$. The size constraint still selects exactly the same critical value $c=-\log\alpha$, independent of the alternative. The [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md) therefore makes this single test most powerful against each $\theta>1$ separately. Hence **it is uniformly most powerful for the composite alternative $\theta>1$**.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
