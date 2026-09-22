<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The equal-[variance](../../../../../variance-split.md) form of [Slepian's lemma](../../../../../slepian-s-lemma.md) is the following. If $U,V$ are centered vectors with [multivariate normal distributions](../../../../../multivariate-normal-distribution.md), $\mathbb EU_i^2=\mathbb EV_i^2$ for every $i$, and $\mathbb EU_iU_j\geq\mathbb EV_iV_j$ whenever $i\ne j$, then

$$
\mathbb P(U_i\leq u_i\text{ for all }i)\geq\mathbb P(V_i\leq u_i\text{ for all }i)
$$

for every threshold vector $(u_i)$. In particular $\mathbb P(\max_iU_i\leq u)\geq\mathbb P(\max_iV_i\leq u)$. No nonsingularity of the [covariance matrices](../../../../../covariance-matrix.md) is required.

Here the pointwise [variances](../../../../../variance-split.md) $2t^{2H}$ and $2t^{2H'}$ differ. To make the comparison rigorous, use the increment form, namely the [Sudakov-Fernique inequality](../../../../../sudakov-fernique-inequality.md): if centered [multivariate normal distributions](../../../../../multivariate-normal-distribution.md) satisfy $\mathbb E(U_i-U_j)^2\leq\mathbb E(V_i-V_j)^2$ for every pair, then $\mathbb E\max_iU_i\leq\mathbb E\max_iV_i$. Unlike the preceding form of [Slepian's lemma](../../../../../slepian-s-lemma.md), this statement has no equal-pointwise-[variance](../../../../../variance-split.md) hypothesis.

For completeness, the increment form follows by [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md). Make $U,V$ [independent](../../../../../independent-random-variables.md), define $Z_r=\sqrt{1-r}U+\sqrt rV$ for $0<r<1$, and let

$$
F_\tau(z)=\frac1\tau\log\sum_{i=1}^n e^{\tau z_i},\qquad p_i(z)=\frac{e^{\tau z_i}}{\sum_j e^{\tau z_j}},\qquad D=\operatorname{Cov}(V)-\operatorname{Cov}(U).
$$

The $p_i$ are [softmax function](../../../../../softmax-function.md) weights, with $p_i\geq0$ and $\sum_i p_i=1$. Direct differentiation gives $\partial_iF_\tau=p_i$ and $\partial_{ij}F_\tau=\tau(p_i\mathbf1_{i=j}-p_ip_j)$. The [Gaussian integration by parts](../../../../../stein-s-lemma-probability.md) identity therefore yields

$$
\begin{aligned}
\frac d{dr}\mathbb EF_\tau(Z_r)&=\frac12\sum_{i,j}D_{ij}\mathbb E[\partial_{ij}F_\tau(Z_r)]\\
&=\frac\tau4\mathbb E\sum_{i,j}p_ip_j(D_{ii}+D_{jj}-2D_{ij})\geq0.
\end{aligned}
$$

The last summands are nonnegative because $D_{ii}+D_{jj}-2D_{ij}=\mathbb E(V_i-V_j)^2-\mathbb E(U_i-U_j)^2$. Since

$$
\max_i z_i\leq F_\tau(z)\leq\max_i z_i+\frac{\log n}{\tau},
$$

integration in $r$ and the limit $\tau\to\infty$ prove the [Sudakov-Fernique inequality](../../../../../sudakov-fernique-inequality.md). All derivatives needed here are bounded for a fixed $\tau$. Singular [covariance matrices](../../../../../covariance-matrix.md) can be handled by adding small [independent](../../../../../independent-random-variables.md) centered [normal](../../../../../normal-distribution.md) noise with the same variance to both vectors, proving the identity for the nonsingular vectors, and letting the noise variance decrease to zero.

Use the printed normalization of [fractional Brownian motion](../../../../../fractional-brownian-motion.md), which omits the conventional factor $1/2$. Its increment [variance](../../../../../variance-split.md) is

$$
\mathbb E|X_H(t)-X_H(s)|^2=2|t-s|^{2H},\qquad \mathbb E|Y_{H'}(t)-Y_{H'}(s)|^2=2|t-s|^{2H'}.
$$

For $s,t\in[0,1]$ and $H>H'$, $|t-s|^{2H}\leq|t-s|^{2H'}$. Enumerate $T$ by increasing finite subsets $T_n$ whose union is $T$, with $0\in T_n$. The [Sudakov-Fernique inequality](../../../../../sudakov-fernique-inequality.md) gives

$$
\mathbb E\max_{t\in T_n}X_H(t)\leq\mathbb E\max_{t\in T_n}Y_{H'}(t).
$$

Both [Gaussian processes](../../../../../gaussian-process.md) vanish at zero almost surely. Thus these maxima are nonnegative and increase with $n$; [monotone convergence theorem](../../../../../monotone-convergence-theorem.md) gives

$$
\mathbb E\sup_{t\in T}X_H(t)\leq\mathbb E\sup_{t\in T}Y_{H'}(t).
$$

Their [continuous modifications](../../../../../continuous-modification.md) agree with the original [Gaussian processes](../../../../../gaussian-process.md) simultaneously on the countable set $T$, after discarding a single null event. Continuity and density of the rational parameters make each rational [supremum](../../../../../supremum.md) equal to the supremum over $[0,1]$ for these modifications.

The expected suprema are finite. Indeed, the canonical distance of $Y_{H'}$ is $d(s,t)=\sqrt2|t-s|^{H'}$. A Euclidean grid supplies a closed-ball [metric covering number](../../../../../metric-covering-number.md) bound $N(\varepsilon)\leq1+\lceil(\sqrt2/\varepsilon)^{1/H'}\rceil$ for $0<\varepsilon\leq\sqrt2$. The [Dudley entropy integral](../../../../../dudley-entropy-integral.md) bound for an anchored centered separable [Gaussian process](../../../../../gaussian-process.md) is

$$
\mathbb E\sup_tY_{H'}(t)\leq C\int_0^{\sqrt2}\sqrt{\log N(\varepsilon)}\,d\varepsilon<\infty.
$$

The integral is finite since its integrand grows at most like a constant times $\sqrt{1+\log(1/\varepsilon)}$ near zero. The same argument applies to $X_H$.

For any real path vanishing at zero,

$$
\sup_{t\in T}|x(t)|\leq\sup_{t\in T}x(t)+\sup_{t\in T}(-x(t)).
$$

A centered [Gaussian process](../../../../../gaussian-process.md) has the same [probability law](../../../../../probability-distribution.md) as its negative. Combining this symmetry with the increment comparison gives the stronger bound

$$
\mathbb E\sup_{t\in T}|X_H(t)|\leq2\mathbb E\sup_{t\in T}X_H(t)\leq2\mathbb E\sup_{t\in T}Y_{H'}(t)\leq2\mathbb E\sup_{t\in T}|Y_{H'}(t)|.
$$

In particular the requested comparison is

$$
\boxed{\mathbb E\sup_{t\in T}|X_H(t)|\leq4\mathbb E\sup_{t\in T}|Y_{H'}(t)|.}
$$

The common normalization factor $\sqrt2$ affects both sides equally. The comparison is valid for every $0<H'<H<1$, including the equality cases $s=t$ or $|s-t|=1$ in the increment bounds.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 217](../../paper-217-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
