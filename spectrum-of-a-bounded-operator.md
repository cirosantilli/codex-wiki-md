# Spectrum of a bounded operator

↑ **Parent:** [Spectrum (functional analysis)](spectrum-functional-analysis.md)

Let $X\ne\{0\}$ be a [Banach space](banach-space-split.md) over the [complex numbers](complex-number.md), and let $T:X\to X$ be a [bounded linear operator](continuous-linear-operator.md) defined on all of $X$. Its [spectrum](spectrum-functional-analysis.md) consists of those $\lambda\in\mathbb C$ for which $T-\lambda I$ has no everywhere-defined [bounded inverse](bounded-inverse.md). Its complement is the [resolvent set of an operator](resolvent-set-of-an-operator.md) $\rho(T)$. By the [bounded inverse theorem](bounded-inverse-theorem.md), a bijective $T-\lambda I$ automatically has a [bounded inverse](bounded-inverse.md). The [spectrum](spectrum-functional-analysis.md) is a nonempty [compact subset](compact-space.md) of the [complex plane](complex-plane.md), with

$$
\sigma(T)\subseteq\{\lambda\in\mathbb C:|\lambda|\leq\|T\|\}.
$$

The bound uses the [operator norm](operator-norm.md), and nonemptiness uses the complex [field](field.md).[HKUST Math 4063 notes, chapter 4, section 3: compactness and nonemptiness of the spectrum](https://www.math.hkust.edu.hk/~makyli/4063/fanotes2_150615.pdf#page=38) For a real [linear operator](linear-operator.md), complex spectral values are understood by extending it to a complex [vector space](vector-space-split.md); restricting $\lambda$ to the real [field](field.md) can give an empty set.

In a [finite-dimensional vector space](finite-dimensional-vector-space.md), failure of inversion forces a nonzero [kernel](kernel-of-a-linear-map-split.md), hence an [eigenvector](eigenvector.md). An [infinite-dimensional vector space](infinite-dimensional-vector-space.md) allows an [injective](injective-function.md) shifted [linear operator](linear-operator.md) that cannot solve every equation $(T-\lambda I)u=g$. The [spectrum](spectrum-functional-analysis.md) therefore records both exact [eigenvectors](eigenvector.md) and failures of solvability or stable inversion. Searching only for [eigenvalues](eigenvalue.md) can miss every spectral value of a perfectly simple [bounded linear operator](continuous-linear-operator.md).

Consider the [multiplication operator](multiplication-operator.md) $M$ on the complex [L2 space](l2-space-is-a-hilbert-space.md) $L^2([0,1],dx)$, with [Lebesgue measure](lebesgue-measure.md):

$$
(Mf)(x)=xf(x),\qquad \|f\|_2^2=\int_0^1|f(x)|^2\,dx.
$$

Its [operator norm](operator-norm.md) is one. The inequality $\|Mf\|_2\leq\|f\|_2$ gives the upper bound; [unit vectors](unit-vector.md) concentrated near $x=1$ approach it. The result is

$$
\sigma(M)=[0,1],\qquad \sigma_p(M)=\varnothing.
$$

This is the interval example of the general connection between [multiplication operators](multiplication-operator.md) and the [essential range](essential-range.md) of their multiplier.[Berkeley Math 224A, lecture 13: spectra of multiplication operators](https://hackmd.io/@knikct/BkX1s2PFr) Indeed, an [eigenfunction](eigenfunction.md) would satisfy $(x-\lambda)f(x)=0$ [almost everywhere](almost-everywhere.md). It vanishes except possibly on the singleton $\{\lambda\}$, a [null set](null-set.md); such a function is the zero vector in [L2 space](l2-space-is-a-hilbert-space.md). Concentrating at one point cannot produce a nonzero [L2 function](square-integrable-function.md).

For $\lambda\notin[0,1]$, the inverse is completely explicit:

$$
((M-\lambda I)^{-1}g)(x)=\frac{g(x)}{x-\lambda},\qquad
\|(M-\lambda I)^{-1}\|=\frac1{\operatorname{dist}(\lambda,[0,1])}.
$$

The [distance to a set](distance-to-a-set.md) is positive, so the inverse multiplier is bounded. Its [essential supremum](essential-supremum.md) gives the displayed [operator norm](operator-norm.md); arbitrarily small intervals near a closest point approach the bound. Our [resolvent of an operator](resolvent-of-an-operator.md) uses $(\lambda I-M)^{-1}$, the negative of this inverse, with the same [operator norm](operator-norm.md). For $\lambda=-1/4$, $5/4$, and $1/2+i/10$, the inverse norms are respectively $4$, $4$, and $10$. The last parameter lies directly above the middle of the [spectrum](spectrum-functional-analysis.md) in the [complex plane](complex-plane.md).

This calculation gives the [spectrum](spectrum-functional-analysis.md) a practical meaning: it marks where solving a shifted equation loses uniform control. At $\lambda=1/2+i\eta$, the largest amplification of an input error is $1/|\eta|$. Changing $\eta$ from $0.1$ to $0.01$ increases that factor from ten to one hundred. The equation remains uniquely solvable for each nonzero $\eta$, but its sensitivity grows as the parameter approaches the [spectrum](spectrum-functional-analysis.md).

<a id="image-an-interval-without-eigenvectors-and-a-diagonal-spectrum-accumulating-at-zero"></a>
![](operator-spectrum-examples.png)

**[Figure 1](#image-an-interval-without-eigenvectors-and-a-diagonal-spectrum-accumulating-at-zero). An interval without eigenvectors and a diagonal spectrum accumulating at zero**.

To see directly why every $\lambda\in[0,1]$ belongs to the [spectrum](spectrum-functional-analysis.md), choose $0<\varepsilon<1$ and define a clipped interval and a normalized [indicator function](indicator-function.md):

$$
a=\max(0,\lambda-\varepsilon),\quad b=\min(1,\lambda+\varepsilon),\quad
\ell=b-a,\qquad u_{\lambda,\varepsilon}(x)=\ell^{-1/2}\mathbf1_{[a,b]}(x).
$$

Its [L2 norm](l2-norm.md) is exactly one, including at both endpoints. On its [support](support.md), $|x-\lambda|\leq\varepsilon$, giving

$$
\|(M-\lambda I)u_{\lambda,\varepsilon}\|_2^2
=\frac{(b-\lambda)^3-(a-\lambda)^3}{3\ell}
\leq\varepsilon^2.
$$

Thus any choice $\varepsilon_n\to0$ produces [approximate eigenvectors](approximate-eigenvector.md). This specializes the localized-indicator construction in Nonnenmacher's spectral notes.[Nonnenmacher, Introduction to Spectral Theory (2021), proposition 4.2.15](https://www.imo.universite-paris-saclay.fr/~nonnenma/enseign/Spectral%20Theory%202021%20chap1-4.pdf#page=47) A hypothetical [bounded inverse](bounded-inverse.md) $B$ would imply $1=\|u_{\lambda,\varepsilon}\|_2\leq\|B\|\varepsilon$, impossible for arbitrarily small $\varepsilon$.

For an interior point with $\varepsilon\leq\min(\lambda,1-\lambda)$, $\ell=2\varepsilon$ and the residual is exactly $\varepsilon/\sqrt3$. At $\lambda=0$ or $1$, $\ell=\varepsilon$ and the same residual formula holds, but the amplitude is $\varepsilon^{-1/2}$ rather than $(2\varepsilon)^{-1/2}$. At $\lambda=1/2$, taking $\varepsilon=0.2,0.1,0.05$ gives amplitudes approximately $1.5811,2.2361,3.1623$ and residuals $0.11547,0.057735,0.028868$. The narrowing [support](support.md) and increasing amplitude keep total squared mass equal to one.

For every $\lambda\in[0,1]$, the [continuous spectrum](continuous-spectrum.md) description is also concrete. Any [L2 function](square-integrable-function.md) $g$ can be approximated in [L2 norm](l2-norm.md) by its truncations to $|x-\lambda|\geq\delta$. Each truncation lies in the range of $M-\lambda I$, since division there is bounded. The range is therefore dense. However, the constant function $g=1$ has no [L2 function](square-integrable-function.md) preimage: $1/(x-\lambda)$ is not square-integrable, including at the endpoints.

These [approximate eigenvectors](approximate-eigenvector.md) do not approach an [eigenvector](eigenvector.md) in [L2 norm](l2-norm.md). Any possible limit would have [L2 norm](l2-norm.md) one and satisfy $(M-\lambda I)u=0$ by [continuity](continuous-function.md), contradicting the empty [point spectrum](point-spectrum.md). This is the striking feature: the [linear operator](linear-operator.md) acts increasingly like [scalar multiplication](scalar-multiplication.md) on suitable [unit vectors](unit-vector.md), although no direction realizes that scaling exactly.

<a id="image-unit-l2-vectors-concentrate-while-their-spectral-residual-tends-to-zero"></a>
![](approximate-spectral-vectors.png)

**[Figure 2](#image-unit-l2-vectors-concentrate-while-their-spectral-residual-tends-to-zero). Unit L2 vectors concentrate while their spectral residual tends to zero**.

A complementary example is the [diagonal operator on sequence space](diagonal-operator-on-sequence-space.md) $(Dx)_n=x_n/n$ on complex [l2 sequence space](l2-sequence-space.md), with $n=1,2,\ldots$. The coordinate [unit vectors](unit-vector.md) satisfy $De_n=(1/n)e_n$, so

$$
\sigma_p(D)=\{1/n:n\geq1\},\qquad
\sigma(D)=\{0\}\cup\{1/n:n\geq1\}.
$$

Zero is not an [eigenvalue](eigenvalue.md), since $Dx=0$ forces every coordinate to vanish. Nevertheless $\|De_n\|=1/n\to0$: these are [approximate eigenvectors](approximate-eigenvector.md) at zero. More concretely, $g=(1/n)_{n\geq1}$ belongs to [l2 sequence space](l2-sequence-space.md), but $Dx=g$ would require $x_n=1$ for all $n$, which does not. Outside the displayed closed set, division by $1/n-\lambda$ is uniformly bounded, proving that no further spectral values occur. Thus the [spectrum](spectrum-functional-analysis.md) contains the missing limit of genuine [eigenvalues](eigenvalue.md), even when that limit has no [eigenvector](eigenvector.md).

## ↑ Ancestors (7)

1. [Spectrum (functional analysis)](spectrum-functional-analysis.md)
2. [Operator theory](linear-operator-theory-split.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (15)

- [Approximate point spectrum](approximate-point-spectrum.md)
- [Essential spectrum of a bounded self-adjoint operator](essential-spectrum-of-a-bounded-self-adjoint-operator.md)
- [Operator theory](linear-operator-theory-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ii/paper-4/22h/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-3/21g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-7/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/2/10/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/2/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-5/2/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/21f/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-358/1/a/solution.md)
- [Point spectrum](point-spectrum.md)
- [Residual spectrum](residual-spectrum.md)
- [Spectral Weyl sequence](spectral-weyl-sequence.md)
