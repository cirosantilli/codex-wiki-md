<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Construct a [mean-square derivative of a Gaussian process](../../../../../mean-square-derivative-of-a-gaussian-process.md) on the original [probability space](../../../../../probability-space.md) before choosing its [continuous modification](../../../../../continuous-modification.md). The real [covariance function](../../../../../covariance-function.md) satisfies $K(h)=K(-h)$, because [covariance](../../../../../covariance.md) is symmetric. Three-times differentiability implies that $K''$ is continuous everywhere and differentiable at zero. Since $K''$ is an [even function](../../../../../even-function.md),

$$
K'''(0)=0,\qquad K''(h)-K''(0)=o(|h|)\quad(h\to0).
$$

This uses differentiability of $K''$ at zero, not a bound on $K'''$ throughout a neighborhood.

Let $D_hX(t)=(X(t+h)-X(t))/h$ for $h\ne0$. Twice applying the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) to the [covariance function](../../../../../covariance-function.md) gives

$$
\mathbb E[D_hX(t)D_kX(s)]=-\frac1{hk}\int_0^h\int_0^k K''(t-s+u-v)\,dv\,du.
$$

Oriented integrals make this identity valid for negative as well as positive $h,k$. For a fixed $t$, the right side tends to $-K''(0)$ as $h,k\to0$. In particular,

$$
\mathbb E|D_hX(t)-D_kX(t)|^2\longrightarrow0.
$$

By completeness of [L2 space](../../../../../l2-space-is-a-hilbert-space.md), the [mean-square derivative of a Gaussian process](../../../../../mean-square-derivative-of-a-gaussian-process.md)

$$
Y(t)=L^2\!\operatorname{-lim}_{h\to0}D_hX(t)
$$

exists. Finite vectors consisting of values of $X$ and $Y$ have a centered [multivariate normal distribution](../../../../../multivariate-normal-distribution.md): approximate the $Y$ coordinates by difference quotients and use [mean-square convergence](../../../../../convergence-in-l2.md) and [characteristic functions](../../../../../characteristic-function.md). Thus $Y$ is a centered [Gaussian process](../../../../../gaussian-process.md) jointly constructed with $X$, with

$$
\mathbb E[Y(t)Y(s)]=-K''(t-s),\qquad \mathbb E[X(t)Y(s)]=-K'(t-s).
$$

In particular $-K''(0)\geq0$, and $-K''$ is a [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel.md) because it is an actual [covariance function](../../../../../covariance-function.md). Merely constructing an unrelated [Gaussian process](../../../../../gaussian-process.md) with that [covariance function](../../../../../covariance-function.md) would not yet construct a [modification of a stochastic process](../../../../../modification-of-a-stochastic-process.md) of $X$.

The increment [variance](../../../../../variance-split.md) of $Y$ is

$$
\mathbb E|Y(t)-Y(s)|^2=2\bigl(K''(t-s)-K''(0)\bigr).
$$

For small $|t-s|$, differentiability of $K''$ at zero bounds this by $C|t-s|$. For the remaining distances in $[0,1]$, continuity of $K''$ enlarges $C$ to give the same bound. The fourth moment of a centered [normal distribution](../../../../../normal-distribution.md) is three times its [variance](../../../../../variance-split.md) squared, so

$$
\mathbb E|Y(t)-Y(s)|^4=3\bigl(\mathbb E|Y(t)-Y(s)|^2\bigr)^2\leq C_4|t-s|^2.
$$

The one-dimensional [Kolmogorov continuity theorem](../../../../../kolmogorov-continuity-theorem.md) states that $\mathbb E|U(t)-U(s)|^p\leq C|t-s|^{1+\eta}$ with $p,\eta>0$ gives a [continuous modification](../../../../../continuous-modification.md), with sample-path [Hölder continuity](../../../../../holder-condition.md) of every order less than $\eta/p$. Apply it here with $p=4,\eta=1$. We obtain a [continuous modification](../../../../../continuous-modification.md) $\widetilde Y$ on $[0,1]$. On its null exceptional event, set the entire path equal to zero.

Define, on this same [probability space](../../../../../probability-space.md),

$$
\widetilde X(t)=X(0)+\int_0^t\widetilde Y(s)\,ds\qquad(0\leq t\leq1).
$$

The path integral exists because its integrand is a [continuous function](../../../../../continuous-function.md). It agrees in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) with the integral of $Y$: [Riemann sums](../../../../../riemann-sum.md) converge in [L2 space](../../../../../l2-space-is-a-hilbert-space.md) because $Y$ is mean-square continuous; sums of $\widetilde Y$ have the same values almost surely at each finite collection of mesh points and converge pathwise to the integral. These two limits therefore agree almost surely for each fixed $t$. Equivalently, the integral is the [Bochner integral](../../../../../bochner-integral.md) of the [L2 space](../../../../../l2-space-is-a-hilbert-space.md)-valued map $s\mapsto Y(s)$.

To verify the [modification of a stochastic process](../../../../../modification-of-a-stochastic-process.md) property directly, put $A_t=X(t)-X(0)$ and $I_t=\int_0^tY(s)\,ds$. The preceding [covariance](../../../../../covariance.md) identities and the [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) give

$$
\begin{aligned}
\mathbb E A_t^2&=2(K(0)-K(t)),\\
\mathbb E[A_tI_t]&=\int_0^t\bigl[-K'(t-s)-K'(s)\bigr]\,ds=2(K(0)-K(t)),\\
\mathbb E I_t^2&=-\int_0^t\int_0^tK''(s-u)\,ds\,du=2(K(0)-K(t)).
\end{aligned}
$$

Therefore $\mathbb E(A_t-I_t)^2=0$ and $\widetilde X(t)=X(t)$ almost surely for every fixed $t$. This is also the [mean-square fundamental theorem of calculus](../../../../../mean-square-fundamental-theorem-of-calculus.md) in this stationary setting. If a version on all of $\mathbb R$ is desired, retain the original $X(t)$ outside $[0,1]$; equality at every fixed parameter still holds.

The ordinary [fundamental theorem of calculus](../../../../../fundamental-theorem-of-calculus.md) now gives the simultaneous pathwise conclusion

$$
\boxed{\widetilde X\in C^1([0,1])\text{ almost surely},\qquad \widetilde X'(t)=\widetilde Y(t)\quad(0<t<1).}
$$

Thus the requested [differentiable modification of a stationary Gaussian process](../../../../../differentiable-modification-of-a-stationary-gaussian-process.md) exists. Integrability of $K$ is compatible with the hypotheses but is unnecessary for this direct argument. It also avoids any assumption that a third absolute moment of a spectral density follows from three-times differentiability.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
