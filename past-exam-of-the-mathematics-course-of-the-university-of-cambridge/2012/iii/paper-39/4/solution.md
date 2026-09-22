<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

There is a genuine qualification: **the first printed inequality is valid as a useful general assertion for $0<\eta<1$, but is false for arbitrary $\eta>0$.** Also the displayed [likelihood ratio](../../../../../likelihood-ratio.md) presupposes $P_{f_1}\ll P_{f_0}$. We first prove the intended bound and then give a counterexample to the unrestricted quantifier.

For any [estimator](../../../../../estimator.md) $T$, set $A=\{d(T,f_0)<r_n\}$. By the [triangle inequality](../../../../../triangle-inequality.md), $d(T,f_1)\ge r_n$ on $A$, while $d(T,f_0)\ge r_n$ on $A^c$. Hence

$$
\max_{j=0,1}r_n^{-1}\mathbb E_{f_j}d(T,f_j)
\ge\frac12\{P_{f_0}(A^c)+P_{f_1}(A)\}.
$$

Let $C=\{|Z-1|\le\eta\}$ with $0<\eta<1$. On $C$, $Z\ge1-\eta$. Therefore

$$
P_{f_0}(A^c)+P_{f_1}(A)
\ge (1-\eta)\{P_{f_0}(A^c)+P_{f_0}(A\cap C)\}
\ge(1-\eta)P_{f_0}(C)
\ge(1-\eta)\left(1-\frac{\mathbb E_{f_0}|Z-1|}{\eta}\right).
$$

The last step is [Markov inequality](../../../../../markov-inequality.md). Taking the supremum over the model and then the infimum over [estimators](../../../../../estimator.md) proves the intended [metric two-point risk bound](../../../../../metric-two-point-risk-bound.md). At $\eta=1$ the right side is zero. For $\eta>1$ a negative right side is also harmless, but a positive right side need not be a lower bound.

Here is an explicit counterexample with positive [probability density functions](../../../../../probability-density-function.md) and $n=3$. Let $A_0=[0,1/2)$, $\delta=1/100$, and take the model consisting of

$$
f_0=2(1-\delta)\mathbf1_{A_0}+2\delta\mathbf1_{A_0^c},\qquad
f_1=2\delta\mathbf1_{A_0}+2(1-\delta)\mathbf1_{A_0^c}.
$$

Use the [L2 norm](../../../../../l2-norm.md) [metric](../../../../../metric.md), for which $D=d(f_0,f_1)=2(1-2\delta)$, and take $r_n=D/2$ for every $n$. The majority-half decision selects $f_0$ if at least two observations lie in $A_0$. Each error probability is $p=3\delta^2-2\delta^3=0.000298$, so its maximum normalized [risk function](../../../../../risk-function.md) is $2p=0.000596$. This is also the [likelihood-ratio test](../../../../../likelihood-ratio-test.md), giving $\mathbb E_{f_0}|Z-1|=2(1-2p)$. At $\eta=3/2$ the proposed right side is $1/12-2p/3>0.083$, contradicting the risk of this explicit [estimator](../../../../../estimator.md). Thus the intended range restriction cannot be omitted.

For the second request use the intended [L2 norm](../../../../../l2-norm.md) [metric](../../../../../metric.md) $d(f,g)=(\int_0^1(f-g)^2)^{1/2}$. The PDF defines its square, not the square itself as a [metric](../../../../../metric.md). Put

$$
g=\mathbf1_{[0,1/2)}-\mathbf1_{[1/2,1]},\qquad
f_0=1,\quad f_{1,n}=1+a_ng,\quad a_n=\frac1{8\sqrt n},\quad r_n=\frac1{16\sqrt n}.
$$

Both [probability density functions](../../../../../probability-density-function.md) belong to the model, and $d(f_0,f_{1,n})=a_n=2r_n$. The two-point choice may depend on $n$, because the lower bound is applied separately at each sample size. Under $f_0$, the product [likelihood ratio](../../../../../likelihood-ratio.md) $Z_n=\prod_i(1+a_ng(X_i))$ satisfies

$$
\mathbb E_0Z_n=1,\qquad
\mathbb E_0(Z_n-1)^2=(1+a_n^2)^n-1\le e^{1/64}-1<\frac1{16}.
$$

This is the product [chi-squared divergence](../../../../../chi-squared-divergence.md). By [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), $\mathbb E_0|Z_n-1|<1/4$. With $\eta=1/2$, the proved [metric two-point risk bound](../../../../../metric-two-point-risk-bound.md) has normalized right side greater than $1/8$. Consequently

$$
\boxed{\inf_T\sup_{f\in\mathcal P_\Psi}\sqrt n\,\mathbb E_fd(T,f)\ge\frac1{128}>0.}
$$

The proof works for every $n\ge1$ despite the introductory $n>2$. [Measurability](../../../../../measurability.md) of the functions defining the [probability density functions](../../../../../probability-density-function.md) is understood. This establishes the requested lower bound; it does not assert a matching upper bound over this unrestricted class.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 39](../../paper-39-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
