<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use the [Fourier transform](../../../../../fourier-transform.md) convention $\widehat h(\xi)=\int h(x)e^{-2\pi ix\cdot\xi}\,dx$. The deleted-ball kernel need not be integrable at infinity, so first work with finite annuli. Write

$$
m_{\varepsilon,R}(\xi)=\int_{\varepsilon<|x|<R}K(x)e^{-2\pi ix\cdot\xi}\,dx.
$$

We will prove a uniform bound, convergence as $R\to\infty$, and then convergence as $\varepsilon\downarrow0$. This makes all Fourier-transform assertions precise for the [annularly cancelling singular convolution kernel](../../../../../annularly-cancelling-singular-convolution-kernel.md).

Fix $\xi\ne0$ and put $y=\xi/(2|\xi|^2)$, so $e^{-2\pi iy\cdot\xi}=-1$. For $R>r\geq4|y|$, let $\Omega=\{r<|x|<R\}$ and define

$$
I_{r,R}=\int_\Omega K(x)e^{-2\pi ix\cdot\xi}\,dx,\qquad J_{r,R}=\int_\Omega K(x-y)e^{-2\pi ix\cdot\xi}\,dx.
$$

The [Hörmander integral kernel condition](../../../../../hormander-integral-kernel-condition.md) gives

$$
|I_{r,R}-J_{r,R}|\leq\int_{|x|>r}|K(x)-K(x-y)|\,dx.
$$

On changing variables $u=x-y$, the phase factor shows $J_{r,R}=-\int_{\Omega-y}K(u)e^{-2\pi iu\cdot\xi}\,du$. The symmetric difference between $\Omega$ and $\Omega-y$ lies in the two shells whose radii are within $|y|$ of $r$ and $R$. On each such shell, the kernel's size bound gives, by polar integration,

$$
\int_{s-|y|<|u|<s+|y|}|K(u)|\,du\leq A|\mathbb S^{d-1}|\log\frac{s+|y|}{s-|y|}\leq C_d A\frac{|y|}{s}\quad(s\geq4|y|).
$$

Therefore

$$
|I_{r,R}+J_{r,R}|\leq C_dA|y|(r^{-1}+R^{-1}),
$$

and adding the two comparisons proves the [oscillatory tail estimate for a singular kernel](../../../../../oscillatory-tail-estimate-for-a-singular-kernel.md):

$$
\boxed{|I_{r,R}|\leq\frac12\int_{|x|>r}|K(x)-K(x-y)|\,dx+C_dA\frac{|y|}{r}}.
$$

The integral on the right is at most $B$. Moreover, for fixed $\xi$, it tends to zero as $r\to\infty$ because the translated difference is absolutely integrable outside $2|y|$. The shell term also tends to zero. Thus the far Fourier integral is Cauchy and converges as its outer radius tends to infinity.

Set $r_0=4|y|=2/|\xi|$. If $\varepsilon<r_0$, annular cancellation allows subtraction of the constant phase on the near annulus:

$$
\begin{aligned}
\left|\int_{\varepsilon<|x|<r_0}K(x)e^{-2\pi ix\cdot\xi}\,dx\right|
&=\left|\int_{\varepsilon<|x|<r_0}K(x)(e^{-2\pi ix\cdot\xi}-1)\,dx\right|\\
&\leq2\pi A|\xi|\int_{|x|<r_0}|x|^{1-d}\,dx\leq C_d A.
\end{aligned}
$$

The same estimate applies to a shorter near annulus when $R<r_0$. The far annulus is bounded by $B/2+C_dA$, using the tail estimate; if $\varepsilon\geq r_0$, apply that estimate with $r=\varepsilon$. At $\xi=0$ the annular integral vanishes by cancellation. We have proved

$$
\sup_{\varepsilon,R,\xi}|m_{\varepsilon,R}(\xi)|\leq C_dA+B/2.
$$

For each fixed $\varepsilon>0$, the size bound makes $K_\varepsilon\in L^2$, and $K1_{\{\varepsilon<|x|<R\}}\to K_\varepsilon$ in $L^2$ as $R\to\infty$. By the [Plancherel theorem](../../../../../plancherel-theorem.md), their Fourier transforms converge in $L^2$ to $\widehat K_\varepsilon$. The pointwise improper limits just established identify this transform, up to a null set, with

$$
m_\varepsilon(\xi)=\lim_{R\to\infty}m_{\varepsilon,R}(\xi).
$$

For example identification follows by selecting an almost-everywhere convergent subsequence from the $L^2$ convergence. Hence

$$
\boxed{\sup_{\varepsilon>0}\|\widehat K_\varepsilon\|_\infty\leq C_dA+B/2}.
$$

The near-annulus integral with the constant phase subtracted converges absolutely at zero, since its bound is proportional to $|x|^{1-d}$. The far integral has already converged. Therefore $m_\varepsilon(\xi)\to m(\xi)$ for every $\xi\ne0$, with the same uniform bound; the value at zero may be set arbitrarily.

For $f\in L^2$, the [convolution](../../../../../convolution.md) $K_\varepsilon*f$ is absolutely convergent for each $x$ by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md). Its [Fourier transform](../../../../../fourier-transform.md) is $m_\varepsilon\widehat f$: first prove this for [Schwartz functions](../../../../../schwartz-function.md) and then approximate any $L^2$ input. The convolutions converge uniformly under this approximation by the same Cauchy-Schwarz bound, and the multiplier outputs converge in $L^2$ by their uniform operator bound, so these two definitions agree. Define the bounded [Fourier multiplier operator](../../../../../fourier-multiplier-operator.md) $T$ by $\widehat{Tf}=m\widehat f$. [Dominated convergence theorem](../../../../../dominated-convergence-theorem.md) and the [Plancherel theorem](../../../../../plancherel-theorem.md) now give

$$
\boxed{\|T_\varepsilon f-Tf\|_2^2=\int|m_\varepsilon-m|^2|\widehat f|^2\,d\xi\longrightarrow0}.
$$

For the final request, use a normalized [bump function](../../../../../bump-function.md), $\int\phi=1$, so that its dilates form an [approximate identity](../../../../../approximate-identity.md). Multiplying Fourier transforms gives

$$
\widehat{T(\phi_\varepsilon)*f}=m\widehat\phi(\varepsilon\xi)\widehat f=\widehat{\phi_\varepsilon*(Tf)}.
$$

These products are integrable by [Cauchy-Schwarz inequality](../../../../../cauchy-schwarz-inequality.md), since $T\phi_\varepsilon,f\in L^2$, and also define $L^2$ functions because $m$ and $\widehat\phi$ are bounded. Thus the [convolution](../../../../../convolution.md) identity is justified even though $T\phi_\varepsilon$ need not be in $L^1$:

$$
T(\phi_\varepsilon)*f=\phi_\varepsilon*(Tf).
$$

The allowed standard [approximate identity](../../../../../approximate-identity.md) results, applied to $Tf\in L^2$, prove convergence to $Tf$ in norm and [almost everywhere](../../../../../almost-everywhere.md). This is the [mass normalization in mollified singular integrals](../../../../../mass-normalization-in-mollified-singular-integrals.md); it does not require proving almost-everywhere convergence of the sharp truncations $T_\varepsilon f$.

If “bump function” means merely smooth with compact support, the stated limit needs the unit-integral qualification. For arbitrary such $\phi$, the limit is $(\int\phi)Tf$ instead. This is also the almost-everywhere limit: at each [Lebesgue point](../../../../../lebesgue-point.md) of $Tf$, subtract $(\int\phi)Tf(x)$ inside the convolution and bound the remaining local average by the boundedness and compact support of $\phi$. As a concrete counterexample without normalization, take $K(x)=1/(\pi x)$ in dimension one and $\phi=2\rho$ for a unit-integral [mollifier](../../../../../mollifier.md) $\rho$. This kernel has the required size, odd annular cancellation, and translation-difference integral $\log(3)/\pi$ on $\{|x|>2|y|\}$ for every $y\ne0$. Its limit operator is the nonzero [Hilbert transform](../../../../../hilbert-transform.md); by the [Hilbert-transform Fourier multiplier](../../../../../hilbert-transform-fourier-multiplier.md), it is an $L^2$ isometry. For any nonzero $f\in L^2$ the mollified limit is $2Tf$, not $Tf$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 8](../../paper-8-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
