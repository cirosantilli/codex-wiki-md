<h1 id="27i/solution">Solution</h1>

↑ **Parent:** [27I](../27i.md)

Write $H_0,H_1$ for the two simple hypotheses, with prior probabilities $\pi_0,\pi_1$ and densities $f_0,f_1$. Under zero-one loss, the posterior expected losses of choosing $H_0$ and $H_1$ are respectively the posterior probabilities of $H_1$ and $H_0$. A [Bayes decision rule](../../../../../bayes-decision-rule.md) therefore chooses $H_1$ if

$$
\pi_1f_1(x)>\pi_0f_0(x),
$$

chooses $H_0$ for the reverse inequality, and may randomize at equality. With positive priors this is a [likelihood-ratio test](../../../../../likelihood-ratio-test.md) with cutoff $k=\pi_0/\pi_1$.

For a test $\phi$, its prior risk is $\pi_0E_0\phi+\pi_1(1-E_1\phi)$. Choose $k$ and boundary randomization so that the [likelihood-ratio test](../../../../../likelihood-ratio-test.md) $\phi_k$ has size $\alpha$, and choose priors with ratio $k$. Equivalence of normal and extensive analyses makes the pointwise posterior minimizer minimize this prior risk over all randomized tests. Thus for any $E_0\phi'\le\alpha$,

$$
\pi_1(E_1\phi_k-E_1\phi')\ge\pi_0(\alpha-E_0\phi')\ge0.
$$

This proves the [Neyman-Pearson lemma](../../../../../neyman-pearson-lemma.md): **a [likelihood-ratio test](../../../../../likelihood-ratio-test.md) of size $\alpha$ has greatest power among tests of size at most $\alpha$**. Such a cutoff and randomization come from a quantile of the [likelihood ratio](../../../../../likelihood-ratio.md) under $H_0$; always reject where $f_0=0<f_1$. Endpoint cutoffs are handled directly or by their limiting rules.

For the remaining assertions use the usual common-support formulation with positive densities. A family has a [monotone likelihood ratio](../../../../../monotone-likelihood-ratio.md) in $T$ if for every $\theta_1>\theta_0$, $f_{\theta_1}(x)/f_{\theta_0}(x)$ is a nondecreasing function $r(T(x))$. A [monotone test](../../../../../monotone-test.md) here is an upper-cutoff test $\phi=\mathbf1_{T>c}+\eta\mathbf1_{T=c}$, $0\le\eta\le1$, including constant tests. It does not mean an arbitrary smoothly increasing randomized rejection function.

Put $D(\theta)=\gamma(\theta)-\gamma'(\theta)$. For a finite cutoff, choose $k>0$ between the values of $r$ below and above $c$, with $k=r(c)$ when the boundary has positive probability. On $T>c$, $\phi-\phi'\ge0$ and $r-k\ge0$; on $T<c$, both are nonpositive. At a boundary with positive mass $r-k=0$. Therefore

$$
D(\theta_1)-kD(\theta_0)=E_{\theta_0}[(r(T)-k)(\phi-\phi')]\ge0.
$$

When there is probability on both sides, finite positive monotone ratios below the cutoff bound those above it away from zero, so $k$ can be positive and finite. A boundary with positive mass instead supplies the positive finite value $r(c)$. If the cutoff yields a constant test on the support, positivity on the common support proves strict propagation directly: a test identically zero cannot have greater power, and for a test identically one any positive-probability nonrejection by the competitor remains positive-probability at the larger parameter. Hence **$D(\theta_0)>0$ implies $D(\theta_1)>0$**.

Let $\theta^*=\inf\{\theta:D(\theta)>0\}$, taking $\theta^*=+\infty$ when this set is empty. Below $\theta^*$ there is no positive difference. Above a finite $\theta^*$ there is a smaller parameter with positive difference, which propagates upward; the same reasoning applies when $\theta^*=-\infty$. Thus

$$
\boxed{\gamma(\theta)\le\gamma'(\theta)\ (\theta<\theta^*),\qquad
\gamma(\theta)\ge\gamma'(\theta)\ (\theta>\theta^*).}
$$

No assertion at $\theta^*$ itself is needed.

For the final request fix any cutoff $a$ and prior density $\pi$. Set $A(x)=\int_{\theta>a}\pi(\theta)f_\theta(x)\,d\theta$ and $B(x)=\int_{\theta\le a}\pi(\theta)f_\theta(x)\,d\theta$. The [posterior odds](../../../../../posterior-odds.md) are $A(x)/B(x)$. If $T(x_2)\ge T(x_1)$, then

$$
A(x_2)B(x_1)-A(x_1)B(x_2)=\int_{\theta>a}\int_{\eta\le a}\pi(\theta)\pi(\eta)
[f_\theta(x_2)f_\eta(x_1)-f_\theta(x_1)f_\eta(x_2)]\,d\eta\,d\theta\ge0.
$$

Every bracket is nonnegative by [monotone likelihood ratio](../../../../../monotone-likelihood-ratio.md). Equal statistics make the bracket zero, so the ratio depends only on $T$. Dividing where the posterior is defined proves **the [posterior odds](../../../../../posterior-odds.md) are nondecreasing in $T$**, with extended values allowed when one posterior mass is zero. This proves that [posterior odds are monotone under a monotone likelihood ratio](../../../../../posterior-odds-are-monotone-under-a-monotone-likelihood-ratio.md) without restricting the prior's shape.

The common positive-support condition is material to the printed strict inequality. Under the broader definition permitting zero densities, take a two-parameter family on $T\in\{0,1,2\}$ with $f_0=(1/3,1/3,1/3)$ and $f_1=(0,0,1)$. Its [likelihood ratio](../../../../../likelihood-ratio.md) $(0,0,3)$ is nondecreasing. The cutoff test rejecting $T\ge1$ has greater power than the test rejecting only $T=2$ at parameter zero, but both have power one at parameter one. Thus the strict assertion needs the usual positivity convention; it is false without it.

## ↑ Ancestors (10)

1. [27I](../27i.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
