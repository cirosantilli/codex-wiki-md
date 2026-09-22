<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A [wavelet](../../../../../../wavelet.md) with $p$ [vanishing moments](../../../../../../vanishing-moment.md) satisfies $x^k\psi\in L^1$ and $\int x^k\psi(x)\,dx=0$ for $0\le k<p$. The [moment differentiation of the Fourier transform](../../../../../../moment-differentiation-of-the-fourier-transform.md) theorem states that these weighted integrability hypotheses make $\widehat\psi\in C^{p-1}$, with $\widehat\psi^{(k)}(\xi)=\int(-ix)^k\psi(x)e^{-ix\xi}\,dx$. Hence $\widehat\psi^{(k)}(0)=0$. The [MRA projection Fourier identity](../../../../../../mra-projection-fourier-identity.md), together with density of the approximation spaces and [continuity](../../../../../../continuous-function.md) of $\widehat\varphi$ at zero, gives $|\widehat\varphi(0)|=1$. These are the two analytic theorems needed in addition to the [quadrature mirror filter](../../../../../../quadrature-mirror-filter.md) construction.

For the ordinary [derivative](../../../../../../derivative.md) conclusion, assume also that the [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) is $C^{p-1}$ near $\pi$ and $\widehat\varphi$ is $C^{p-1}$ near zero. These hypotheses hold, for example, for a compactly supported [scaling function](../../../../../../scaling-function.md) with a finite refinement filter. The [wavelet](../../../../../../wavelet.md) identity gives

$$
\overline{m(\pi+t)}=\frac{e^{it}\widehat\psi(2t)}{\widehat\varphi(t)}.
$$

The denominator is nonzero near zero. Its reciprocal and the exponential are $C^{p-1}$, so the [product rule](../../../../../../product-rule.md) and the zero [Taylor polynomial](../../../../../../taylor-polynomial.md) of $\widehat\psi$ give the [smooth-mask vanishing-moment criterion](../../../../../../smooth-mask-vanishing-moment-criterion.md)

$$
\boxed{m^{(k)}(\pi)=0\quad(0\le k<p),\quad\text{under the stated smoothness hypotheses}.}
$$

**The printed integrability hypothesis alone does not guarantee ordinary higher [derivatives](../../../../../../derivative.md).** It gives only a [continuous](../../../../../../continuous-function.md) $\widehat\varphi$. Without added smoothness, [Taylor theorem](../../../../../../taylor-theorem.md) for $\widehat\psi$ still gives $m(\pi+t)=o(|t|^{p-1})$ for the representative defined by the quotient: a [Peano zero](../../../../../../peano-zero.md). This establishes the value at $\pi$, and for $p\ge2$ the first [derivative](../../../../../../derivative.md) there, but it does not automatically establish iterated [derivatives](../../../../../../derivative.md).

Here is a [lacunary scaling-phase regularity counterexample](../../../../../../lacunary-scaling-phase-regularity-counterexample.md) for $p\ge3$. Start with a compactly supported [Daubechies wavelet](../../../../../../daubechies-wavelet.md) having $p$ [vanishing moments](../../../../../../vanishing-moment.md), with [scaling function](../../../../../../scaling-function.md) $\varphi_0$ and finite [MRA low-pass filter](../../../../../../low-pass-filter-of-a-multiresolution-analysis.md) $m_0$. Define the periodic phase

$$
\theta(t)=\sum_{n\ge0}2^{-n}\sin(2^nt),\qquad a(t)=e^{i\theta(t)},\qquad\widehat\varphi(t)=a(t)\widehat\varphi_0(t).
$$

The [Fourier coefficients](../../../../../../fourier-coefficient.md) of $\theta$ are absolutely summable. The [Wiener algebra](../../../../../../wiener-algebra.md) is closed under multiplication and the exponential [series](../../../../../../series-mathematics.md), so $a$ and $a^{-1}$ have absolutely summable [Fourier coefficients](../../../../../../fourier-coefficient.md). Thus $\varphi$ is an absolutely summable combination of [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md) of $\varphi_0$, belongs to $L^1\cap L^2$, and generates the same $V_0$. Unimodularity preserves [orthogonality](../../../../../../orthogonal-vectors.md) and unit [norm](../../../../../../norm.md) of its [integer](../../../../../../integer.md) [function translations](../../../../../../translation-of-a-function.md); the inverse phase preserves their complete span. The same approximation spaces therefore give a [multiresolution analysis](../../../../../../multiresolution-analysis.md).

The identity $\theta(2t)=\theta(t)+\theta(t+\pi)$ gives $a(2t)=a(t)a(t+\pi)$, so the [periodic phase change of a scaling function](../../../../../../periodic-phase-change-of-a-scaling-function.md) produces $m(t)=a(t+\pi)m_0(t)$. In the high-pass formula the phases cancel:

$$
e^{-it}\overline{m(t+\pi)}\widehat\varphi(t)
=e^{-it}\overline{m_0(t+\pi)}\widehat\varphi_0(t).
$$

The associated [wavelet](../../../../../../wavelet.md) is therefore exactly the original one, with unchanged [vanishing moments](../../../../../../vanishing-moment.md).

At any dyadic point $t_0=2\pi k/2^j$, the [difference quotient](../../../../../../difference-quotient.md) of the terms with $j\le n\le\log_2(1/|h|)$ is $1+O((2^nh)^2)$ per term. The sum of these errors and the remaining tail divided by $h$ are bounded; the finitely many earlier terms have finite limits. Hence $(\theta(t_0+h)-\theta(t_0))/h=\log_2(1/|h|)+O(1)$, which has no finite limit. The exponential has the same failure of [differentiability](../../../../../../differentiability.md). Dyadic points are [dense](../../../../../../dense-set.md), and $m_0(\pi+t)$ is nonzero for sufficiently small $t\ne0$. Thus $m$ is not [differentiable](../../../../../../differentiable-function.md) on any neighborhood of $\pi$, so an ordinary second [derivative](../../../../../../derivative.md) at $\pi$, understood as the [derivative](../../../../../../derivative.md) of a locally defined first [derivative](../../../../../../derivative.md), need not exist. The [Peano zero](../../../../../../peano-zero.md) remains valid. This separates the intended smooth-mask theorem from what the literal assumptions establish.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 340](../../../paper-340-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
