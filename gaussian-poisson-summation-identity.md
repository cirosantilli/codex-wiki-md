# Gaussian Poisson summation identity

↑ **Parent:** [Poisson summation formula](poisson-summation-formula.md)

Take the [Gaussian function](gaussian-function.md) $f_a(x)=e^{-\pi ax^2}$ with $a>0$. Every [derivative](derivative.md) is a [polynomial](polynomial-split.md) times the same [Gaussian function](gaussian-function.md), so $f_a$ is a [Schwartz function](schwartz-function.md). The [Fourier transform of a Gaussian](fourier-transform-of-a-gaussian.md) gives, in the cycles convention,

$$
\widehat f_a(\xi)=a^{-1/2}e^{-\pi\xi^2/a}.
$$

Thus the [Poisson summation formula](poisson-summation-formula.md) gives the exact identity

$$
S(a):=\sum_{n\in\mathbb Z}e^{-\pi an^2}
=\frac1{\sqrt a}\sum_{k\in\mathbb Z}e^{-\pi k^2/a}
=\frac1{\sqrt a}S(1/a),\qquad a>0.
$$

The [Gaussian Fourier transform](fourier-transform-of-a-gaussian.md) is given in scaled form in Exercise 41 of [Terence Tao](terence-tao.md)'s _245C, Notes 2: The Fourier transform_.[§3, Exercise 41: transform of a scaled Gaussian; put r=1/sqrt(a) and adjust its prefactor](245c-notes-2-the-fourier-transform-by-terence-tao.md) The identity is also the imaginary-axis transformation of the [Jacobi theta function](jacobi-theta-function.md). At $a=1$ the [Gaussian function](gaussian-function.md) is its own [Fourier transform](fourier-transform-split.md); at reciprocal values of $a$ its spatial and spectral widths exchange.

For a short derivation of the [Gaussian Fourier transform](fourier-transform-of-a-gaussian.md), write $H(\xi)=\widehat f_a(\xi)$. Differentiation under the [integral](integral-split.md) and [integration by parts](integration-by-parts.md), using $f_a'(x)=-2\pi axf_a(x)$, give

$$
H'(\xi)=-2\pi i\int_{\mathbb R}xf_a(x)e^{-2\pi i\xi x}\,dx
=-\frac{2\pi\xi}{a}H(\xi).
$$

The [Gaussian integral](gaussian-integral.md) gives $H(0)=a^{-1/2}$, so this [ordinary differential equation](ordinary-differential-equation.md) yields the claimed formula. The decay of the [Gaussian function](gaussian-function.md) justifies these steps and removes the boundary term.[Lecture 17, §17.1, Lemma 17.9 and proof, printed p. 3: differential-equation proof for the unit Gaussian; scaled here to a\>0](number-theory-i-mit-18-785-fall-2021/lecture-17-the-functional-equation.md)

<a id="image-gaussian-weights-at-integer-physical-and-dual-points-for-reciprocal-parameters-0-04-and-25"></a>
![](poisson-gaussian-physical-dual-weights.png)

**[Figure 3](#image-gaussian-weights-at-integer-physical-and-dual-points-for-reciprocal-parameters-0-04-and-25). Gaussian weights at integer physical and dual points for reciprocal parameters 0.04 and 25**.

For $a=0.04$, the physical [Gaussian function](gaussian-function.md) has width parameter $1/\sqrt a=5$, while its [Fourier transform](fourier-transform-split.md) has width parameter $\sqrt a=0.2$. Many physical samples matter, but the dual zero sample already gives

$$
S(0.04)=5\left(1+2e^{-25\pi}+2e^{-100\pi}+\cdots\right),\qquad
0<S(0.04)-5<7.774\times10^{-34}.
$$

For $a=25$, use the physical side instead:

$$
S(25)=1+2e^{-25\pi}+2e^{-100\pi}+\cdots,\qquad
0<S(25)-1<1.555\times10^{-34}.
$$

These are bounds on the full positive tails, obtained below, rather than estimates based only on the first omitted term. Ordinary floating-point arithmetic rounds these sums to $5$ and $1$; the exact [real numbers](real-number.md) are slightly larger. A [Gaussian sum truncation bound](gaussian-sum-truncation-bound.md) lets us choose the cheaper side and certify its truncation error before evaluating it.

**Table of contents**

- [Gaussian sum truncation bound](gaussian-sum-truncation-bound.md)

## ↑ Ancestors (6)

1. [Poisson summation formula](poisson-summation-formula.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Poisson summation formula for a Euclidean lattice](poisson-summation-formula-for-a-euclidean-lattice.md)
