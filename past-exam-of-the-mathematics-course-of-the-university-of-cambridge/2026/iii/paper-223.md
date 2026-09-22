# Paper 223

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20223.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2026/III%20Paper%20223.pdf)

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
- [2](#2)
  - [a](#2/a)
    - [Solution](#2/a/solution)
  - [b](#2/b)
    - [Solution](#2/b/solution)
  - [c](#2/c)
    - [Solution](#2/c/solution)
  - [d](#2/d)
    - [Solution](#2/d/solution)
- [3](#3)
  - [a](#3/a)
    - [Solution](#3/a/solution)
  - [b](#3/b)
    - [Solution](#3/b/solution)
  - [c](#3/c)
    - [Solution](#3/c/solution)
  - [d](#3/d)
    - [Solution](#3/d/solution)

## 1

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="1/a">a</h3>

↑ **Parent:** [1](#1)

<h4 id="1/a/solution">Solution</h4>

↑ **Parent:** [A](#1/a)

The [gross-error sensitivity](../../../statistical-inference.md#gross-error-sensitivity) is $\gamma^*(T,F)=\sup_x|\operatorname{IF}(x;T,F)|$. At $N(\theta,1)$, the [influence function of the sample median](../../../statistical-inference.md#influence-function-of-the-sample-median) has magnitude $1/(2\varphi(0))=\sqrt{\pi/2}$, so

$$
\gamma^*(\widehat\theta_{\mathrm{med}})=\sqrt{\frac\pi2}.
$$

For the [Huber location estimator](../../../statistical-inference.md#huber-location-estimator), $\psi_k(u)=\max(-k,\min(u,k))$ and $\mathbb E\psi_k'(Z)=\mathbb P(|Z|\leq k)=2\Phi(k)-1$, giving

$$
\gamma^*(\widehat\theta_{\mathrm{Hub},k})
=\frac{k}{2\Phi(k)-1}.
$$

For the symmetric normal law, the trimmed population mean is $\theta$. Writing $q_\gamma=\Phi^{-1}(1-\gamma)$ in the supplied influence function gives

$$
\boxed{\gamma^*(\widehat\theta_{\mathrm{trim},\gamma})
=\frac{q_\gamma}{1-2\gamma}.}
$$

<h3 id="1/b">b</h3>

↑ **Parent:** [1](#1)

<h4 id="1/b/solution">Solution</h4>

↑ **Parent:** [B](#1/b)

Let replacement tolerance mean the greatest number of observations that can be replaced while the estimator remains bounded. For $n=2m$, a sample with $m$ zeros and $m$ copies of $a$ is within $m$ replacements of both the all-zero sample and its translate by $a$. If an equivariant estimator tolerated $m$ replacements, it would remain within bounded distance of both $T(0^n)$ and $T(0^n)+a$, which is impossible as $a\to\infty$. Thus at most $m-1$ replacements are tolerable.

For $n=2m+1$, a sample with $m$ zeros and $m+1$ copies of $a$ is obtained from the all-zero sample by $m+1$ replacements and from the all-$a$ sample by $m$ replacements. Translation equivariance again forces breakdown by $m+1$ replacements. In both cases the finite-sample [replacement breakdown point](../../../statistical-inference.md#replacement-breakdown-point) is at most

$$
\boxed{\frac1n\left\lfloor\frac{n-1}{2}\right\rfloor.}
$$

<h3 id="1/c">c</h3>

↑ **Parent:** [1](#1)

<h4 id="1/c/solution">Solution</h4>

↑ **Parent:** [C](#1/c)

The sample median attains the equivariant upper bound:

$$
\varepsilon^*(\widehat\theta_{\mathrm{med}})
=\frac1n\left\lfloor\frac{n-1}{2}\right\rfloor.
$$

For the Huber estimator, fewer than half the observations cannot overpower the bounded scores of the uncontaminated majority. Evaluating the estimating equation below $x_{(1)}-k$ or above $x_{(n)}+k$ makes every uncontaminated score have the same sign. A contaminating majority can balance these scores arbitrarily far away, so

$$
\varepsilon^*(\widehat\theta_{\mathrm{Hub},k})
=\frac1n\left\lfloor\frac{n-1}{2}\right\rfloor.
$$

A $\gamma$-trimmed mean remains bounded while at most $\lfloor\gamma n\rfloor$ arbitrary observations are removed by each tail trim; one more arbitrarily large replacement survives. Hence

$$
\boxed{\varepsilon^*(\widehat\theta_{\mathrm{trim},\gamma})
=\frac{\lfloor\gamma n\rfloor}{n}.}
$$

<h3 id="1/d">d</h3>

↑ **Parent:** [1](#1)

<h4 id="1/d/solution">Solution</h4>

↑ **Parent:** [D](#1/d)

If $v_T=\mathbb E[operatorname{IF}(X;T,N(\theta_0,1))^2]$, asymptotic normality gives an asymptotically level-$\alpha$ test that rejects when

$$
\widehat\theta_T>\theta_0+z_{1-\alpha}\sqrt{v_T/n}.
$$

For the median, $v_T=\pi/2$. For Huber,

$$
v_T=\frac{\mathbb E[\min(Z^2,k^2)]}{(2\Phi(k)-1)^2}.
$$

For the trimmed mean, with $q=\Phi^{-1}(1-\gamma)$,

$$
v_T=\mathbb E\left[
\frac{\max(-q,\min(Z,q))^2}{(1-2\gamma)^2}
\right].
$$

These tests have bounded influence functions, so a small contamination proportion has bounded first-order effect on their statistics, asymptotic levels, and powers. Their finite-contamination protection is quantified by the breakdown points in part (c).

## 2

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="2/a">a</h3>

↑ **Parent:** [2](#2)

<h4 id="2/a/solution">Solution</h4>

↑ **Parent:** [A](#2/a)

For residual $r=y_i-x_i^\top\theta$, minimize

$$
\frac{(r-\gamma)^2}{2\sigma}+k|\gamma|
$$

over $\gamma$. [Soft thresholding](../../../probability-and-statistics.md#soft-thresholding) gives $\widehat\gamma=\operatorname{sgn}(r)(|r|-k\sigma)_+$, and the minimized value is

$$
\begin{cases}
r^2/(2\sigma),&|r|\leq k\sigma,\\
k|r|-k^2\sigma/2,&|r|>k\sigma.
\end{cases}
$$

This is $\sigma\rho_k(r/\sigma)$ for the usual [Huber loss](../../../statistical-inference.md#huber-loss). Multiplication by the positive constant $\sigma$ does not change the minimizing $\theta$, proving equivalence.

<h3 id="2/b">b</h3>

↑ **Parent:** [2](#2)

<h4 id="2/b/solution">Solution</h4>

↑ **Parent:** [B](#2/b)

For fixed residual $r=y_i-x_i^\top\theta$, choosing $\gamma_i=0$ costs $r^2$, while choosing $\gamma_i=r$ costs $\ell$. No other nonzero choice improves on $\gamma_i=r$. Thus

$$
\inf_{\gamma_i}\{(r-\gamma_i)^2+\ell\mathbf1_{\{\gamma_i\ne0\}}\}
=\min(r^2,\ell)=\rho_L(r)
$$

with $L=\sqrt\ell$. Summing over observations proves the equivalence.

<h3 id="2/c">c</h3>

↑ **Parent:** [2](#2)

<h4 id="2/c/solution">Solution</h4>

↑ **Parent:** [C](#2/c)

Away from the two nondifferentiable cutoffs, the skipped-mean score is $\psi_L(u)=2u\mathbf1_{\{|u|\leq L\}}$. The estimating equation is therefore

$$
\boxed{\sum_{i=1}^nx_i(y_i-x_i^\top\theta)
\mathbf1_{\{|y_i-x_i^\top\theta|\leq L\}}=0.}
$$

<h3 id="2/d">d</h3>

↑ **Parent:** [2](#2)

<h4 id="2/d/solution">Solution</h4>

↑ **Parent:** [D](#2/d)

Choose $v\in\mathbb R^p$ outside the finitely many hyperplanes $\{v:x_i^\top v=0\}$. Then $x_i^\top v\ne0$ for every $i$. For $\theta_t=tv$, every residual $y_i-tx_i^\top v$ eventually has absolute value greater than $L$. Every indicator in the estimating equation is then zero, so the equation is satisfied for every sufficiently large $t$.

Thus arbitrarily large solutions already exist without contamination. Under the definition in the question, the skipped-mean regression estimator has breakdown point zero. This is a standard pathology of an exactly redescending score when every root is admitted as an estimator.

## 3

↑ **Parent:** [Paper 223](paper-223.md)

<h3 id="3/a">a</h3>

↑ **Parent:** [3](#3)

<h4 id="3/a/solution">Solution</h4>

↑ **Parent:** [A](#3/a)

Randomly partition the observations into $k$ groups of size $m=n/k$, form the group means $\overline X_1,\ldots,\overline X_k$, and define the [median-of-means estimator](../../../statistical-inference.md#median-of-means-estimator) by

$$
\widehat\mu_{\mathrm{MOM}}=\operatorname{median}
(\overline X_1,\ldots,\overline X_k).
$$

Chebyshev gives

$$
\mathbb P\left(|\overline X_j-\mu|>
2\sigma\sqrt{k/n}\right)\leq\frac14.
$$

A binomial tail bound shows that at least half the groups are good with probability at least $1-e^{-k/8}\geq1-\delta$. Therefore

$$
|\widehat\mu_{\mathrm{MOM}}-\mu|
\leq2\sigma\sqrt{\frac kn}
$$

with probability at least $1-\delta$.

<h3 id="3/b">b</h3>

↑ **Parent:** [3](#3)

<h4 id="3/b/solution">Solution</h4>

↑ **Parent:** [B](#3/b)

The analogous statement is false under only a finite-variance assumption. Let $X=0$ with probability $3/4$ and $X=4$ with probability $1/4$. Then $\mu=1$, while the unique population median is zero. With fixed $k$ and group size $n/k\to\infty$, every group median converges in probability to zero, so their mean also converges to zero. Its error from $\mu$ tends to one rather than having order $n^{-1/2}$. Medians inside groups estimate the population median, while means inside groups preserve the population mean.

<h3 id="3/c">c</h3>

↑ **Parent:** [3](#3)

<h4 id="3/c/solution">Solution</h4>

↑ **Parent:** [C](#3/c)

Write $k=2r+1$ and $m=n/k$. The [central limit theorem](../../../convergence-of-random-variables.md#central-limit-theorem) gives jointly

$$
\frac{\sqrt m(\overline X_j-\mu)}\sigma
\Longrightarrow Z_j,
$$

where the $Z_j$ are independent standard normal variables. Hence

$$
\sqrt n(\widehat\mu_{\mathrm{MOM}}-\mu)
\Longrightarrow\sigma\sqrt k,Z_{(r+1)}.
$$

Its limiting cumulative distribution function is

$$
\boxed{\sum_{j=r+1}^k\binom kj
\Phi\left(\frac{x}{\sigma\sqrt k}\right)^j
\left[1-\Phi\left(\frac{x}{\sigma\sqrt k}\right)\right]^{k-j}.}
$$

<h3 id="3/d">d</h3>

↑ **Parent:** [3](#3)

<h4 id="3/d/solution">Solution</h4>

↑ **Parent:** [D](#3/d)

Now both the number of groups and their size equal $\sqrt n$. A group mean is approximately $N(\mu,\sigma^2/\sqrt n)$, whose density at $\mu$ is approximately $n^{1/4}/(\sigma\sqrt{2\pi})$. The [asymptotic distribution of a sample median](../../../statistical-inference.md#asymptotic-distribution-of-a-sample-median) based on $\sqrt n$ such values therefore has variance

$$
\frac1{4\sqrt n,f(\mu)^2}
\sim\frac{\pi\sigma^2}{2n}.
$$

This suggests the conjecture

$$
\sqrt n(\widehat\mu_{\mathrm{MOM}}-\mu)
\Longrightarrow N\left(0,\frac{\pi\sigma^2}{2}\right),
$$

provided a sufficiently uniform central and local limit approximation controls the triangular array.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2026](../../2026.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
