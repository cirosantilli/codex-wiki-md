<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Let the summands be [independent and identically distributed random variables](../../../../../independent-and-identically-distributed-random-variables.md) with mean $\mu$, [variance](../../../../../variance-split.md) $\sigma^2>0$, and standardized third [cumulant](../../../../../cumulant.md) $\gamma_1=\mathbb E[(Y_1-\mu)^3]/\sigma^3$. Define

$$
S_n^*=\frac{\sum_{i=1}^n(Y_i-\mu)}{\sigma\sqrt n}.
$$

An [Edgeworth expansion](../../../../../edgeworth-series.md) refines the [central limit theorem](../../../../../central-limit-theorem.md) using the higher [cumulants](../../../../../cumulant.md) of one summand. Some smoothness and moment assumptions are essential: finite [variance](../../../../../variance-split.md) alone does not supply a density expansion. A convenient sufficient set for the expansions here is a smooth density whose [derivatives](../../../../../derivative.md) decay faster than every inverse power, together with $\mathbb E e^{\delta|Y_1|}<\infty$ for some $\delta>0$. These assumptions give all required moments, Fourier smoothing and the nonlattice characteristic-function condition. Less restrictive sufficient conditions are possible, but this set covers the logistic model below.

Write $\phi$ and $\Phi$ for the [standard normal density](../../../../../standard-normal-density.md) and [standard normal distribution function](../../../../../standard-normal-distribution-function.md). The first-order density [Edgeworth expansion](../../../../../edgeworth-series.md) is

$$
\boxed{p_{S_n^*}(x)=\phi(x)\left[1+\frac{\gamma_1}{6\sqrt n}(x^3-3x)\right]+O(n^{-1}).}
$$

The remainder is uniform on every fixed compact interval under the stated assumptions. To see the origin of the correction, for $Z=(Y_1-\mu)/\sigma$ the [cumulant expansion](../../../../../cumulant-expansion.md) of its [characteristic function](../../../../../characteristic-function.md) gives

$$
n\log\mathbb E e^{itZ/\sqrt n}
=-\frac{t^2}{2}+\frac{\gamma_1(it)^3}{6\sqrt n}+O(n^{-1}).
$$

Exponentiating and using [Fourier inversion](../../../../../fourier-inversion-theorem.md) yields the displayed correction, since the inverse transform of $(it)^3e^{-t^2/2}$ is $-\phi^{(3)}(x)=(x^3-3x)\phi(x)$. The [Probabilists' Hermite polynomial](../../../../../probabilists-hermite-polynomial.md) convention is being used: $H_2(x)=x^2-1$ and $H_3(x)=x^3-3x$.

The corresponding [distribution function](../../../../../cumulative-distribution-function.md) expansion is

$$
\boxed{F_{S_n^*}(x)=\Phi(x)-\frac{\gamma_1}{6\sqrt n}(x^2-1)\phi(x)+O(n^{-1}),}
$$

uniformly on fixed compact intervals. The sign follows from $\frac{d}{dx}[H_2(x)\phi(x)]=-H_3(x)\phi(x)$. These are expansions of both the density and [distribution function](../../../../../cumulative-distribution-function.md); a uniform density error alone would not justify integrating an error bound over the entire real line without the accompanying tail control.

For a fixed $\alpha\in(0,1)$, write $z=z_\alpha=\Phi^{-1}(\alpha)$. At leading order the proposed [quantile](../../../../../quantile-function.md) expansion gives $\Phi(p_0(z))=\Phi(z)$, and strict monotonicity gives $p_0(z)=z$. Substitute $y_\alpha=z+p_1(z)n^{-1/2}+O(n^{-1})$ into the [distribution function](../../../../../cumulative-distribution-function.md) expansion. A [Taylor expansion](../../../../../taylor-expansion.md) at $z$ gives

$$
F_{S_n^*}(y_\alpha)
=\alpha+\frac{\phi(z)}{\sqrt n}\left[p_1(z)-\frac{\gamma_1}{6}(z^2-1)\right]+O(n^{-1}).
$$

Since $\phi(z)>0$, the coefficient of $n^{-1/2}$ must vanish. Thus the first [Cornish-Fisher expansion](../../../../../cornish-fisher-expansion.md) coefficients are

$$
\boxed{p_0(z)=z,\qquad p_1(z)=\frac{\gamma_1}{6}(z^2-1).}
$$

For the [logistic distribution](../../../../../logistic-distribution.md), set $Z_i=Y_i-\theta$. Its density $q(z)=e^z/(1+e^z)^2$ satisfies $q(-z)=q(z)$ and has exponentially decreasing tails. Symmetry and integrability give $\mathbb E Z_i=0$, and the supplied integral gives

$$
\mathbb E Z_i^2=2\int_0^\infty\frac{z^2e^z}{(1+e^z)^2}\,dz=\frac{\pi^2}{3}.
$$

Therefore $\mathbb E Y_i=\theta$, $\operatorname{Var}(Y_i)=\pi^2/3$, and the [central limit theorem](../../../../../central-limit-theorem.md) gives

$$
T_n=\frac{\sqrt n(\bar Y-\theta)}{\pi/\sqrt3}\xrightarrow{d}N(0,1).
$$

Writing $z_-=z_{\alpha/2}$ and $z_+=z_{1-\alpha/2}$, the condition $z_-\leq T_n\leq z_+$ is equivalent to

$$
\bar Y-\frac{\pi}{\sqrt{3n}}z_+\leq\theta\leq
\bar Y-\frac{\pi}{\sqrt{3n}}z_-.
$$

Consequently the [confidence interval](../../../../../confidence-interval.md)

$$
\boxed{\left(\bar Y-\frac{\pi}{\sqrt{3n}}z_{1-\alpha/2},\quad
\bar Y-\frac{\pi}{\sqrt{3n}}z_{\alpha/2}\right)}
$$

has limiting coverage $\Phi(z_+)-\Phi(z_-)=1-\alpha$. Whether the finite endpoints are included makes no probability difference because the sample mean has a density.

The centered [logistic distribution](../../../../../logistic-distribution.md) is symmetric, so $\gamma_1=0$. Its smooth density and exponentially decreasing [derivatives](../../../../../derivative.md) satisfy the conditions stated above; in particular all moments exist and Fourier smoothing is available. The first correction in the [Edgeworth expansion](../../../../../edgeworth-series.md) vanishes, leaving $F_{T_n}(z)=\Phi(z)+O(n^{-1})$ at each of the two fixed [quantiles](../../../../../quantile-function.md). Subtracting gives the stronger conclusion

$$
\boxed{P_\theta(\theta\text{ lies in the interval})=1-\alpha+O(n^{-1}).}
$$

The standardized law is independent of $\theta$, so this coverage-error conclusion holds with the same bound for every location parameter.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 42](../../paper-42-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
