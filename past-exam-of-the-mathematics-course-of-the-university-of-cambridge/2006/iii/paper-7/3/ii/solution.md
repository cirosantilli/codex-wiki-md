<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $\widehat f(\lambda)=\int f(t)e^{-i\lambda t}\,dt$ and interpret the regularity assumption to include $f\in L^2(\mathbb R)$ with the continuous representative furnished by [Fourier inversion](../../../../../../fourier-inversion-theorem.md). Write $F=\widehat f$. The bandwidth assumption implies $F\in L^1$ as well as $L^2$, by the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) on its finite support, so

$$
f(t)=\frac1{2\pi}\int_{-\pi}^{\pi}F(\lambda)e^{it\lambda}\,d\lambda
$$

is continuous and defined at every $t$. The integer samples are precisely the [Fourier coefficients](../../../../../../fourier-coefficient.md) of $F$ with the sign convention appropriate to the basis $e^{-in\lambda}$:

$$
f(n)=\frac1{2\pi}\int_{-\pi}^{\pi}F(\lambda)e^{in\lambda}\,d\lambda.
$$

The completeness and [Parseval identity](../../../../../../parseval-identity.md) for the exponential [orthonormal basis](../../../../../../orthonormal-basis.md) on $[-\pi,\pi]$ give $F=\sum_{n\in\mathbb Z}f(n)e^{-in\lambda}$ in $L^2$ and

$$
\sum_{n\in\mathbb Z}|f(n)|^2=\frac1{2\pi}\|F\|_2^2=\|f\|_2^2.
$$

The last equality is the [Plancherel theorem](../../../../../../plancherel-theorem.md). Apply the inverse integral to the finite symmetric [Fourier partial sums](../../../../../../fourier-partial-sum.md). Since

$$
\frac1{2\pi}\int_{-\pi}^{\pi}e^{i(t-n)\lambda}\,d\lambda=\frac{\sin\pi(t-n)}{\pi(t-n)},
$$

we obtain the [Nyquist–Shannon sampling theorem](../../../../../../nyquist-shannon-sampling-theorem.md) in this normalization:

$$
\boxed{f(t)=\sum_{n\in\mathbb Z}f(n)\frac{\sin\pi(t-n)}{\pi(t-n)}\quad(t\in\mathbb R),}
$$

where the quotient is one at $t=n$. This is a [sampling expansion by periodic Fourier projection](../../../../../../sampling-expansion-by-periodic-fourier-projection.md), not merely an almost-everywhere inversion. Indeed, the inverse integral of an error $G\in L^2[-\pi,\pi]$ is bounded, uniformly in $t$, by $\|G\|_2/\sqrt{2\pi}$. Hence the symmetric finite sampling sums converge uniformly on all of $\mathbb R$. Moreover, the [Parseval identity](../../../../../../parseval-identity.md) applied to $e^{it\lambda}$ gives

$$
\sum_{n\in\mathbb Z}\left|\frac{\sin\pi(t-n)}{\pi(t-n)}\right|^2=1.
$$

The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) therefore makes the sampling series absolutely convergent at every $t$, with its absolute tail bounded uniformly by $(\sum_{|n|>N}|f(n)|^2)^{1/2}$. Thus the integer samples recover the function everywhere.

For the nonuniqueness beyond this bandwidth, fix $0<\epsilon_0<\min(\epsilon,\pi)$ and a nonzero smooth function $\Phi$ compactly supported in $(-\epsilon_0,\epsilon_0)$. Let $h$ be its inverse [Fourier transform](../../../../../../fourier-transform.md) and put

$$
g(t)=\sin(\pi t)h(t),\qquad \widehat g(\lambda)=\frac{\Phi(\lambda-\pi)-\Phi(\lambda+\pi)}{2i}.
$$

The function $h$, and hence $g$, is a [Schwartz function](../../../../../../schwartz-function.md). The two shifted spectral supports are disjoint, so $\widehat g\ne0$, but its support is contained strictly inside $(-\pi-\epsilon,\pi+\epsilon)$. Every integer sample of $g$ is zero. Therefore **$g$ and the zero function have identical samples but are distinct**, providing a [strictly supercritical sampling alias counterexample](../../../../../../strictly-supercritical-sampling-alias-counterexample.md) for every positive bandwidth enlargement.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
