<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

For $f(x)=x$, the [continuous martingale](../../../../../continuous-martingale.md) is $M_t^f=B_t$. Since $B_t$ has the centered [normal distribution](../../../../../normal-distribution.md) of variance $t$,

$$
\mathbb E|M_t^f|^2=t=\int_0^t\mathbb E|f'(B_s)|^2\,ds.
$$

For $f(x)=x^2$, the [continuous martingale](../../../../../continuous-martingale.md) is $B_t^2-t$. The [Gaussian fourth moment](../../../../../gaussian-fourth-moment.md) gives

$$
\mathbb E(B_t^2-t)^2=3t^2-2t^2+t^2=2t^2=\int_0^t4\mathbb EB_s^2\,ds.
$$

This verifies both cases. The time integral in the printed identity is understood with its omitted $ds$.

Write $M^{(n)}=M^{f_n}$. The derivatives of the approximations are

$$
g_n(x):=f_n'(x)=\begin{cases}-1&x\le-1/n,\\nx&|x|<1/n,\\1&x\ge1/n.\end{cases}
$$

Thus $|g_n|\le1$. The [Itô formula](../../../../../ito-s-lemma.md) gives $M_t^{(n)}=\int_0^t g_n(B_s)\,dB_s$. This use of the formula is valid despite the two second-derivative discontinuities: mollify the $C^1$ function $f_n$, whose derivative is Lipschitz. Its smooth derivatives converge boundedly, while the second derivatives are bounded by $n$ and converge except at $\pm1/n$. For every $s>0$, the [normal distribution](../../../../../normal-distribution.md) of $B_s$ assigns those points zero [probability](../../../../../probability.md). [Dominated convergence](../../../../../dominated-convergence-theorem.md) for the drift integral and the [Itô isometry](../../../../../ito-isometry.md) for the stochastic integral pass the smooth formula to $f_n$. Equivalently, this identifies the [martingale](../../../../../martingale-split.md) in the assumed decomposition and permits its cross-covariances to be calculated.

If $m\ge n$, then $|g_m-g_n|\le\mathbf1_{\{|x|<1/n\}}$. The [Itô isometry](../../../../../ito-isometry.md) and [Doob L2 maximal inequality](../../../../../doob-l2-maximal-inequality.md) therefore give, for every fixed $T$,

$$
\mathbb E\sup_{s\le T}|M_s^{(m)}-M_s^{(n)}|^2\le4\int_0^T\mathbb E|g_m(B_s)-g_n(B_s)|^2\,ds\le4\int_0^T\mathbb P(|B_s|<1/n)\,ds.
$$

The [Gaussian density](../../../../../multivariate-normal-density.md) is bounded by $(2\pi s)^{-1/2}$, so

$$
\mathbb P(|B_s|<1/n)\le\frac{\sqrt{2/\pi}}{n\sqrt s},\qquad \mathbb E\sup_{s\le T}|M_s^{(m)}-M_s^{(n)}|^2\le\frac{8\sqrt{2T/\pi}}n.
$$

Consequently the processes are Cauchy in the complete space of continuous random paths with norm $(\mathbb E\sup_{s\le T}|Z_s|^2)^{1/2}$. They have a continuous-path limit $M$ there. Limits obtained for different integer horizons agree on overlaps; choose these versions consistently. Each $M_t$ is adapted, and passing to the $L^2$ limit in $\mathbb E[M_t^{(n)}\mid\mathcal F_s]=M_s^{(n)}$ shows that $M$ is a [continuous martingale](../../../../../continuous-martingale.md). Letting $m\to\infty$ in the preceding bound proves the requested convergence, with an explicit rate:

$$
\boxed{\mathbb E\sup_{s\le T}|M_s^{(n)}-M_s|^2\le\frac{8\sqrt{2T/\pi}}n\longrightarrow0.}
$$

The same [Itô isometry](../../../../../ito-isometry.md) identifies $M_t=\int_0^t\operatorname{sgn}(B_s)\,dB_s$, with $\operatorname{sgn}(0)=0$.

There is a genuine **factor-of-two error in the last printed conclusion**. The stated $f_n$ has second derivative $n\mathbf1_{\{|x|<1/n\}}$ almost everywhere, and the generator in the decomposition is one half of the second derivative. Hence the exact identity is

$$
L_n(t):=\frac n2\int_0^t\mathbf1_{\{|B_s|<1/n\}}\,ds=f_n(B_t)-f_n(0)-M_t^{(n)}.
$$

Because $\sup_x|f_n(x)-|x||\le1/(2n)$ and $f_n(0)=1/(2n)$, this already proves uniform $L^2$ convergence on bounded intervals to $L_t=|B_t|-M_t$. It does not by itself prove almost-sure convergence of the full sequence, so we supply that additional step.

Take $n_k=k^2$. For each fixed integer $T$ and each $\varepsilon>0$, the maximal-error bound and [Markov's inequality](../../../../../markov-inequality.md) imply

$$
\sum_k\mathbb P\!\left(\sup_{s\le T}|M_s^{(k^2)}-M_s|>\varepsilon\right)\le\frac{8\sqrt{2T/\pi}}{\varepsilon^2}\sum_k\frac1{k^2}<\infty.
$$

The first [Borel-Cantelli lemma](../../../../../borel-cantelli-lemmas.md), applied to rational positive $\varepsilon$ and integer $T$, gives uniform almost-sure convergence of this subsequence on every bounded interval. Therefore $L_{k^2}\to L$ uniformly there [almost surely](../../../../../almost-sure-convergence.md).

For $k^2\le n\le(k+1)^2$, the indicator windows are nested. The [ratio-one interpolation for shrinking-window occupation integrals](../../../../../ratio-one-interpolation-for-shrinking-window-occupation-integrals.md) gives

$$
\frac n{(k+1)^2}L_{(k+1)^2}(t)\le L_n(t)\le\frac n{k^2}L_{k^2}(t).
$$

Both ratios tend uniformly to one as $k\to\infty$. The two bounds converge uniformly to the continuous nonnegative process $L$, so the entire sequence does too. Thus the correct normalized conclusion is

$$
\boxed{\frac n2\int_0^t\mathbf1_{\{|B_s|<1/n\}}\,ds\longrightarrow |B_t|-M_t\quad\text{almost surely},}
$$

and with the factor actually printed in the question the limit is

$$
\boxed{n\int_0^t\mathbf1_{\{|B_s|<1/n\}}\,ds\longrightarrow2(|B_t|-M_t).}
$$

These are the [occupation approximations for Brownian local time](../../../../../occupation-approximations-for-brownian-local-time.md). In the [Tanaka formula](../../../../../tanaka-s-formula.md) convention, $L_t$ is the [local time of a semimartingale](../../../../../local-time-of-a-semimartingale.md) at zero. It is not identically zero: $\mathbb EL_t=\mathbb E|B_t|=\sqrt{2t/\pi}>0$ for $t>0$, since $M$ starts at zero and is a [martingale](../../../../../martingale-split.md). Thus the discrepancy cannot be removed by treating the two limits as equal. The standard normalization is also given in [Lalley's notes on the Itô calculus and local time](https://galton.uchicago.edu/~lalley/Courses/385/ItoIntegral.pdf).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 31](../../paper-31-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
