<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

**The printed assertion is false as a supremum bound uniform over shrinking bandwidths.** The supplied hint proves a pointwise [stochastic order](../../../../../stochastic-order.md) with constants uniform in $x$. Taking the [supremum](../../../../../supremum.md) inside the probability changes the problem: a growing number of spatial windows produces a logarithmic cost. We first establish the valid consequence of the hint, then give a [counterexample](../../../../../counterexample.md) satisfying the printed assumptions.

For $I=I_{x,h}=[x-h,x+h]$, let $p=\mu(I)$, $A_T=\int_0^T\mathbf1_I(X_t)\,dt$ and $N_T=\int_0^T\mathbf1_I(X_t)\sigma(X_t)\,dW_t$. The [Invariant distribution of an Itô diffusion](../../../../../invariant-distribution-of-an-ito-diffusion.md) has a [probability density function](../../../../../probability-density-function.md) bounded above and bounded away from zero on the required compact interval. Choosing $h_0<M/4$ therefore gives constants $c_0,C_0>0$ such that $c_0h\leq p\leq C_0h$, uniformly for $|x|\leq M/2$ and $0<h<h_0$.

For the centered function $f=\mathbf1_I-p$, $\int|f|\,d\mu=2p(1-p)\leq2p$. Outside $[-M,M]$, $f=-p$. The given second-moment estimate and the [Chebyshev inequality](../../../../../chebyshev-inequality.md) yield

$$
\mathbb E(A_T-Tp)^2\leq5C(1+T)p^2,\qquad
\mathbb P(A_T<Tp/2)\leq\frac{20C(1+T)}{T^2}\leq\frac{40C}{T}\quad(T\geq1).
$$

On the event $A_T\geq Tp/2$, the [drift coefficient](../../../../../drift-coefficient.md) contributes an average whose error is at most $Rh^\alpha$, by [Hölder continuity](../../../../../holder-condition.md). The [Itô isometry](../../../../../ito-isometry.md) and [stationarity](../../../../../stationary-process.md) give $\mathbb E N_T^2\leq\|\sigma\|_\infty^2Tp$. Another use of the [Chebyshev inequality](../../../../../chebyshev-inequality.md) proves

$$
\boxed{\sup_{|x|\leq M/2}\mathbb P\left(|\widehat b_T(x,h)-b(x)|>Rh^\alpha+
\frac{z}{\sqrt{Th}}\right)\leq\frac{40C}{T}+\frac{4\|\sigma\|_\infty^2}{c_0z^2}.}
$$

This also accounts for the zero-denominator convention through the first exceptional event. The bound proves **pointwise $Rh^\alpha+O_{\mathbb P}((Th)^{-1/2})$, uniformly in the location's tail probabilities**. It supplies no bound for the probability of a supremum over all locations.

For an explicit [counterexample](../../../../../counterexample.md), take $\sigma\equiv1$ and the bounded [globally Lipschitz function](../../../../../globally-lipschitz-function.md)

$$
b(x)=-\operatorname{sgn}(x)\min\{(|x|-1)_+,1\}.
$$

It has [Lipschitz constant](../../../../../lipschitz-constant.md) $R=1$, exponent $\alpha=1$, and satisfies the inward-drift conditions with $M=2$, $\gamma=2$. The [stochastic differential equation](../../../../../stochastic-differential-equation.md) has a unique [strong solution of a stochastic differential equation](../../../../../strong-solution-of-a-stochastic-differential-equation.md). Its [Invariant distribution of an Itô diffusion](../../../../../invariant-distribution-of-an-ito-diffusion.md) has density

$$
\rho(x)=Z^{-1}\exp\left(2\int_0^x b(y)\,dy\right),\qquad
Z=\int_{\mathbb R}\exp\left(2\int_0^x b(y)\,dy\right)dx<\infty.
$$

The exponent is zero on $[-1,1]$, equals $-(|x|-1)^2$ when $1<|x|<2$, and equals $3-2|x|$ outside $[-2,2]$. This verifies integrability, positivity and a constant density $\rho_0=Z^{-1}$ on the central interval. Start the [Itô diffusion](../../../../../ito-diffusion.md) in this [Invariant distribution of an Itô diffusion](../../../../../invariant-distribution-of-an-ito-diffusion.md) to obtain the required [stationary process](../../../../../stationary-process.md).

Set $h=T^{-1/3}$ and choose $N=\lfloor(4h)^{-1}\rfloor$ windows with centers $x_j=-1/2+(4j-2)h$, $1\leq j\leq N$. Their intervals $I_j=[x_j-h,x_j+h]$ are disjoint and lie in $[-1,1]$, where the [drift](../../../../../drift-coefficient.md) is zero. Write

$$
A_j(t)=\int_0^t\mathbf1_{I_j}(X_s)\,ds,\qquad
M_j(t)=\int_0^t\mathbf1_{I_j}(X_s)\,dW_s,\qquad q=2\rho_0Th.
$$

Then $\widehat b_T(x_j,h)=M_j(T)/A_j(T)$ whenever $A_j(T)>0$. The same occupation bound as above gives $\mathbb E(A_j(T)-q)^2\leq C_1Th^2$ for $T\geq1$. With $\delta=T^{-1/6}$, a [union bound](../../../../../boole-s-inequality.md) and the [Chebyshev inequality](../../../../../chebyshev-inequality.md) imply

$$
\mathbb P\left(\max_{j\leq N}|A_j(T)-q|>\delta q\right)
\leq\frac{C_2N}{T\delta^2}=O(T^{-1/3})\longrightarrow0.
$$

The [quadratic variations](../../../../../quadratic-variation.md) are $\langle M_j\rangle=A_j$, and the cross [quadratic covariations](../../../../../quadratic-covariation.md) vanish since the windows are disjoint. Each clock tends to infinity almost surely: for any fixed window, the occupation estimate at times $2^k$, followed by the [Borel-Cantelli lemmas](../../../../../borel-cantelli-lemmas.md), gives $A_j(2^k)/(2^k\mu(I_j))\to1$. The [Knight theorem for orthogonal martingales](../../../../../knight-theorem-for-orthogonal-martingales.md) therefore represents $M_j(t)=B_j(A_j(t))$ using [independent](../../../../../independent-random-variables.md) standard [Brownian motions](../../../../../brownian-motion-split.md) $B_1,\ldots,B_N$. This theorem is applied to the finite collection for each $T$; no growing-dimensional [central limit theorem](../../../../../central-limit-theorem.md) is being assumed.

On the preceding clock event, compare each time-changed [Brownian motion](../../../../../brownian-motion-split.md) with its value at deterministic time $q$. The [Brownian reflection principle](../../../../../reflection-principle-wiener-process.md) and a [union bound](../../../../../boole-s-inequality.md) show that, for every fixed $\varepsilon>0$,

$$
\mathbb P\left(\max_{j\leq N}\sup_{|s-q|\leq\delta q}
|B_j(s)-B_j(q)|>\varepsilon\sqrt q\right)
\leq8N\exp\left(-\frac{\varepsilon^2}{2\delta}\right)\longrightarrow0.
$$

This bound does not require the [Brownian motions](../../../../../brownian-motion-split.md) to be independent of their clocks. In particular, $\max_j|M_j(T)-B_j(q)|/\sqrt q\to0$ in [probability](../../../../../probability.md). The variables $B_j(q)/\sqrt q$ are [independent](../../../../../independent-random-variables.md) $N(0,1)$ [random variables](../../../../../random-variable-split.md). Their [Gaussian maximum](../../../../../gaussian-maximum.md) exceeds $\sqrt{\log N}$ with probability tending to one: for $r\geq1$, integration of the [normal density](../../../../../normal-density.md) over $[r,r+1/r]$ gives $\mathbb P(|Z|>r)\geq c r^{-1}e^{-r^2/2}$, and hence

$$
\mathbb P\left(\max_{j\leq N}|Z_j|\leq\sqrt{\log N}\right)
\leq\exp\left(-c\frac{\sqrt N}{\sqrt{\log N}}\right)\longrightarrow0.
$$

Since $A_j(T)\leq(1+\delta)q$ on the clock event, it follows that, for some $c_3>0$,

$$
\mathbb P\left(\sqrt{Th}\sup_{|x|\leq1}|\widehat b_T(x,h)-b(x)|
\geq c_3\sqrt{\log(1/h)}\right)\longrightarrow1.
$$

But $\sqrt{Th}\,Rh=1$ for this bandwidth. Thus the error after subtraction of $Rh$ and multiplication by $\sqrt{Th}$ is not [bounded in probability](../../../../../boundedness-in-probability.md), contradicting the printed [stochastic order](../../../../../stochastic-order.md). **The valid pointwise bound above is provable; the uniform shrinking-bandwidth assertion is not.** This [counterexample](../../../../../counterexample.md) shows why a uniform rate needs at least a $\sqrt{\log(1/h)}$ enlargement of the noise scale. If $h$ is instead held fixed and constants may depend on $h$, this counterexample does not contradict that different interpretation.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 209](../../paper-209-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
