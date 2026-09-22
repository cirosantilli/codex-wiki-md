# Paper 210

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_210.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2016/paper_210.pdf)

**Table of contents**

- [1](#1)
  - [a](#1/a)
    - [Solution](#1/a/solution)
  - [b](#1/b)
    - [Solution](#1/b/solution)
  - [c](#1/c)
    - [Solution](#1/c/solution)
  - [d](#1/d)
    - [Solution](#1/d/solution)
  - [e](#1/e)
    - [Solution](#1/e/solution)
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
  - [e](#2/e)
    - [Solution](#2/e/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)
  - [e](#3/e)
    - [Solution](#3/e/solution)
- [4](#4)
  - [a](#4/a)
    - [Solution](#4/a/solution)
  - [b](#4/b)
    - [Solution](#4/b/solution)
  - [c](#4/c)
    - [Solution](#4/c/solution)
  - [d](#4/d)
    - [Solution](#4/d/solution)
  - [e](#4/e)
    - [Solution](#4/e/solution)

## 1

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

For each ball, the event of landing in $S_j$ is a [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) trial. Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) its [probability](../../../probability-theory.md#probability) is $\varepsilon$. Under the selected alternative $Q_j$, its [probability](../../../probability-theory.md#probability) is $p_1=\pi+(1-\pi)\varepsilon=\varepsilon+\pi(1-\varepsilon)$. The placements are [independent random variables](../../../random-variable.md#independent-random-variables) conditional on that selected index, so the count has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution):

$$
\boxed{c_j\sim\operatorname{Bin}(n,\varepsilon)\text{ under }P_0,\qquad c_j\sim\operatorname{Bin}(n,\varepsilon+\pi(1-\varepsilon))\text{ under }Q_j.}
$$

The second assertion concerns $Q_j$, rather than the unconditional [mixture model](../../../statistical-modelling.md#mixture-model) $P_1$.

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

The [Hoeffding lemma](../../../probability-inequality.md#hoeffding-lemma) for a [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) variable gives $\mathbb E e^{s(B-p)}\leq e^{s^2/8}$. Multiplication of the [moment-generating functions](../../../probability-theory.md#moment-generating-function) of the [independent random variables](../../../random-variable.md#independent-random-variables) gives $\mathbb E e^{s(X-np)}\leq e^{ns^2/8}$. Thus the centered count is a [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution) with variance proxy $n/4$. The [Chernoff bound](../../../probability-inequality.md#chernoff-bound), optimized at $s=4t/n$, gives

$$
\boxed{\mathbb P(X-np>t)\leq e^{-2t^2/n},\qquad t>0.}
$$

The same estimate holds for the lower tail by applying the [Chernoff bound](../../../probability-inequality.md#chernoff-bound) to $-(X-np)$. No [independence](../../../random-variable.md#independent-random-variables) between different bin counts is needed.

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

Put $a=\sqrt{n\log d/2}$ and $b=\sqrt{n\log(1/\delta)/2}$. Use the [scan statistic](../../../statistical-modelling.md#scan-statistic) $C$ and the [statistical hypothesis testing](../../../statistical-modelling.md#statistical-hypothesis-test) rule

$$
\boxed{\psi=\mathbf1_{\{C>n\varepsilon+a+b\}}.}
$$

The [union bound](../../../probability-inequality.md#boole-s-inequality) and the [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) give $P_0(\psi=1)\leq d\exp[-2(a+b)^2/n]\leq\delta$, since $(a+b)^2\geq a^2+b^2$. Conditional on index $j$, accepting the [null hypothesis](../../../statistical-modelling.md#null-hypothesis) implies $c_j\leq n\varepsilon+a+b$. The assumed separation gives $n\pi(1-\varepsilon)>a+2b$, so this threshold lies more than $b$ below the alternative [expected value](../../../probability-theory.md#expected-value) $np_1$. The lower-tail [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) therefore gives $Q_j(\psi=0)\leq\delta$. Averaging the conditional error over the [mixture model](../../../statistical-modelling.md#mixture-model) gives $P_1(\psi=0)\leq\delta$ as well.

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

For $P\ll Q$, the [chi-squared divergence](../../../probability-and-statistics.md#chi-squared-divergence) is $\chi^2(P\Vert Q)=\mathbb E_Q[(dP/dQ-1)^2]$. Write $L_j=dQ_j/dP_0$ for the [likelihood ratios](../../../statistical-modelling.md#likelihood-ratio) of the complete $n$-ball sample. Since $dP_1/dP_0=d^{-1}\sum_jL_j$ and $\mathbb E_0L_j=1$, the [second moment of a mixture likelihood ratio](../../../probability-and-statistics.md#second-moment-of-a-mixture-likelihood-ratio) gives

$$
\boxed{\chi^2(P_1\Vert P_0)=\frac1{d^2}\sum_{j,\ell=1}^d\mathbb E_0[L_jL_\ell]-1.}
$$

If instead $L_j$ denotes a one-ball [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio), its cross moment must be raised to the $n$th power for the full sample, by [independence](../../../random-variable.md#independent-random-variables).

<h3 id="1/e">e</h3>

↑ **Parent:** [1](#1)

<h4 id="1/e/solution">Solution</h4>

↑ **Parent:** [E](#1/e)

Let $a=\pi^2(\varepsilon^{-1}-1)$. From the supplied [second moment of a mixture likelihood ratio](../../../probability-and-statistics.md#second-moment-of-a-mixture-likelihood-ratio), dropping a nonpositive term gives

$$
\chi^2(P_1\Vert P_0)\leq\frac{(1+a)^n}{d}\leq\frac{e^{na}}d\leq16\nu^2.
$$

The last step uses the assumed separation. It has a real square root only when $16\nu^2d\geq1$; otherwise no parameters satisfy it. The [chi-squared testing lower bound](../../../statistical-inference.md#chi-squared-testing-lower-bound) follows from the [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality): $\|P_1-P_0\|_{\mathrm{TV}}\leq\frac12\sqrt{\chi^2(P_1\Vert P_0)}\leq2\nu$. Every [statistical hypothesis testing](../../../statistical-modelling.md#statistical-hypothesis-test) rule has sum of its [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) and [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) at least $1-\|P_1-P_0\|_{\mathrm{TV}}$. Its larger error is at least half the sum, hence

$$
\boxed{\inf_\psi\max\{P_0(\psi=1),P_1(\psi=0)\}\geq\tfrac12-\nu.}
$$

## 2

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

Because the scalar signal and the noise vector are [independent random variables](../../../random-variable.md#independent-random-variables) with [normal distributions](../../../probability-theory.md#normal-distribution), their sum is a [Gaussian random vector](../../../probability-and-statistics.md#gaussian-random-vector). Its [expected value](../../../probability-theory.md#expected-value) is zero, and the [covariance matrix](../../../variance.md#covariance-matrix) is

$$
\boxed{\Sigma_S=I_d+\theta u(S)u(S)^\top,\qquad P_{\theta,S}=N(0,\Sigma_S).}
$$

Thus this is a [rank-one covariance spike](../../../variance.md#rank-one-covariance-spike). Each summand $X_iX_i^\top$ has [expected value](../../../probability-theory.md#expected-value) $\Sigma_S$, so **$\mathbb E\widehat\Sigma=\Sigma_S$**. Here the empirical matrix is an [uncentered empirical second-moment matrix](../../../variance.md#uncentered-empirical-second-moment-matrix); because the population [expected value](../../../probability-theory.md#expected-value) is known to be zero, it is an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) of the [covariance matrix](../../../variance.md#covariance-matrix). The TeX's apparent factorial denominator is a transcription error.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

Use the convention $\mathbb E e^{sX}\leq e^{\sigma^2s^2/2}$ for the centered [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution). Applying the two-sided [Chernoff bound](../../../probability-inequality.md#chernoff-bound) to $X$ gives $\mathbb P(|X|>x)\leq2e^{-x^2/(2\sigma^2)}$. Since $\mathbb E X^2\geq0$, this already supplies the requested bound:

$$
\boxed{\mathbb P(X^2-\mathbb E X^2>t)\leq\min\{1,2e^{-t/(2\sigma^2)}\},\qquad t>0.}
$$

For averages of [independent random variables](../../../random-variable.md#independent-random-variables), the stronger useful statement is that the [centered square of a sub-Gaussian random variable](../../../probability-and-statistics.md#centered-square-of-a-sub-gaussian-random-variable) is a [sub-exponential random variable](../../../probability-and-statistics.md#subexponential-distribution-light-tailed). The [Bernstein bound for independent sub-exponential variables](../../../probability-inequality.md#bernstein-bound-for-independent-sub-exponential-variables) then give $\mathbb P(n^{-1}\sum_i(X_i^2-\mathbb E X_i^2)>t)\leq2\exp[-c n\min\{t^2/\sigma^4,t/\sigma^2\}]$ for a universal positive $c$. These are the concentration theorems used for quadratic [scan statistics](../../../statistical-modelling.md#scan-statistic).

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Put $\ell=\log(d/\delta)$ and $r=\sqrt{\ell/n}\leq1$. Use the [quadratic scan statistic](../../../statistical-modelling.md#quadratic-scan-statistic) $\Lambda$ and reject when $\Lambda>1+4r$. Under the [null hypothesis](../../../statistical-modelling.md#null-hypothesis), each $n u(T)^\top\widehat\Sigma u(T)$ has the [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution) with $n$ degrees of freedom. The [chi-squared concentration inequality](../../../probability-theory.md#chi-squared-concentration-inequality) gives $P_0^{\otimes n}(\Lambda>1+2r+2r^2)\leq d e^{-\ell}=\delta$, by the [union bound](../../../probability-inequality.md#boole-s-inequality). Since $2r+2r^2\leq4r$, the proposed [Type I error](../../../information-theory.md#type-i-and-type-ii-errors) is at most $\delta$.

For the true set $S$, $n u(S)^\top\widehat\Sigma u(S)/(1+\theta)$ has the same [chi-squared distribution](../../../probability-theory.md#chi-squared-distribution). We need a lower-tail bound that remains positive even when $\ell/n$ is close to one. Set $a=e^{-4r}$. The [chi-squared Chernoff lower-tail bound](../../../probability-theory.md#chi-squared-chernoff-lower-tail-bound) gives $P(V\leq na)\leq\exp[-n(a-1-\log a)/2]\leq e^{-nr^2}=e^{-\ell}$: indeed $e^{-4r}-1+4r\geq2r^2$ for $0\leq r\leq1$. To verify this last inequality, its derivative is $4(1-r-e^{-4r})$; the expression in parentheses is strictly concave, starts at zero, and changes sign once, so the minimum occurs at an endpoint, where the inequality holds.

The function $g(r)=(1+4r)e^{4r}-1$ is [convex](../../../real-analysis.md#convex-function) with $g(0)=0$, so $g(r)\leq r g(1)<300r$ on this interval. Consequently $\theta>300r$ implies $(1+\theta)e^{-4r}>1+4r$. Failure to reject then requires $V\leq na$, giving [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) at most $e^{-\ell}\leq\delta$, uniformly in $S$. An explicit, deliberately conservative answer is

$$
\boxed{\psi=\mathbf1_{\{\Lambda>1+4\sqrt{\log(d/\delta)/n}\}},\qquad C=300.}
$$

The sharp constant is unnecessary; the detection scale is $\sqrt{\log(d/\delta)/n}$.

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Define $P_{\theta,n}=d^{-1}\sum_{S\in\mathcal S}P_{\theta,S}^{\otimes n}$. Expanding its [chi-squared divergence](../../../probability-and-statistics.md#chi-squared-divergence) by the [second moment of a mixture likelihood ratio](../../../probability-and-statistics.md#second-moment-of-a-mixture-likelihood-ratio), and using the supplied one-observation cross moment and [independence](../../../random-variable.md#independent-random-variables), gives

$$
\boxed{\chi^2(P_{\theta,n}\Vert P_0^{\otimes n})=\mathbb E_{S,T}\left[\left(1-\theta^2\frac{|S\cap T|^2}{k^2}\right)^{-n/2}\right]-1.}
$$

Here $S,T$ are independent uniform members of the specified family of cyclic intervals. Their overlap $R=|S\cap T|$ does not have the [hypergeometric distribution](../../../discrete-probability-distribution.md#hypergeometric-distribution) of arbitrary uniform $k$-subsets. The family's geometry must be retained.

Let $x=\theta^2R^2/k^2<1/4$. Since $-\log(1-x)\leq x/(1-x)\leq2x$ and $R^2/k^2\leq R/k$, we obtain $(1-x)^{-n/2}\leq e^{nx}\leq e^{n\theta^2R/k}$. Taking the [expected value](../../../probability-theory.md#expected-value) proves the upper bound. The factor $n$ in the last exponent is present in the PDF and missing in the TeX aid.

<h3 id="2/e">e</h3>

↑ **Parent:** [2](#2)

<h4 id="2/e/solution">Solution</h4>

↑ **Parent:** [E](#2/e)

Two independent cyclic intervals intersect with [probability](../../../probability-theory.md#probability) at most $\min\{1,(2k-1)/d\}\leq2k/d$. For $k\leq d/2$, precisely the $2k-1$ starting-point offsets $-(k-1),\ldots,k-1$ can overlap; for larger $k$, the upper bound is automatic. The [cyclic interval overlap bound](../../../statistical-modelling.md#cyclic-interval-overlap-bound) and the preceding [chi-squared divergence](../../../probability-and-statistics.md#chi-squared-divergence) estimate therefore give

$$
\chi^2(P_{\theta,n}\Vert P_0^{\otimes n})\leq\frac{2k}{d}(e^{n\theta^2}-1)\leq2d^{-\varepsilon}(\alpha d)^\varepsilon=2\alpha^\varepsilon.
$$

As in 1(e), the square-root hypothesis is meaningful when $\alpha d\geq1$. The [chi-squared testing lower bound](../../../statistical-inference.md#chi-squared-testing-lower-bound) bounds the [total variation distance](../../../probability-and-statistics.md#total-variation-distance) by $\sqrt{2\alpha^\varepsilon}/2$. The worst individual [Type II error](../../../information-theory.md#type-i-and-type-ii-errors) dominates the error under the uniform [mixture model](../../../statistical-modelling.md#mixture-model). Thus

$$
\boxed{\inf_\psi\max\{P_0^{\otimes n}(\psi=1),\max_{S\in\mathcal S}P_{\theta,S}^{\otimes n}(\psi=0)\}\geq\tfrac12-\nu_{\varepsilon,\alpha},\quad\nu_{\varepsilon,\alpha}=\frac{\sqrt{2\alpha^\varepsilon}}4.}
$$

Taking $\alpha$ small makes this lower bound informative. This argument uses the actual cyclic-interval alternative, without substituting a different family of subsets.

## 3

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Each row of the [oriented incidence matrix](../../../graph.md#oriented-incidence-matrix) records one signed endpoint difference, hence

$$
\boxed{s(\theta)=\|D\theta\|_1.}
$$

Reversing an [edge](../../../graph-theory.md#edge-of-a-graph) changes the sign of its row, and permuting the [edges](../../../graph-theory.md#edge-of-a-graph) permutes rows; neither operation changes the sum of absolute differences. Thus the [graph total variation](../../../inverse-problem.md#graph-total-variation) is independent of the chosen orientation and ordering. If $D\theta=0$, values agree at the endpoints of every [edge](../../../graph-theory.md#edge-of-a-graph). Any two [graph vertices](../../../graph.md#vertex-graph-theory) of a [connected graph](../../../graph.md#connected-graph) are joined by a [graph path](../../../graph-theory.md#path-in-a-graph), so their values agree. Therefore **$\ker D=\operatorname{span}\{\mathbf1\}$**.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

Let $h=\widehat\theta-\theta^*$. The defining minimum for [graph total variation denoising](../../../inverse-problem.md#graph-total-variation-denoising), compared with the feasible value $\theta^*$, gives $n^{-1}\|z-h\|_2^2+\lambda\|D\widehat\theta\|_1\leq n^{-1}\|z\|_2^2+\lambda\|D\theta^*\|_1$. Expand the squared [Euclidean norm](../../../functional-analysis.md#euclidean-norm) and cancel $\|z\|_2^2/n$ to obtain the [basic inequality for a penalized least-squares estimator](../../../statistical-learning.md#basic-inequality-for-a-penalized-least-squares-estimator):

$$
\boxed{\frac{\|h\|_2^2}{n}\leq\frac2n\langle z,h\rangle+\lambda\|D\theta^*\|_1-\lambda\|D\widehat\theta\|_1.}
$$

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Decompose $h=\Pi_1h+D^\dagger Dh$ using the [incidence pseudoinverse decomposition](../../../graph.md#incidence-pseudoinverse-decomposition). The [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality) controls the constant component, and the duality of the $\ell_\infty$ and $\ell_1$ [norms](../../../functional-analysis.md#norm) controls the remaining component:

$$
\langle z,h\rangle\leq\|\Pi_1z\|_2\|h\|_2+\|(D^\dagger)^\top z\|_\infty\|Dh\|_1.
$$

On the stipulated event, the second term contributes at most $\lambda\|Dh\|_1$ after multiplication by $2/n$. The [triangle inequality](../../../topological-analysis.md#triangle-inequality) gives $\|Dh\|_1\leq\|D\widehat\theta\|_1+\|D\theta^*\|_1$, so the negative penalty in the [basic inequality for a penalized least-squares estimator](../../../statistical-learning.md#basic-inequality-for-a-penalized-least-squares-estimator) cancels. We obtain

$$
\boxed{\frac{\|h\|_2^2}{n}\leq2\lambda s(\theta^*)+\frac2n\|\Pi_1z\|_2\|h\|_2}
$$

on an event of [probability](../../../probability-theory.md#probability) at least $1-\delta$.

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

With the usual variance-proxy convention for a [sub-Gaussian random vector](../../../probability-and-statistics.md#sub-gaussian-random-vector), every column inner product is a [sub-Gaussian random variable](../../../probability-and-statistics.md#sub-gaussian-distribution) with proxy at most $\tau^2$. The two-sided [Chernoff bound](../../../probability-inequality.md#chernoff-bound) and [union bound](../../../probability-inequality.md#boole-s-inequality) imply

$$
\boxed{\|A^\top g\|_\infty\leq\tau\sqrt{2\log(2m/\delta)}\leq\sqrt2\tau\bigl(\sqrt{\log(2m)}+\sqrt{\log(1/\delta)}\bigr)}
$$

with [probability](../../../probability-theory.md#probability) at least $1-\delta$. No [independence](../../../random-variable.md#independent-random-variables) between these inner products is required.

**The printed coefficient-one bound is false under this convention.** Take $k=m=1$, $A=[1]$, and $g=\pm\tau$ with equal [probability](../../../probability-theory.md#probability). This [Rademacher random variable](../../../probability-theory.md#rademacher-distribution) has the stipulated variance proxy, but for $\delta=0.99$ the printed threshold is less than $\tau$, whereas $|g|=\tau$ surely. Even a general sub-Gaussian assumption does not imply [Gaussian concentration inequality](../../../stochastic-process.md#gaussian-concentration-inequality) for arbitrary Lipschitz functions. Under the stronger convention $\mathbb E e^{\langle a,g\rangle}\leq e^{\tau^2\|a\|_2^2/4}$, the same [union bound](../../../probability-inequality.md#boole-s-inequality) proves the printed constants. That convention, however, differs from the binomial variance proxy used in 1(b).

<h3 id="3/e">e</h3>

↑ **Parent:** [3](#3)

<h4 id="3/e/solution">Solution</h4>

↑ **Parent:** [E](#3/e)

Let $B_\delta=\sqrt{\log(2m)}+\sqrt{\log(1/\delta)}$. The columns of $D^\dagger/L$ have [Euclidean norm](../../../functional-analysis.md#euclidean-norm) at most one. Under the usual [sub-Gaussian random vector](../../../probability-and-statistics.md#sub-gaussian-random-vector) convention, 3(d) justifies the tuning choice $\lambda=2\sqrt2 L B_\delta/n$, which is independent of $\theta^*$. Also $\|\Pi_1z\|_2=|\langle z,\mathbf1/\sqrt n\rangle|$, so the [Chernoff bound](../../../probability-inequality.md#chernoff-bound) gives $\|\Pi_1z\|_2^2\leq c_\delta=2\log(2/\delta)$ with [probability](../../../probability-theory.md#probability) at least $1-\delta$.

On the intersection of these events, of [probability](../../../probability-theory.md#probability) at least $1-2\delta$, set $a=\|h\|_2/\sqrt n$ and $b=\|\Pi_1z\|_2/\sqrt n$. The weighted [Young inequality](../../../nonlinear-analysis.md#young-s-inequality-for-products) gives $2ab\leq t^2a^2+b^2/t^2$ for $0<t<1$. Applying it to 3(c) and rearranging yields the rigorous bound

$$
\boxed{\frac{\|h\|_2^2}{n}\leq\frac{4\sqrt2\,s(\theta^*)L}{n(1-t^2)}B_\delta+\frac{c_\delta}{nt^2(1-t^2)}.}
$$

If the coefficient-one concentration statement in 3(d) is taken as an extra hypothesis, instead choose $\lambda=2LB_\delta/n$; the identical argument gives precisely the printed coefficient $4$ in the first term. Thus the deterministic argument and its risk rate are sound; its concentration constants depend on correcting or strengthening 3(d).

## 4

↑ **Parent:** [Paper 210](paper-210.md)

<h3 id="4/a">a</h3>

↑ **Parent:** [4](#4)

<h4 id="4/a/solution">Solution</h4>

↑ **Parent:** [A](#4/a)

Write $s_i=1$ on $S$ and $s_i=-1$ on $S^c$, and put $v=s/\sqrt n$ and $w=\mathbf1/\sqrt n$. Because the two groups have equal size, $v,w$ are [orthonormal](../../../linear-algebra.md#orthonormal-set). Let $a=1/2-t/(2\sqrt n)$ and $b=t/(2\sqrt n)$. The [expected value](../../../probability-theory.md#expected-value) of the [adjacency matrix of a graph](../../../graph-theory.md#adjacency-matrix) is $A_0=a\mathbf1\mathbf1^\top+bss^\top-I_n/2$. Consequently

$$
\boxed{A_0+I_n/2=(n/2-t\sqrt n/2)ww^\top+(t\sqrt n/2)vv^\top,\qquad M_0=(t\sqrt n/2)vv^\top.}
$$

Both displayed [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are positive under the stated range of $t$, so the first matrix has [matrix rank](../../../vector-space.md#matrix-rank) two. The other $n-2$ [eigenvalues](../../../linear-operator-theory.md#eigenvalue) are zero. The figure shows the within-group and between-group blocks of this balanced [stochastic block model](../../../statistical-modelling.md#stochastic-block-model); $A_0$ itself has zero diagonal.

<a id="4/a/image-expected-adjacency-blocks-and-the-positive-rank-one-community-signal"></a>
![](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-210-block-expectation.png)

**[Figure 1](#4/a/image-expected-adjacency-blocks-and-the-positive-rank-one-community-signal). Expected adjacency blocks and the positive rank-one community signal**.

<h3 id="4/b">b</h3>

↑ **Parent:** [4](#4)

<h4 id="4/b/solution">Solution</h4>

↑ **Parent:** [B](#4/b)

For a [symmetric matrix](../../../linear-algebra.md#symmetric-matrix) $H$ with simple largest [eigenvalue](../../../linear-operator-theory.md#eigenvalue) and [spectral gap](../../../linear-operator-theory.md#spectral-gap) $\gamma$, the [Davis-Kahan curvature lemma](../../../linear-operator-theory.md#davis-kahan-curvature-lemma) says $\frac\gamma2\|uu^\top-vv^\top\|_F^2\leq\operatorname{tr}(H(vv^\top-uu^\top))$, where $v$ is its leading unit [eigenvector](../../../linear-operator-theory.md#eigenvector). Applying this to a leading [eigenvector](../../../linear-operator-theory.md#eigenvector) $\widehat v$ of $H+W$, the maximal [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) and duality of the [operator norm](../../../continuous-dual-space.md#operator-norm) and [trace norm](../../../functional-analysis.md#trace-norm) give $\|\widehat v\widehat v^\top-vv^\top\|_F\leq2\sqrt2\|W\|_{\mathrm{op}}/\gamma$; the projector difference has [matrix rank](../../../vector-space.md#matrix-rank) at most two. This is a [rank-one eigenprojector perturbation bound](../../../linear-operator-theory.md#rank-one-eigenprojector-perturbation-bound).

Here $W=M-M_0=A-A_0$ has independent centered bounded upper-triangular entries, apart from symmetry. The [spectral norm bound for a centered Bernoulli adjacency matrix](../../../statistical-modelling.md#spectral-norm-bound-for-a-centered-bernoulli-adjacency-matrix) gives $\mathbb E\|W\|_{\mathrm{op}}\leq C_0\sqrt n$. Taking $H=M_0$ and $\gamma=t\sqrt n/2$ therefore gives, **for the largest-eigenvalue estimator**,

$$
\boxed{\mathbb E\|\widehat v\widehat v^\top-vv^\top\|_F\leq\frac{4\sqrt2 C_0}{t}.}
$$

**The printed argmin selects the wrong end of the spectrum.** For a minimizing unit [eigenvector](../../../linear-operator-theory.md#eigenvector) $u$, compare its [Rayleigh quotient](../../../linear-operator-theory.md#rayleigh-quotient) with any unit vector orthogonal to $v$. This yields $\gamma|u^\top v|^2\leq2\|W\|_{\mathrm{op}}$, and hence $\mathbb E|u^\top v|^2\leq4C_0/t$. Its mean projector error is at least $\sqrt2(1-4C_0/t)$, using $\sqrt{1-x}\geq1-x$. Along $t=n^{1/4}$ with sufficiently large even $n$, the printed parameter restriction holds and this lower bound tends to $\sqrt2$, contradicting an error of order $1/t$. Replace argmin by argmax, or negate the entire matrix before minimizing.

<h3 id="4/c">c</h3>

↑ **Parent:** [4](#4)

<h4 id="4/c/solution">Solution</h4>

↑ **Parent:** [C](#4/c)

For partitions, the appropriate [Hamming distance between unlabelled bipartitions](../../../coding-theory.md#hamming-distance-between-unlabelled-bipartitions) is $\Delta(T,S)=\min\{|T\mathbin\triangle S|,|T\mathbin\triangle S^c|\}$. It counts vertices assigned to the wrong group after the better global exchange of the two group names. The printed signed-indicator formula does not implement this exchange: negating a zero-one indicator is not taking its complement. It must be read as this partition distance, or written with the $\pm1$ membership vectors.

Use the corrected leading [eigenvector](../../../linear-operator-theory.md#eigenvector) estimator from 4(b), and orient its sign to minimize $\|\widehat v-\sigma v\|_2$. At every wrongly signed coordinate, this difference has magnitude at least $1/\sqrt n$. Therefore the [sign rounding bound for a unit eigenvector](../../../coding-theory.md#sign-rounding-bound-for-a-unit-eigenvector) gives

$$
\Delta(\widehat S,S)\leq n\min_\sigma\|\widehat v-\sigma v\|_2^2\leq n\|\widehat v\widehat v^\top-vv^\top\|_F^2\leq2n\|\widehat v\widehat v^\top-vv^\top\|_F.
$$

The last inequality uses the projector distance bound $\sqrt2\leq2$. Taking the [expected value](../../../probability-theory.md#expected-value) of this [Frobenius norm](../../../compact-operator.md#frobenius-norm) estimate proves **$\mathbb E\Delta(\widehat S,S)\leq2nc/t$**. The assertion relies on the corrected estimator and partition-distance definition.

<h3 id="4/d">d</h3>

↑ **Parent:** [4](#4)

<h4 id="4/d/solution">Solution</h4>

↑ **Parent:** [D](#4/d)

The [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) of a [product measure](../../../probability-theory.md#product-measure) is the sum of the individual divergences, by expanding the logarithm of the [likelihood ratio](../../../statistical-modelling.md#likelihood-ratio) and taking its [expected value](../../../probability-theory.md#expected-value). Put $q=1/2-t/\sqrt n$ and define $W(S)$ to be the unordered pairs lying within one group, while $C(S)$ is the set of unordered pairs crossing between groups. Then

$$
D_{\mathrm{KL}}(P_S\Vert P_{S'})=\sum_{e\in W(S)\setminus W(S')}D_{\mathrm{KL}}(\operatorname{Ber}(1/2)\Vert\operatorname{Ber}(q))+\sum_{e\in W(S')\setminus W(S)}D_{\mathrm{KL}}(\operatorname{Ber}(q)\Vert\operatorname{Ber}(1/2)).
$$

Thus choosing the printed $\partial S$ to mean $W(S)$ gives its order of the summands. If $\partial S$ denotes the usual [graph cut](../../../graph.md#graph-cut) $C(S)$, their two orders must be interchanged. Each unordered [edge](../../../graph-theory.md#edge-of-a-graph) is counted once.

The inequality $\log x\leq x-1$ gives

$$
\boxed{D_{\mathrm{KL}}(\operatorname{Ber}(p)\Vert\operatorname{Ber}(q))\leq p\left(\frac pq-1\right)+(1-p)\left(\frac{1-p}{1-q}-1\right)=\frac{(p-q)^2}{q(1-q)}.}
$$

Since $1/3<q<1/2$, each changed-edge divergence is at most $9t^2/(2n)$. Summing over at most $n(n-1)/2$ pairs gives $D_{\mathrm{KL}}(P_S\Vert P_{S'})\leq9nt^2/4$. This is the information scale needed for [Fano's inequality](../../../information-theory.md#fano-s-inequality).

<h3 id="4/e">e</h3>

↑ **Parent:** [4](#4)

<h4 id="4/e/solution">Solution</h4>

↑ **Parent:** [E](#4/e)

In natural logarithms, [Fano's inequality](../../../information-theory.md#fano-s-inequality) for a uniform index $J$ among $N$ alternatives states $\mathbb P(\widehat J\ne J)\geq1-(I(J;G)+\log2)/\log N$. The [mutual information](../../../information-theory.md#mutual-information) is at most the average [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) to any fixed reference law. With the supplied packing, nearest-neighbour decoding turns partition error below half the separation into correct decoding. Thus the packing alone proves a bound at radius $n(1/4-\varepsilon/2)$, with the unavoidable $\log2$ term. It does not automatically prove the much larger printed radius.

A [list-decoding Fano inequality](../../../information-theory.md#list-decoding-fano-inequality) supplies the intended near-half error threshold. Assume $0<\varepsilon<1/4$, since otherwise that threshold is nonpositive and its event is automatic. Take a uniform prior on all $N=\binom n{n/2}/2$ unlabelled balanced partitions, and let $r=n(1/2-2\varepsilon)$. A [Hamming ball](../../../coding-theory.md#hamming-ball) of radius less than $r$ around any estimated partition contains at most $B=\sum_{j<r}\binom nj$ such partitions. This follows by selecting the representative closer to the estimated group; each unlabelled partition contributes at most one such representative because $r<n/2$. The [entropy bound for a Hamming ball](../../../coding-theory.md#entropy-bound-for-a-hamming-ball) gives $\log B\leq n h(r/n)$, where $h$ is the [binary entropy function](../../../combinatorics.md#binary-entropy-function) measured in natural logarithms. Its curvature gives $\log2-h(1/2-2\varepsilon)\geq8\varepsilon^2$. Also $\binom n{n/2}\geq2^n/(n+1)$, so

$$
\log(N/B)\geq8\varepsilon^2n-\log(2(n+1)).
$$

Use the all-$1/2$ independent-edge law $P_*$ as a reference. Only the $n^2/4$ crossing pairs differ; the preceding [Bernoulli distribution](../../../discrete-probability-distribution.md#bernoulli-distribution) divergence estimate gives $D_{\mathrm{KL}}(P_S\Vert P_*)\leq nt^2$. Hence $I(J;G)\leq nt^2$. Whenever the denominator is positive, the [list-decoding Fano inequality](../../../information-theory.md#list-decoding-fano-inequality) proves the finite-sample answer

$$
\boxed{\inf_{\widehat S}\max_S P_S\{\Delta(\widehat S,S)\geq r\}\geq1-\frac{nt^2+\log2}{8\varepsilon^2n-\log(2(n+1))}.}
$$

For $4\varepsilon^2n\geq\log(2(n+1))$, this is at least $1-t^2/(4\varepsilon^2)-\log2/(4\varepsilon^2n)$. If in addition $nt^2\geq\log2$, it implies the intended form with $c'=1/2$. This proves the claimed information-theoretic scale with its needed finite-sample qualifications.

**As a uniform finite-sample assertion for every positive $t$, the printed form is false.** At $t=0$ every partition has the same data law, and a uniformly random balanced guess has a positive chance of being correct, giving error strictly below one. Such randomness can also be extracted from the finite graph sample: assign distinct graph outcomes to the finitely many balanced partitions; under the common law every selected outcome has positive [probability](../../../probability-theory.md#probability). The worst error remains strictly below one for sufficiently small positive $t$, by continuity. The printed lower bound tends to one as $t\downarrow0$ for any fixed universal $c'$, which contradicts this. The entropy correction cannot be dropped without an asymptotic or signal-size condition.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2016](../../2016.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
