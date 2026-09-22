<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [M-estimator](../../../../../m-estimator.md) based on an [estimating equation](../../../../../estimating-equation.md) chooses a consistent root of

$$
\frac1n\sum_{i=1}^n\psi(X_i,\widehat\theta)=0.
$$

Its population target $T(F)=\theta_F$ solves $\mathbb E_F\psi(X,\theta_F)=0$. For a scalar parameter, suppose the root is locally unique and

$$
A=-\mathbb E_F[\partial_\theta\psi(X,\theta_F)]\ne0,
\qquad B=\mathbb E_F[\psi(X,\theta_F)^2]<\infty.
$$

For the contaminated distribution $F_\varepsilon=(1-\varepsilon)F+\varepsilon\delta_x$, differentiate its population equation at zero contamination. The [influence function](../../../../../influence-function.md) satisfies

$$
0=\psi(x,\theta_F)-A\operatorname{IF}(x;T,F).
$$

Consequently

$$
\boxed{\operatorname{IF}(x;T,F)=\frac{\psi(x,\theta_F)}{A}.}
$$

The constant of proportionality is independent of $x$. A local expansion of the sample [estimating equation](../../../../../estimating-equation.md) similarly gives

$$
\sqrt n(\widehat\theta-\theta_F)
=A^{-1}\frac1{\sqrt n}\sum_{i=1}^n\psi(X_i,\theta_F)+o_p(1).
$$

The [central limit theorem](../../../../../central-limit-theorem.md) yields [asymptotic normality](../../../../../asymptotic-normality.md) with the [sandwich variance of an M-estimator](../../../../../sandwich-variance-of-an-m-estimator.md)

$$
\boxed{V(\psi,F)=\mathbb E_F[\operatorname{IF}(X;T,F)^2]=\frac B{A^2}.}
$$

Thus the first-order [variance](../../../../../variance-split.md) of the unscaled estimator is $V/n$. For a vector parameter the same differentiation gives $\operatorname{IF}=A^{-1}\psi$ and $V=A^{-1}BA^{-\mathsf T}$, with $A=-\mathbb E\partial_\theta\psi$ and $B=\mathbb E\psi\psi^{\mathsf T}$.

For the location problem, take the target location to be zero and let $Z$ have the standard [normal distribution](../../../../../normal-distribution.md), with density $\phi$ and distribution function $\Phi$. An odd score has $\mathbb E\psi(Z)=0$. For a differentiable score, integration by parts gives

$$
A=\mathbb E\psi'(Z)=\mathbb E[Z\psi(Z)].
$$

The last expression also gives the appropriate derivative of the population equation for bounded monotone scores with jumps, by differentiating the shifted normal density. Assume $A>0$ and put $h=\psi/A$. Then

$$
\mathbb E[Zh(Z)]=1,\qquad |h(x)|\le C,\qquad V=\mathbb E h(Z)^2.
$$

Multiplying a score by a positive constant changes neither its estimator nor this normalized [influence function](../../../../../influence-function.md).

First establish feasibility. The bound implies

$$
1=\mathbb E[Zh(Z)]\le C\mathbb E|Z|=C\sqrt{2/\pi},
$$

so necessarily $C\ge\sqrt{\pi/2}$. For $C>\sqrt{\pi/2}$, let $K>0$ solve

$$
C=\frac K{p_K},\qquad p_K=2\Phi(K)-1.
$$

This solution is unique: the ratio tends to $\sqrt{\pi/2}$ as $K\downarrow0$, tends to infinity as $K\to\infty$, and has positive derivative because

$$
p_K-2K\phi(K)=2\int_0^K\{\phi(z)-\phi(K)\}\,dz>0.
$$

Take the [Huber score](../../../../../huber-score.md) $\psi_K(x)=\max(-K,\min(x,K))$. Its derivative is one on $(-K,K)$ and zero outside, so $A=p_K$. Hence

$$
h_K(x)=\frac{\psi_K(x)}{p_K}
=\max\left(-C,\min\left(\frac{x}{p_K},C\right)\right).
$$

It is odd, nondecreasing, meets the bound, and satisfies $\mathbb E[Zh_K(Z)]=1$.

To prove optimality, put $a=1/p_K$. For each fixed $x$, the minimum of $u^2-2axu$ over $|u|\le C$ is attained by projecting $ax$ onto $[-C,C]$, which is exactly $h_K(x)$. Therefore every competing normalized [influence function](../../../../../influence-function.md) $h$ satisfies

$$
h(x)^2-h_K(x)^2\ge2ax\{h(x)-h_K(x)\}.
$$

Taking [expectations](../../../../../expected-value.md), the right-hand side vanishes because both functions satisfy $\mathbb E[Zh(Z)]=1$. Thus $\mathbb E h^2\ge\mathbb E h_K^2$. This proves the [optimal bounded influence function for normal location](../../../../../optimal-bounded-influence-function-for-normal-location.md), even over the larger class of all bounded normalized functions, and hence over the required odd nondecreasing class. Its minimum [asymptotic variance](../../../../../asymptotic-variance.md) is

$$
\boxed{V_K=
\frac{p_K-2K\phi(K)+K^2(1-p_K)}{p_K^2},
\qquad C=\frac K{p_K}.}
$$

The numerator is $\mathbb E[Z^2\mathbf1_{\{|Z|\le K\}}]+K^2\Pr(|Z|>K)$.

At the included boundary $C=\sqrt{\pi/2}$, equality in the feasibility bound forces $h(x)=C\operatorname{sgn}(x)$ almost everywhere. This is the [influence function of the sample median](../../../../../influence-function-of-the-sample-median.md), with $V=\pi/2$. It is obtained from the rescaled scores $\psi_K/K$ as $K\downarrow0$. **The boundary solution is the sign score, or equivalently the median estimator.** Literal substitution of $K=0$ in the clipped score gives the identically zero function and no identifiable [estimating equation](../../../../../estimating-equation.md); the printed clipped formula therefore requires this limiting interpretation at equality.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 32](../../paper-32-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
