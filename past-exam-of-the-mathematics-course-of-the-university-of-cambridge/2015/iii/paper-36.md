# Paper 36

↑ **Parent:** [Iii](../iii.md)

[https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_36.pdf](https://www.maths.cam.ac.uk/postgrad/part-iii/files/pastpapers/2015/paper_36.pdf)

**Table of contents**

- [1](#1)
  - [Solution](#1/solution)
- [2](#2)
  - [Solution](#2/solution)
- [3](#3)
  - [Solution](#3/solution)
- [4](#4)
  - [Solution](#4/solution)

## 1

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="1/solution">Solution</h3>

↑ **Parent:** [1](#1)

Put $p=dP/d\mu$ and $q=dQ/d\mu$. Using natural [logarithms](../../../calculus.md#logarithm), the [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) is

$$
\boxed{K(P,Q)=\int_\Omega p\log\frac pq\,d\mu.}
$$

The integrand is zero where $p=0$, including where both densities vanish, and is $+\infty$ where $p>0=q$. Equivalently, $K(P,Q)=\int\log(dP/dQ)\,dP$ when $P$ is [absolutely continuous with respect to](../../../measure-theory.md#absolute-continuity-of-measures) $Q$, and it is $+\infty$ otherwise. This is a well-defined extended integral: on $p<q$, writing $t=p/q$ gives $-p\log(p/q)=-qt\log t\leq q/e$, so its negative part is integrable.

For [Pinsker's inequality](../../../probability-and-statistics.md#pinsker-s-inequality), an infinite [Kullback-Leibler divergence](../../../probability-and-statistics.md#kullback-leibler-divergence) makes the conclusion immediate. Assume it is finite. Set

$$
A=\{p\geq q\},\qquad a=P(A),\quad b=Q(A),\quad t=a-b.
$$

Since $\int(p-q)\,d\mu=0$, the positive and negative parts of $p-q$ have equal integrals. Thus

$$
\int|p-q|\,d\mu=2t,\qquad t\geq0.
$$

This $t$ is the [total variation distance](../../../probability-and-statistics.md#total-variation-distance) with the convention $\sup_E|P(E)-Q(E)|$.

We first prove the [binary partition bound for relative entropy](../../../probability-and-statistics.md#binary-partition-bound-for-relative-entropy). For any measurable $E$ with $Q(E)>0$, apply [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) to the [convex function](../../../real-analysis.md#convex-function) $u\mapsto u\log u$ under the conditional [probability measure](../../../probability-theory.md#probability-measure) $Q(\cdot\mid E)$. [Absolute continuity of measures](../../../measure-theory.md#absolute-continuity-of-measures) gives

$$
\int_E p\log\frac pq\,d\mu\geq P(E)\log\frac{P(E)}{Q(E)}.
$$

If $P(E)=0$, both sides are zero; if $Q(E)=0$, finiteness forces $P(E)=0$ as well. Apply this bound to $A$ and its complement to obtain

$$
K(P,Q)\geq d(a,b):=a\log\frac ab+(1-a)\log\frac{1-a}{1-b}.
$$

For $0<b<1$, regarding $d(a,b)$ as a [function](../../../function.md) of $a$ gives

$$
d(b,b)=0,\qquad \partial_a d(b,b)=0,\qquad \partial_a^2d(a,b)=\frac1{a(1-a)}\geq4.
$$

Consequently $d(a,b)-2(a-b)^2$ is a [convex function](../../../real-analysis.md#convex-function) and has its minimum zero at $a=b$. By continuity this also holds at $a=0,1$. For $b=0,1$, the finite case has $a=b$ and the remaining cases have infinite divergence. This proves the [Bernoulli relative entropy lower bound](../../../probability-and-statistics.md#bernoulli-relative-entropy-lower-bound) in every case. Combining the bounds yields

$$
K(P,Q)\geq2t^2=\frac12\left(\int|p-q|\,d\mu\right)^2,\qquad\boxed{\int|p-q|\,d\mu\leq\sqrt{2K(P,Q)}.}
$$

For the [Hellinger distance](../../../probability-and-statistics.md#hellinger-distance), retain the unnormalized convention in which

$$
H^2(P,Q)=2-2\int\sqrt{pq}\,d\mu.
$$

The integral is the [Hellinger affinity](../../../probability-and-statistics.md#hellinger-affinity). In the finite-divergence case, $q/p>0$ for $P$-almost every point. Apply $-\log u\geq1-u$ with $u=\sqrt{q/p}$ to get

$$
\begin{aligned}
K(P,Q)&=\int_{\{p>0\}}-2\log\sqrt{q/p}\,p\,d\mu\\
&\geq2\int_{\{p>0\}}(1-\sqrt{q/p})p\,d\mu\\
&=2-2\int\sqrt{pq}\,d\mu=H^2(P,Q).
\end{aligned}
$$

The affinity is finite by [Cauchy-Schwarz inequality](../../../probability-and-statistics.md#cauchy-schwarz-inequality). Mass of $Q$ on $\{p=0\}$ creates no difficulty, since the affinity vanishes there and both [probability measures](../../../probability-theory.md#probability-measure) have mass one. The infinite-divergence case is again immediate. We obtain the [relative entropy bound for the unnormalized Hellinger distance](../../../probability-and-statistics.md#relative-entropy-bound-for-the-unnormalized-hellinger-distance):

$$
\boxed{H(P,Q)\leq\sqrt{K(P,Q)}.}
$$

## 2

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="2/solution">Solution</h3>

↑ **Parent:** [2](#2)

In the [Gaussian white noise model](../../../stochastic-process.md#gaussian-white-noise-model), observe the entire path

$$
\boxed{Y(t)=\int_0^tf(s)\,ds+n^{-1/2}W(t),\qquad0\leq t\leq1,}
$$

where $W$ is standard [Brownian motion](../../../brownian-motion.md) and the deterministic drift belongs to [L2 space](../../../measure-theory.md#l2-space-is-a-hilbert-space) on $[0,1]$. Equivalently, $dY(t)=f(t)\,dt+n^{-1/2}dW(t)$. For every deterministic $h\in L^2[0,1]$, the observed [stochastic integral](../../../stochastic-calculus.md#stochastic-integral) satisfies

$$
Y(h):=\int_0^1h(t)\,dY(t)=\langle h,f\rangle+n^{-1/2}W(h),\qquad \operatorname{Cov}(W(h),W(g))=\langle h,g\rangle.
$$

The noise $W(h)=\int h\,dW$ is an [isonormal Gaussian process](../../../stochastic-process.md#isonormal-gaussian-process). In particular its [variance](../../../variance.md) is $\|h\|_2^2$. [Gaussian white noise](../../../stochastic-process.md#gaussian-white-noise) is interpreted through these integrals, rather than as an ordinary random [function](../../../function.md) with a pointwise value at every time. No smoothness of $f$ is needed.

Here is the [Gaussian maximum bound without independence](../../../probability-theory.md#gaussian-maximum-bound-without-independence). Put $M=\max_{1\leq i\leq N}|g_i|$. It is integrable since it is bounded by $\sum_i|g_i|$. For every $\lambda>0$,

$$
e^{\lambda M}\leq\sum_{i=1}^N\left(e^{\lambda g_i}+e^{-\lambda g_i}\right),\qquad E e^{\lambda M}\leq2N e^{\lambda^2/2}.
$$

The second inequality uses only the [moment-generating function](../../../probability-theory.md#moment-generating-function) of the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution), so [independence](../../../random-variable.md#independent-random-variables) is unnecessary. [Jensen inequality](../../../real-analysis.md#jensen-s-inequality) gives $e^{\lambda EM}\leq E e^{\lambda M}$, hence

$$
EM\leq\frac{\log(2N)}\lambda+\frac\lambda2.
$$

Minimizing at $\lambda=\sqrt{2\log(2N)}$ proves

$$
\boxed{E\max_{1\leq i\leq N}|g_i|\leq\sqrt{2\log(2N)}.}
$$

For the [dyadic partition](../../../real-analysis.md#dyadic-partition), let $I_{J,k}=[k2^{-J},(k+1)2^{-J})$, $0\leq k<2^J$, putting the endpoint $1$ into the final interval. The [Haar scaling functions](../../../fourier-analysis.md#haar-scaling-function)

$$
\phi_{J,k}=2^{J/2}\mathbf1_{I_{J,k}}
$$

form an [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of the space $V_J$ of [functions](../../../function.md) constant on each interval. The [Haar wavelets](../../../fourier-analysis.md#haar-wavelet) can be written as

$$
\psi_{j,k}=2^{j/2}\left(\mathbf1_{I_{j+1,2k}}-\mathbf1_{I_{j+1,2k+1}}\right).
$$

For $J\geq1$, the constant [function](../../../function.md) $\phi_{0,0}=1$ together with $\psi_{j,k}$, $0\leq j<J$, is another [orthonormal basis](../../../linear-algebra.md#orthonormal-basis) of $V_J$. Indeed, each successive level splits a cell's two constants into their sum and difference; the number of basis elements is $1+\sum_{j=0}^{J-1}2^j=2^J$. Thus the [Haar projection](../../../fourier-analysis.md#haar-projection) is the [orthogonal projection](../../../hilbert-space.md#orthogonal-projection)

$$
\begin{aligned}
\Pi_{V_J}f&=\sum_{k=0}^{2^J-1}\langle f,\phi_{J,k}\rangle\phi_{J,k}\\
&=\langle f,1\rangle\,1+\sum_{j=0}^{J-1}\sum_{k=0}^{2^j-1}\langle f,\psi_{j,k}\rangle\psi_{j,k}.
\end{aligned}
$$

On cell $I_{J,k}$ its value is $2^J\int_{I_{J,k}}f(t)\,dt$. The first formula also applies to $J=0$.

Estimate each coefficient by its observed [stochastic integral](../../../stochastic-calculus.md#stochastic-integral):

$$
\widehat\alpha_{J,k}=\int_0^1\phi_{J,k}(t)\,dY(t)=2^{J/2}\left[Y((k+1)2^{-J})-Y(k2^{-J})\right],\qquad\widehat\Pi_{V_J}f=\sum_k\widehat\alpha_{J,k}\phi_{J,k}.
$$

This is the [Haar projection estimator in Gaussian white noise](../../../fourier-analysis.md#haar-projection-estimator-in-gaussian-white-noise). The noise integrals over disjoint intervals form a [Gaussian vector](../../../probability-and-statistics.md#gaussian-random-vector) with zero off-diagonal [covariance](../../../variance.md#covariance). The principle that [uncorrelated jointly Gaussian variables are independent](../../../probability-and-statistics.md#uncorrelated-jointly-normal-variables-are-independent) then makes these coefficients [independent](../../../random-variable.md#independent-random-variables). Therefore

$$
\widehat\alpha_{J,k}=\langle f,\phi_{J,k}\rangle+n^{-1/2}Z_k,\qquad Z_k\overset{\mathrm{iid}}\sim N(0,1).
$$

Taking [expectations](../../../probability-theory.md#expected-value) shows that **$\widehat\Pi_{V_J}f$ is an [unbiased estimator](../../../statistical-modelling.md#unbiased-estimator) of $\Pi_{V_J}f$**, both coefficientwise and pointwise for the stated step-function representatives.

Only one scaling [function](../../../function.md) is nonzero in each cell, so the [supremum norm](../../../functional-analysis.md#supremum-norm) of the error has the exact form

$$
\left\|\widehat\Pi_{V_J}f-\Pi_{V_J}f\right\|_\infty=\sqrt{\frac{2^J}{n}}\max_{0\leq k<2^J}|Z_k|.
$$

The endpoint convention ensures the same identity at $1$. Apply the [Gaussian maximum bound without independence](../../../probability-theory.md#gaussian-maximum-bound-without-independence) with $N=2^J$ to obtain the [supremum norm risk of a Haar projection estimator](../../../fourier-analysis.md#supremum-norm-risk-of-a-haar-projection-estimator):

$$
\boxed{E\left\|\widehat\Pi_{V_J}f-\Pi_{V_J}f\right\|_\infty\leq\sqrt{\frac{2^J}{n}}\sqrt{2\log(2^{J+1})}=\sqrt{\frac{2^J(2J+2)\log2}{n}}.}
$$

The factor $2^{J/2}$ comes from cellwise scaling, while the extra square root of $J+1$ comes from taking the maximum over $2^J$ Gaussian errors.

## 3

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="3/solution">Solution</h3>

↑ **Parent:** [3](#3)

The [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) states that if $X_1,\ldots,X_n$ are [independent random variables](../../../random-variable.md#independent-random-variables) with $a_i\leq X_i\leq b_i$ almost surely, then for $t>0$

$$
P\left(\sum_{i=1}^n(X_i-EX_i)\geq t\right)\leq\exp\left(-\frac{2t^2}{\sum_i(b_i-a_i)^2}\right).
$$

The same bound holds for the lower tail. Consequently the two-sided tail is at most twice this bound. When all ranges have length zero, the sum is deterministic and every positive tail probability is zero.

We construct an [exponential packing of a Hamming cube](../../../coding-theory.md#exponential-packing-of-a-hamming-cube). Choose an [inclusion-maximal separated set](../../../topological-analysis.md#inclusion-maximal-separated-set) $S$ in $\{-1,1\}^n$ with separation at least $r=n/8$ for the [Hamming distance](../../../coding-theory.md#hamming-distance). It exists by a finite greedy procedure: keep adding any vertex at distance at least $r$ from all selected vertices until none remains. By maximality, every vertex is within distance strictly less than $r$ of some member of $S$. This is the principle that [maximal separated sets give covers](../../../topological-analysis.md#maximal-separated-sets-give-covers).

For a uniformly random vertex $U$ and any fixed vertex $s$, the mismatch indicators in different coordinates are [independent](../../../random-variable.md#independent-random-variables) [Bernoulli random variables](../../../discrete-probability-distribution.md#bernoulli-distribution) with success probability $1/2$. Hence $\rho(U,s)$ has the [binomial distribution](../../../discrete-probability-distribution.md#binomial-distribution) with parameters $n,1/2$. The lower-tail [Hoeffding inequality](../../../probability-inequality.md#hoeffding-inequality) gives

$$
P\left(\rho(U,s)\leq\frac n8\right)=P\left(\rho(U,s)-\frac n2\leq-\frac{3n}8\right)\leq e^{-9n/32}.
$$

Thus the [Hoeffding lower-tail bound for Hamming balls](../../../coding-theory.md#hoeffding-lower-tail-bound-for-hamming-balls) shows that every strict-radius ball $B_{<r}(s)$ has at most $2^ne^{-9n/32}$ vertices. Using a strict ball handles noninteger $n/8$ without changing the required separation.

The strict balls centered at $S$ cover the entire [Hamming cube](../../../coding-theory.md#hamming-cube). Counting their union by the sum of their sizes yields

$$
2^n\leq\sum_{s\in S}|B_{<r}(s)|\leq|S|\,2^ne^{-9n/32},\qquad |S|\geq e^{9n/32}\geq e^{n/4}.
$$

Therefore

$$
\boxed{|S|\geq e^{n/4},\qquad\min_{s\ne s'\in S}\rho(s,s')\geq n/8.}
$$

In particular this proves the assertion for every $n\geq8$. Maximality here means that no further vertex can be added; finding a largest [separated set](../../../topological-analysis.md#separated-subset-of-a-metric-space) is unnecessary.

## 4

↑ **Parent:** [Paper 36](paper-36.md)

<h3 id="4/solution">Solution</h3>

↑ **Parent:** [4](#4)

The relevant [fixed coordinate subspace](../../../vector-space.md#fixed-coordinate-subspace) is $\{(u,0):u\in\mathbb R^k\}$. Let $G$ be the first $k$ columns of $X$ and let

$$
D=\frac1nG^TG-I_k.
$$

The [Gaussian empirical Gram matrix](../../../linear-algebra.md#gaussian-empirical-gram-matrix) $G^TG/n$ is the empirical second moment with the known mean zero; no subtraction of an estimated mean is involved. For $\theta=(u,0)$, the ratio under consideration is $|u^TDu|/\|u\|_2^2$. Since $D$ is a real [symmetric matrix](../../../linear-algebra.md#symmetric-matrix), the [finite-dimensional spectral theorem](../../../linear-operator-theory.md#finite-dimensional-spectral-theorem) gives

$$
\sup_{u\ne0}\frac{|u^TDu|}{\|u\|_2^2}=\|D\|_{\mathrm{op}}.
$$

Indeed, diagonalizing $D$ bounds every unit-vector [quadratic form](../../../linear-algebra.md#quadratic-form) by the largest absolute [eigenvalue](../../../linear-operator-theory.md#eigenvalue), and a corresponding unit [eigenvector](../../../linear-operator-theory.md#eigenvector) attains the bound.

We first construct a [unit sphere net from ball covering](../../../topological-analysis.md#unit-sphere-net-from-ball-covering). Enlarge the numerical covering constant, if necessary, to $A_0\geq1$. Cover the [unit ball](../../../functional-analysis.md#unit-ball) in $\mathbb R^k$ with at most $(2A_0/\delta)^k$ balls of radius at most $\delta/2$. For each such ball meeting the [unit sphere](../../../topology.md#unit-sphere), choose a point of the sphere in it and discard the others. These selected points form a [metric net](../../../topological-analysis.md#metric-net) $\mathcal N$ of the [unit sphere](../../../topology.md#unit-sphere) with radius $\delta$: any two points in one covering ball have distance at most $\delta$. This argument ensures that the net points have unit length even if the original covering centers did not.

Take $\delta=1/4$ and put $B=8A_0$, so $|\mathcal N|\leq B^k$. For unit vectors $u,v$ with $\|u-v\|_2\leq\delta$,

$$
|u^TDu-v^TDv|=|(u-v)^TDu+v^TD(u-v)|\leq2\delta\|D\|_{\mathrm{op}}.
$$

Taking a net point for every unit $u$ and then a supremum proves the [quadratic form net bound](../../../topological-analysis.md#quadratic-form-net-bound)

$$
\|D\|_{\mathrm{op}}\leq\frac1{1-2\delta}\max_{v\in\mathcal N}|v^TDv|=2\max_{v\in\mathcal N}|v^TDv|.
$$

It follows that

$$
\{\|D\|_{\mathrm{op}}>1/2\}\subseteq\bigcup_{v\in\mathcal N}\{|v^TDv|>1/4\}.
$$

Fix $v\in\mathcal N$. The rows of $G$ are [independent](../../../random-variable.md#independent-random-variables) vectors of [independent](../../../random-variable.md#independent-random-variables) random variables with the [standard normal distribution](../../../probability-theory.md#standard-normal-distribution), and $\|v\|_2=1$. Their scalar products with $v$ are therefore [independent](../../../random-variable.md#independent-random-variables) $N(0,1)$ variables $g_1,\ldots,g_n$, so

$$
v^TDv=\frac1n\sum_{i=1}^n(g_i^2-1).
$$

Use the supplied [chi-squared concentration inequality](../../../probability-theory.md#chi-squared-concentration-inequality) with $z=n/1024$. Its threshold is

$$
4(\sqrt{nz}+z)=4n\left(\frac1{32}+\frac1{1024}\right)=\frac{33n}{256}<\frac n4.
$$

Consequently $P(|v^TDv|>1/4)\leq2e^{-n/1024}$. The [union bound](../../../probability-inequality.md#boole-s-inequality) gives the stronger fixed-subspace estimate

$$
P(\|D\|_{\mathrm{op}}>1/2)\leq2\exp\left(k\log B-\frac n{1024}\right).
$$

This is [Gaussian Gram matrix concentration on a fixed subspace](../../../linear-algebra.md#gaussian-gram-matrix-concentration-on-a-fixed-subspace).

Since $1\leq k<p$, we have $p\geq2$. Under $n\geq Ck\log p$,

$$
\frac n{1024}-k\log B\geq\left(\frac C{1024}-\frac{\log B}{\log2}\right)k\log p.
$$

Choose the numerical constant $C\geq1024(1+\log B/\log2)$. Then the parenthesis is at least one, so **$C'=1$ is a valid choice**, and

$$
\boxed{P\left(\sup_{\theta\in\mathbb R_k^p,\,\theta\ne0}\left|\frac{\theta^T\widehat\Sigma\theta-\theta^T\theta}{\theta^T\theta}\right|>\frac12\right)\leq2e^{-k\log p}.}
$$

The covering factor is only $B^k$ because the coordinate subspace is fixed. The ambient dimension enters through the assumed sample-size bound.

## ↑ Ancestors (8)

1. [Iii](../iii.md)
2. [2015](../../2015.md)
3. [Past exam of the mathematics course of the University of Cambridge](../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge.md)
4. [Mathematics course of the University of Cambridge](../../../university-of-cambridge.md#mathematics-course-of-the-university-of-cambridge)
5. [Course of the University of Cambridge](../../../university-of-cambridge.md#course-of-the-university-of-cambridge)
6. [University of Cambridge](../../../university-of-cambridge.md)
7. [List of universities](../../../README.md#list-of-universities)
8. [Codex Wiki](../../../README.md)
