<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For deterministic [step functions](../../../../../../step-function.md), define directly from [Brownian motion](../../../../../../brownian-motion-split.md) increments

$$
Z_t=\sum_{i=1}^n f_i\bigl(B_{t\wedge s_i}-B_{t\wedge s_{i-1}}\bigr),
$$

with $s_0$ the left endpoint of the first interval and $f=0$ outside the listed intervals. The printed endpoint list omits $s_0$; the intended convention is $0\leq s_0<s_1<\cdots<s_n$, usually $s_0=0$.

Given finitely many observation times, refine the deterministic [partition of an interval](../../../../../../partition-of-an-interval.md) to include all observation times and all $s_i$. Every $Z_{t_j}$ is a linear combination of the same finite family of [independent](../../../../../../independent-random-variables.md) centered [normal](../../../../../../normal-distribution.md) [Brownian motion](../../../../../../brownian-motion-split.md) increments. Thus every linear combination of $(Z_{t_1},\ldots,Z_{t_m})$ is [normal](../../../../../../normal-distribution.md), including possibly a degenerate constant: $Z$ is a [Gaussian process](../../../../../../gaussian-process.md). By [independence](../../../../../../independent-random-variables.md), only increments in the common interval $[0,s\wedge t]$ contribute to the [covariance](../../../../../../covariance.md), giving

$$
\boxed{\mathbb EZ_t=0,\qquad C(s,t)=\int_0^{s\wedge t}f(u)^2\,du.}
$$

The same calculation for two [step functions](../../../../../../step-function.md) $f,g$ proves, rather than assumes, the [Itô isometry](../../../../../../ito-isometry.md)

$$
\mathbb E|Z_t(f)-Z_t(g)|^2=\int_0^t|f(u)-g(u)|^2\,du.
$$

For $f\in L^2(\mathbb R_+)$, choose deterministic [step functions](../../../../../../step-function.md) $f_n\to f$ in the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md). This identity makes $Z_t(f_n)$ a [Cauchy sequence](../../../../../../cauchy-sequence.md) in the [L2 space](../../../../../../l2-space-is-a-hilbert-space.md); the [Riesz-Fischer theorem](../../../../../../riesz-fischer-theorem.md) defines $Z_t(f)$ by [mean-square convergence](../../../../../../convergence-in-l2.md), independently of the approximation. The [covariance](../../../../../../covariance.md) formula passes to the limit by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md). For finitely many times and coefficients $a_j$, the [characteristic functions](../../../../../../characteristic-function.md) converge to

$$
\mathbb E\exp\!\left(i\sum_j a_jZ_{t_j}(f)\right)
=\exp\!\left(-\frac12\sum_{j,k}a_ja_k\int_0^{t_j\wedge t_k}f(u)^2\,du\right),
$$

so the extension remains a [Gaussian process](../../../../../../gaussian-process.md).

For completeness, the construction has a continuous version. Each approximating $Z(f_n)$ is a [martingale](../../../../../../martingale-split.md), directly by the centered [independent increments](../../../../../../independent-increments.md) of [Brownian motion](../../../../../../brownian-motion-split.md); the [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) gives

$$
\mathbb E\sup_{u\leq T}|Z_u(f_n)-Z_u(f_m)|^2\leq4\|f_n-f_m\|_{L^2(\mathbb R_+)}^2.
$$

To prove the inequality used here without assuming [Itô integral](../../../../../../ito-integral.md) properties, a continuous [martingale](../../../../../../martingale-split.md) $N$ satisfies $\lambda\mathbb P(N^*_T\geq\lambda)\leq\mathbb E(|N_T|\mathbf1_{\{N^*_T\geq\lambda\}})$, by conditioning at the first crossing on finite deterministic grids and then using continuity; integrating in $\lambda$ and using the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) yields $\|N^*_T\|_2\leq2\|N_T\|_2$. A sufficiently fast subsequence therefore converges uniformly [almost surely](../../../../../../almost-sure-convergence.md) on every compact time interval, giving the continuous version of the [stochastic integral](../../../../../../stochastic-integral.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
