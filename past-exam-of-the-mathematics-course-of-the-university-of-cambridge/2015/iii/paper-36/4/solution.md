<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The relevant [fixed coordinate subspace](../../../../../fixed-coordinate-subspace.md) is $\{(u,0):u\in\mathbb R^k\}$. Let $G$ be the first $k$ columns of $X$ and let

$$
D=\frac1nG^TG-I_k.
$$

The [Gaussian empirical Gram matrix](../../../../../gaussian-empirical-gram-matrix.md) $G^TG/n$ is the empirical second moment with the known mean zero; no subtraction of an estimated mean is involved. For $\theta=(u,0)$, the ratio under consideration is $|u^TDu|/\|u\|_2^2$. Since $D$ is a real [symmetric matrix](../../../../../symmetric-matrix.md), the [finite-dimensional spectral theorem](../../../../../finite-dimensional-spectral-theorem.md) gives

$$
\sup_{u\ne0}\frac{|u^TDu|}{\|u\|_2^2}=\|D\|_{\mathrm{op}}.
$$

Indeed, diagonalizing $D$ bounds every unit-vector [quadratic form](../../../../../quadratic-form.md) by the largest absolute [eigenvalue](../../../../../eigenvalue.md), and a corresponding unit [eigenvector](../../../../../eigenvector.md) attains the bound.

We first construct a [unit sphere net from ball covering](../../../../../unit-sphere-net-from-ball-covering.md). Enlarge the numerical covering constant, if necessary, to $A_0\geq1$. Cover the [unit ball](../../../../../unit-ball.md) in $\mathbb R^k$ with at most $(2A_0/\delta)^k$ balls of radius at most $\delta/2$. For each such ball meeting the [unit sphere](../../../../../unit-sphere.md), choose a point of the sphere in it and discard the others. These selected points form a [metric net](../../../../../metric-net.md) $\mathcal N$ of the [unit sphere](../../../../../unit-sphere.md) with radius $\delta$: any two points in one covering ball have distance at most $\delta$. This argument ensures that the net points have unit length even if the original covering centers did not.

Take $\delta=1/4$ and put $B=8A_0$, so $|\mathcal N|\leq B^k$. For unit vectors $u,v$ with $\|u-v\|_2\leq\delta$,

$$
|u^TDu-v^TDv|=|(u-v)^TDu+v^TD(u-v)|\leq2\delta\|D\|_{\mathrm{op}}.
$$

Taking a net point for every unit $u$ and then a supremum proves the [quadratic form net bound](../../../../../quadratic-form-net-bound.md)

$$
\|D\|_{\mathrm{op}}\leq\frac1{1-2\delta}\max_{v\in\mathcal N}|v^TDv|=2\max_{v\in\mathcal N}|v^TDv|.
$$

It follows that

$$
\{\|D\|_{\mathrm{op}}>1/2\}\subseteq\bigcup_{v\in\mathcal N}\{|v^TDv|>1/4\}.
$$

Fix $v\in\mathcal N$. The rows of $G$ are [independent](../../../../../independent-random-variables.md) vectors of [independent](../../../../../independent-random-variables.md) random variables with the [standard normal distribution](../../../../../standard-normal-distribution.md), and $\|v\|_2=1$. Their scalar products with $v$ are therefore [independent](../../../../../independent-random-variables.md) $N(0,1)$ variables $g_1,\ldots,g_n$, so

$$
v^TDv=\frac1n\sum_{i=1}^n(g_i^2-1).
$$

Use the supplied [chi-squared concentration inequality](../../../../../chi-squared-concentration-inequality.md) with $z=n/1024$. Its threshold is

$$
4(\sqrt{nz}+z)=4n\left(\frac1{32}+\frac1{1024}\right)=\frac{33n}{256}<\frac n4.
$$

Consequently $P(|v^TDv|>1/4)\leq2e^{-n/1024}$. The [union bound](../../../../../boole-s-inequality.md) gives the stronger fixed-subspace estimate

$$
P(\|D\|_{\mathrm{op}}>1/2)\leq2\exp\left(k\log B-\frac n{1024}\right).
$$

This is [Gaussian Gram matrix concentration on a fixed subspace](../../../../../gaussian-gram-matrix-concentration-on-a-fixed-subspace.md).

Since $1\leq k<p$, we have $p\geq2$. Under $n\geq Ck\log p$,

$$
\frac n{1024}-k\log B\geq\left(\frac C{1024}-\frac{\log B}{\log2}\right)k\log p.
$$

Choose the numerical constant $C\geq1024(1+\log B/\log2)$. Then the parenthesis is at least one, so **$C'=1$ is a valid choice**, and

$$
\boxed{P\left(\sup_{\theta\in\mathbb R_k^p,\,\theta\ne0}\left|\frac{\theta^T\widehat\Sigma\theta-\theta^T\theta}{\theta^T\theta}\right|>\frac12\right)\leq2e^{-k\log p}.}
$$

The covering factor is only $B^k$ because the coordinate subspace is fixed. The ambient dimension enters through the assumed sample-size bound.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
