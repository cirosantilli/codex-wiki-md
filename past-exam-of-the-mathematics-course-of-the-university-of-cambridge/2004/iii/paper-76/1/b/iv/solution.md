<h1 id="1/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Write $K_0(z)=-F(z)\log z+G(z)$ locally, with analytic $F,G$ and $F(0)=1$. The coefficient of $\log z$ in the [Modified Bessel differential equation](../../../../../../../modified-bessel-differential-equation.md) requires $z^2F''+zF'-z^2F=0$. If $F=\sum a_mz^m$, its recurrence is $m^2a_m=a_{m-2}$, with $a_1=0$. Hence

$$
F(z)=1+\frac{z^2}{4}+O(z^4),\qquad
K_0(|x|)=-\log|x|-\frac{x^2}{4}\log|x|+G(|x|)+O(x^4\log|x|).
$$

The analytic part is even: an odd-power term in $G$ would produce an uncancelled odd-power term under the same differential operator, and the recurrence removes all such terms. Insert a smooth even cutoff equal to one near zero. The smooth part and the exponentially decaying tails give no algebraic large-[wavenumber](../../../../../../../wavenumber.md) terms after repeated [integration by parts](../../../../../../../integration-by-parts.md). Therefore the [logarithmic singularities](../../../../../../../logarithmic-singularity.md) determine the requested terms. For $k\ne0$,

$$
\mathcal F(\log|x|)=-\frac\pi{|k|},\qquad
\mathcal F(x^2\log|x|)=-\frac{d^2}{dk^2}\left(-\frac\pi{|k|}\right)=\frac{2\pi}{|k|^3}.
$$

Thus the [Fourier transform of the modified Bessel function K0](../../../../../../../fourier-transform-of-the-modified-bessel-function-k0.md) has expansion

$$
\boxed{\widehat{K_0(|x|)}(k)=\frac\pi{|k|}-\frac\pi{2|k|^3}+O(|k|^{-5})}.
$$

An independent check follows from the [integral representation of the modified Bessel function of the second kind](../../../../../../../integral-representation-of-the-modified-bessel-function-of-the-second-kind.md). Integrating $e^{-|x|\cosh t}$ first and then setting $u=\sinh t$ gives $2\int_0^\infty du/(u^2+1+k^2)=\pi/\sqrt{1+k^2}$, with exactly these first two terms.

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 76](../../../../paper-76-split.md)
5. [Iii](../../../../split.md)
6. [2004](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
