# Wavelet polynomial annihilation

↑ **Parent:** [Vanishing moment](vanishing-moment.md)

For $a>0$ and $b\in\mathbb R$, define the shifted, scaled analyzing [function](function-split.md) and its coefficient by

$$
\psi_{a,b}(x)=a^{-1/2}\psi\!\left(\frac{x-b}{a}\right),\qquad c_\psi(f;a,b)=\int_{\mathbb R}f(x)\overline{\psi_{a,b}(x)}\,dx=\sqrt a\int_{\mathbb R}f(b+au)\overline{\psi(u)}\,du.
$$

Assume the product is [integrable](integrability.md); for example this holds for a [locally integrable function](locally-integrable-function.md) $f$ and a bounded analyzing [function](function-split.md) with [compact support](compact-support.md). The bar is [complex conjugation](complex-conjugation.md). This normalization preserves the [L2 norm](l2-norm.md) of the analyzing [function](function-split.md). If $p$ is a [polynomial](polynomial-split.md) of [degree of a polynomial](degree-of-a-polynomial.md) less than $q$, then $p(b+au)$ is a sum of [monomials](monomial.md) $u^r$ with $r<q$. [Linearity of integration](linearity-of-integration.md) and the [vanishing moments](vanishing-moment.md) give $c_\psi(p;a,b)=0$ at every position and scale. Nonzero [polynomials](polynomial-split.md) on the whole [real line](real-line.md) are not [square-integrable](square-integrable-function.md), so this cancellation is an [integral](integral-split.md) pairing; it is not a claim that these [polynomials](polynomial-split.md) are vectors of $L^2(\mathbb R)$.

Here is a quantitative reason that [smooth](smooth-function.md) regions yield small details. Let $ψ$ have [compact support](compact-support.md) and $q$ [vanishing moments](vanishing-moment.md), and suppose $f$ is $q$ times [continuously differentiable](continuously-differentiable-function.md) on an [interval](interval-mathematics.md) containing $b$ and $b+a\operatorname{supp}\psi$. Subtract its degree-$(q-1)$ [Taylor polynomial](taylor-polynomial.md) at $b$. If $|f^{(q)}|\leq M$ on that [interval](interval-mathematics.md), the [Taylor remainder](taylor-remainder.md) bound gives

$$
|c_\psi(f;a,b)|\leq\frac{M}{q!}a^{q+1/2}\int_{\mathbb R}|u|^q|\psi(u)|\,du.
$$

The factor $a^q$ comes from the [Taylor remainder](taylor-remainder.md); $a^{1/2}$ comes from the coefficient normalization. Thus the analyzing [function](function-split.md) measures the departure from the local [polynomial](polynomial-split.md) trend, rather than the height of $f$ itself. The [wavelet coefficient decay for Hölder functions](wavelet-coefficient-decay-for-holder-functions.md) uses the same argument with a [Hölder-Taylor remainder bound](holder-taylor-remainder-bound.md). These estimates concern regularity of $f$ on the analyzing [function](function-split.md)'s entire [support of a function](support.md); extra [vanishing moments](vanishing-moment.md) alone do not make $ψ$ [smooth](smooth-function.md) or establish an [orthonormal wavelet](orthonormal-wavelet.md) construction.[Wavelet Zoom, §6.1.1, printed p. 141, equations (6.1)–(6.2); §6.1.2, printed p. 143, Polynomial Suppression, equations (6.6)–(6.8)](a-wavelet-tour-of-signal-processing-by-stephane-mallat/wavelet-zoom.md)

## ↑ Ancestors (7)

1. [Vanishing moment](vanishing-moment.md)
2. [Wavelet](wavelet.md)
3. [Fourier analysis](fourier-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
