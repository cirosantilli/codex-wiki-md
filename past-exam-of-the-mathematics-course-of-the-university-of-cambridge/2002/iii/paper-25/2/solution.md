<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**First alternative.** The [Euler product](../../../../../euler-product.md) of the [Riemann zeta function](../../../../../riemann-zeta-function.md) is absolutely convergent for $\sigma>1$. Its [logarithm](../../../../../logarithm.md) and the nonnegative [trigonometric polynomial](../../../../../trigonometric-polynomial.md)

$$
3+4\cos u+\cos2u=2(1+\cos u)^2
$$

give

$$
3\log\zeta(\sigma)+4\log|\zeta(\sigma+it)|+\log|\zeta(\sigma+2it)|
=\sum_p\sum_{m\ge1}\frac{3+4\cos(mt\log p)+\cos(2mt\log p)}{mp^{m\sigma}}\ge0.
$$

Consequently $\zeta(\sigma)^3|\zeta(\sigma+it)|^4|\zeta(\sigma+2it)|\ge1$. Suppose $t\ne0$ and the [Riemann zeta function](../../../../../riemann-zeta-function.md) had a [zero](../../../../../zero-of-a-function.md) of order $m\ge1$ at $1+it$. As $\sigma\downarrow1$, its simple [pole](../../../../../pole.md) at one gives $\zeta(\sigma)=O((\sigma-1)^{-1})$, the alleged [zero](../../../../../zero-of-a-function.md) gives $\zeta(\sigma+it)=O((\sigma-1)^m)$, and $\zeta(\sigma+2it)$ remains bounded. The product would be $O((\sigma-1)^{4m-3})\to0$, contradicting its lower bound. Thus **there are no zeta [zeros](../../../../../zero-of-a-function.md) on $\Re s=1$**; the point $s=1$ itself is a [pole](../../../../../pole.md), not a [zero](../../../../../zero-of-a-function.md).

For the [first integral of the Chebyshev function](../../../../../first-integral-of-the-chebyshev-function.md), define

$$
\Psi_1(x)=\int_0^x\psi(u)\,du=\sum_{n\le x}(x-n)\Lambda(n).
$$

The [logarithmic derivative](../../../../../logarithmic-derivative.md) identity $-\zeta'/\zeta(s)=\sum_n\Lambda(n)n^{-s}$, valid for $\Re s>1$, leads to

$$
\boxed{\Psi_1(x)=\frac1{2\pi i}\int_{c-i\infty}^{c+i\infty}
-\frac{\zeta'(s)}{\zeta(s)}\frac{x^{s+1}}{s(s+1)}\,ds,\qquad c>1.}
$$

To verify the kernel rather than assume an inversion formula, integrate $y^s/(s(s+1))$ on the vertical line $\Re s=c$. Closing to the left when $y>1$ gives the [residues](../../../../../residue.md) at [zero](../../../../../zero-of-a-function.md) and minus one, namely $1-y^{-1}$; closing to the right when $0<y<1$ gives [zero](../../../../../zero-of-a-function.md). At $y=1$ the integral is [zero](../../../../../zero-of-a-function.md) as well. The horizontal integrals tend to [zero](../../../../../zero-of-a-function.md) because of the quadratic denominator, and the distant vertical integrals vanish in the indicated direction. Multiplying this kernel by $x$ with $y=x/n$ gives $(x-n)^+$. The [absolute convergence](../../../../../absolute-convergence.md) of the [Dirichlet series](../../../../../dirichlet-series.md) on $\Re s=c$, together with the integrable denominator, permits interchange with the integral and proves the formula.

Here is a quantitative contour route from this relation to the [Prime number theorem](../../../../../prime-number-theorem.md). Question 3 establishes a [zero-free region of the Riemann zeta function](../../../../../zero-free-region-of-the-riemann-zeta-function.md) and the accompanying bounds for its [logarithmic derivative](../../../../../logarithmic-derivative.md), independently of the [Prime number theorem](../../../../../prime-number-theorem.md). In a sufficiently narrow half-width region they imply

$$
\left|\frac{\zeta'(s)}{\zeta(s)}\right|\ll\log^2(T+3)
$$

on the left and horizontal sides of the rectangle with heights $\pm T$ and left edge $\sigma_L=1-b/(2\log(T+3))$, after making $b>0$ small enough also for bounded heights. The explanation of this bound is included at the end of Question 3. Take $c=1+1/\log x$ and $T=\exp(\sqrt{\log x})$. On the original line, the omitted tails are

$$
O\left(\frac{x^2\log x}{T}\right),
$$

since the [Euler product](../../../../../euler-product.md) bounds $|\zeta'/\zeta(c+it)|$ by $-\zeta'/\zeta(c)=O(\log x)$. Shift the truncated integral to the left edge. The only enclosed [pole](../../../../../pole.md) is at $s=1$, with [residue](../../../../../residue.md) $x^2/2$; the kernel [poles](../../../../../pole.md) at [zero](../../../../../zero-of-a-function.md) and minus one lie outside the rectangle. The left edge contributes $O(x^{2-b/(2\log(T+3))}\log^2(T+3))$, since $|s(s+1)|^{-1}\ll(1+t^2)^{-1}$ there. The two horizontal edges contribute $O(x^2\log^2(T+3)/T^2)$. In particular, for some $a>0$,

$$
\Psi_1(x)=\frac{x^2}{2}+O\left(x^2e^{-a\sqrt{\log x}}\right),
\qquad\text{so}\qquad\Psi_1(x)\sim\frac{x^2}{2}.
$$

It remains to remove the smoothing; differentiating an asymptotic formula would not justify this step. The [monotonicity](../../../../../monotonic-function.md) of the [Second Chebyshev function](../../../../../second-chebyshev-function.md) gives, for $h=\varepsilon x$ with $0<\varepsilon<1$,

$$
\frac{\Psi_1(x)-\Psi_1(x-h)}h\le\psi(x)
\le\frac{\Psi_1(x+h)-\Psi_1(x)}h.
$$

First let $x\to\infty$ with $\varepsilon$ fixed. After division by $x$, the lower and upper bounds tend to $1-\varepsilon/2$ and $1+\varepsilon/2$. Let $\varepsilon\downarrow0$ to obtain $\psi(x)\sim x$. Higher [prime powers](../../../../../prime-power.md) contribute $O(\sqrt x\log x)$ by the [Chebyshev estimate](../../../../../chebyshev-estimate.md), so $\theta(x)\sim x$. Finally [partial summation](../../../../../abel-s-summation-formula.md) gives

$$
\pi(x)=\frac{\theta(x)}{\log x}+\int_2^x\frac{\theta(t)}{t(\log t)^2}\,dt
\sim\frac{x}{\log x}.
$$

The integral is $O(x/\log^2x)$, by splitting at $\sqrt x$ and using $\theta(t)=O(t)$. This proves the [Prime number theorem](../../../../../prime-number-theorem.md) with **$\pi(x)\sim x/\log x$**.

**Second alternative.** We prove the [functional equation of the Riemann zeta function](../../../../../functional-equation-of-the-riemann-zeta-function.md) from a [theta function](../../../../../theta-function.md). Set $\Theta(u)=\sum_{n\in\mathbb Z}e^{-\pi n^2u}$ for $u>0$. With [Fourier transform](../../../../../fourier-transform.md) convention $\widehat f(\xi)=\int_{\mathbb R}f(v)e^{-2\pi iv\xi}\,dv$, the [Gaussian function](../../../../../gaussian-function.md) $f(v)=e^{-\pi uv^2}$ has

$$
\widehat f(\xi)=u^{-1/2}e^{-\pi\xi^2/u}.
$$

Indeed, differentiation under the integral and [integration by parts](../../../../../integration-by-parts.md) give $\widehat f'(\xi)=-2\pi\xi\widehat f(\xi)/u$, while the [Gaussian integral](../../../../../gaussian-integral.md) gives $\widehat f(0)=u^{-1/2}$. Periodize $f$: the smooth period-one function $\sum_n f(v+n)$ has [Fourier coefficients](../../../../../fourier-coefficient.md) $\widehat f(k)$, by integrating on $[0,1]$ and interchanging its absolutely convergent sum with the integral. Its absolutely convergent [Fourier series](../../../../../fourier-series-split.md), evaluated at [zero](../../../../../zero-of-a-function.md), proves the [Poisson summation formula](../../../../../poisson-summation-formula.md) in this case. Hence

$$
\Theta(u)=u^{-1/2}\Theta(1/u).
$$

For $\Re s>1$, termwise integration and the defining integral of the [Gamma function](../../../../../gamma-function.md) give the [Mellin representation of the completed Riemann zeta function](../../../../../mellin-representation-of-the-completed-riemann-zeta-function.md):

$$
Z(s):=\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\frac12\int_0^\infty(\Theta(u)-1)u^{s/2-1}\,du.
$$

Split at one and substitute $u=1/v$ in the lower integral. The elementary part is

$$
\frac12\int_0^1(u^{-1/2}-1)u^{s/2-1}\,du
=\frac1{s-1}-\frac1s=\frac1{s(s-1)},
$$

and the remaining part becomes an integral over $[1,\infty)$. Thus

$$
Z(s)=\frac1{s(s-1)}+\frac12\int_1^\infty(\Theta(u)-1)
\left(u^{s/2-1}+u^{(1-s)/2-1}\right)\,du.
$$

The integral is an [entire function](../../../../../entire-function.md) of $s$, because $\Theta(u)-1$ decays exponentially and [uniform convergence](../../../../../uniform-convergence.md) holds on every compact subset of the [complex plane](../../../../../complex-plane.md). This proves [meromorphic continuation](../../../../../meromorphic-continuation.md) of the [completed Riemann zeta function](../../../../../completed-riemann-zeta-function.md), with only the displayed simple [poles](../../../../../pole.md), and the right side is invariant under $s\mapsto1-s$. Therefore

$$
\boxed{\pi^{-s/2}\Gamma(s/2)\zeta(s)
=\pi^{-(1-s)/2}\Gamma((1-s)/2)\zeta(1-s).}
$$

The [Gamma reflection formula](../../../../../gamma-reflection-formula.md) and [Gamma duplication formula](../../../../../gamma-duplication-formula.md) give the equivalent form $\zeta(s)=2^s\pi^{s-1}\sin(\pi s/2)\Gamma(1-s)\zeta(1-s)$, understood by [meromorphic continuation](../../../../../meromorphic-continuation.md). Multiplication by $s(s-1)/2$ gives the [entire](../../../../../entire-function.md) [Riemann xi function](../../../../../riemann-xi-function.md) $\xi(s)=\xi(1-s)$.

Let $N(T)$ count positive ordinates of [Nontrivial zeros of the Riemann zeta function](../../../../../nontrivial-zero-of-the-riemann-zeta-function.md) up to height $T$, including [multiplicity](../../../../../multiplicity-mathematics.md). The [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md) is

$$
N(T)=\frac{T}{2\pi}\log\frac{T}{2\pi}-\frac{T}{2\pi}+O(\log T).
$$

More precisely, away from ordinates of [zeros](../../../../../zero-of-a-function.md), the constant term is $7/8$, the additional term is $S(T)=\pi^{-1}\arg\zeta(1/2+iT)$, and the remaining error is $O(T^{-1})$. Here the argument is continued along $2\to2+iT\to1/2+iT$, and $S(T)=O(\log T)$. The coarse formula displayed above holds at all large heights with the usual right-continuous counting convention. Subtract it at $T+1$ and $T$: the main term changes by $O(\log T)$ and each error is $O(\log T)$. Hence

$$
\boxed{N(T+1)-N(T)\ll\log T.}
$$

For [infinitely many reciprocal-logarithmic gaps between zeta zeros](../../../../../infinitely-many-reciprocal-logarithmic-gaps-between-zeta-zeros.md), fix any $0<c<2\pi$, for example $c=\pi$. Suppose all sufficiently late gaps satisfied $\gamma_{n+1}-\gamma_n\le c/\log n$. Summing and using

$$
\sum_{j=2}^{n}\frac1{\log j}\sim\frac n{\log n}
$$

gives $\gamma_n\le(c+o(1))n/\log n$. The last elementary estimate follows by integral comparison with $1/\log t$ and one [integration by parts](../../../../../integration-by-parts.md). The [Riemann–von Mangoldt formula](../../../../../riemann-von-mangoldt-formula.md) would imply

$$
n\le N(\gamma_n)\le\left(\frac c{2\pi}+o(1)\right)n,
$$

a contradiction. This reasoning is valid whether repeated ordinates are listed according to [multiplicity](../../../../../multiplicity-mathematics.md) or only distinct ordinates are listed, since in either case $n\le N(\gamma_n)$. Consequently **$\gamma_{n+1}-\gamma_n>c/\log n$ infinitely often**, for any fixed $0<c<2\pi$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
