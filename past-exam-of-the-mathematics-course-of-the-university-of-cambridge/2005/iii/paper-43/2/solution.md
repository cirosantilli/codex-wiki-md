<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $M(t)=\mathbb Ee^{tX}$, with $M(0)=1$, and differentiate $\kappa(t)=\log M(t)$:

$$
\begin{aligned}
\kappa'(t)&=\frac{M'(t)}{M(t)},\\
\kappa''(t)&=\frac{M''(t)}{M(t)}-\frac{M'(t)^2}{M(t)^2},\\
\kappa'''(t)&=\frac{M'''(t)}{M(t)}-\frac{3M'(t)M''(t)}{M(t)^2}
 +\frac{2M'(t)^3}{M(t)^3}.
\end{aligned}
$$

Using $M^{(j)}(0)=\mathbb EX^j$ and $\mu=\mathbb EX$ gives

$$
\boxed{\kappa_1=\mu,\qquad\kappa_2=\mathbb EX^2-\mu^2=\operatorname{Var}X,\qquad
\kappa_3=\mathbb EX^3-3\mu\mathbb EX^2+2\mu^3=\mathbb E(X-\mu)^3.}
$$

Thus the first three [cumulants](../../../../../cumulant.md) are the mean, [variance](../../../../../variance-split.md) and third [central moment](../../../../../central-moment.md). A finite [moment-generating function](../../../../../moment-generating-function.md) near zero justifies these differentiations. For positive claims with only three finite ordinary [moments](../../../../../moment.md), the same calculations are valid as left [derivatives](../../../../../derivative.md) at zero of the logarithm of the [Laplace transform of a nonnegative random variable](../../../../../laplace-transform-of-a-nonnegative-random-variable.md); positive [exponential moments](../../../../../exponential-moment.md) are not needed for the resulting [moment](../../../../../moment.md) identities.

For the independent [Poisson distribution](../../../../../poisson-distribution.md) count, the [random-sum transform identity](../../../../../random-sum-transform-identity.md) gives

$$
M_S(t)=\exp\{\lambda(M_{X_1}(t)-1)\},\qquad
\kappa_S(t)=\lambda(M_{X_1}(t)-1).
$$

Consequently the [compound Poisson distribution](../../../../../compound-poisson-distribution.md) has

$$
\kappa_{S,1}=\lambda m_1,\qquad
\kappa_{S,2}=\lambda m_2,\qquad
\kappa_{S,3}=\lambda m_3.
$$

These are raw severity [moments](../../../../../moment.md), not severity [cumulants](../../../../../cumulant.md).

The printed gamma density uses rate $\nu$, not scale. Direct integration against $e^{ty}$ gives

$$
M_Y(t)=\left(\frac\nu{\nu-t}\right)^\alpha\quad(t<\nu),\qquad
\kappa_V(t)=kt-\alpha\log(1-t/\nu).
$$

Therefore the required matching equations for the [shifted gamma distribution](../../../../../shifted-gamma-distribution.md) are

$$
k+\frac\alpha\nu=\lambda m_1,\qquad
\frac\alpha{\nu^2}=\lambda m_2,\qquad
\frac{2\alpha}{\nu^3}=\lambda m_3.
$$

For $\lambda>0$ and nonzero positive claims with finite $m_3$, these equations give positive $\alpha,\nu$ and the unique solution

$$
\boxed{\nu=\frac{2m_2}{m_3},\qquad
\alpha=\frac{4\lambda m_2^3}{m_3^2},\qquad
k=\lambda m_1-\frac{2\lambda m_2^2}{m_3}.}
$$

This is the [three-cumulant shifted gamma approximation](../../../../../three-cumulant-shifted-gamma-approximation.md). In particular, its [skewness](../../../../../skewness.md) $2/\sqrt\alpha$ equals $m_3/(\sqrt\lambda\,m_2^{3/2})$, the [skewness](../../../../../skewness.md) of $S$.

The competing [normal approximation to a compound Poisson aggregate](../../../../../normal-approximation-to-a-compound-poisson-aggregate.md) is

$$
\boxed{S\approx\mathcal N(\lambda m_1,\lambda m_2),\qquad
\mathbb P(S\leq x)\approx\Phi\!\left(\frac{x-\lambda m_1}{\sqrt{\lambda m_2}}\right).}
$$

To justify its large-count limit, let $\varphi_X$ be the claim [characteristic function](../../../../../characteristic-function.md). For fixed severity law with $m_2<\infty$, its expansion is $\varphi_X(u)=1+im_1u-m_2u^2/2+o(u^2)$. The [characteristic function](../../../../../characteristic-function.md) of $(S-\lambda m_1)/\sqrt{\lambda m_2}$ is

$$
\exp\left\{\lambda\left[\varphi_X\left(\frac t{\sqrt{\lambda m_2}}\right)-1\right]
-\frac{it\lambda m_1}{\sqrt{\lambda m_2}}\right\}
\longrightarrow e^{-t^2/2}.
$$

Thus it converges in distribution to a standard [normal distribution](../../../../../normal-distribution.md) as $\lambda\to\infty$.

The [normal approximation](../../../../../normal-approximation.md) is simple, uses only $m_1,m_2$, and works well in the centre when the count is large and standardized [skewness](../../../../../skewness.md) is small. It imposes symmetry, whereas positive compound-Poisson claims have positive third [cumulant](../../../../../cumulant.md). The shifted-gamma approximation reproduces that third [cumulant](../../../../../cumulant.md) and can better describe moderate right [skewness](../../../../../skewness.md). It requires a finite and reliably known third [moment](../../../../../moment.md), and matching three [cumulants](../../../../../cumulant.md) alone does not guarantee accurate extreme tails.

Neither continuous approximation reproduces the genuine atom $\mathbb P(S=0)=e^{-\lambda}$, which matters at small $\lambda$. The [normal distribution](../../../../../normal-distribution.md) also assigns [probability](../../../../../probability.md) $\Phi(-\sqrt\lambda m_1/\sqrt{m_2})$ to negative losses. The gamma approximation is bounded below by $k$, but **its fitted shift need not be nonnegative**: exponential claims of mean $\mu$ give $k=-\lambda\mu/3$, so it too can assign mass to negative losses. If $k>0$, it instead excludes some genuinely possible small losses. These support and atom discrepancies prevent either approximation from being a universal replacement for the exact aggregate law.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
