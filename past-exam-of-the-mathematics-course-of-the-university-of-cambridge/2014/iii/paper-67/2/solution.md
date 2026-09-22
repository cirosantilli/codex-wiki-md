<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For $u\in\mathcal E'$, choose a [cutoff function](../../../../../cutoff-function.md) $\chi=1$ on a neighborhood of its support. Its extension to [smooth functions](../../../../../smooth-function.md) makes

$$
F(z)=\langle u_x,\chi(x)e^{-iz\cdot x}\rangle
$$

independent of the choice of cutoff. For real frequency, the definition of the [distributional Fourier transform](../../../../../fourier-transform-of-a-tempered-distribution.md) gives $F(\lambda)=\widehat u(\lambda)$: interchange the pairing with the integral of a [Schwartz function](../../../../../schwartz-function.md), using the finite-order estimate on the cutoff's [compact support](../../../../../compact-support.md). On each compact set of complex frequencies the exponential and all its $x$ derivatives have uniformly convergent power series. Continuity of the [distribution](../../../../../distribution-mathematical-analysis.md) allows termwise differentiation, with

$$
\partial_z^\alpha F(z)=\langle u_x,(-ix)^\alpha e^{-iz\cdot x}\rangle.
$$

Consequently **$F$ is entire on $\mathbb C^n$**.

For the precise exponential type, a fixed enlarged support would give an unnecessarily enlarged radius. Instead use the [shrinking-cutoff exponential-type estimate](../../../../../shrinking-cutoff-exponential-type-estimate.md). On one fixed compact neighborhood of the closed radius-$\delta$ ball, $u$ has finite [order of a distribution](../../../../../order-of-a-distribution.md) $m$. Choose $\chi_\varepsilon=1$ near that ball, supported in the radius-$(\delta+\varepsilon)$ ball, with $|\partial^\alpha\chi_\varepsilon|\le C_\alpha\varepsilon^{-|\alpha|}$ for $0<\varepsilon\le1/2$. The finite-order estimate gives

$$
|F(z)|\le C\varepsilon^{-m}(1+|z|)^m
 e^{(\delta+\varepsilon)|\operatorname{Im}z|}.
$$

Take $\varepsilon=[2(1+|z|)]^{-1}$. Its extra exponential is bounded by $e^{1/2}$, while the derivative cost is [polynomial](../../../../../polynomial-split.md). Thus

$$
\boxed{|\widehat u(z)|\le C'(1+|z|)^{2m}e^{\delta|\operatorname{Im}z|}.}
$$

The entire function was defined with a fixed cutoff; only its bound uses a frequency-dependent cutoff, so no holomorphic dependence is lost. This proves the required estimate with some $N\ge0$ without enlarging $\delta$.

For the converse, set $V(z)=e^{iz\cdot y}U(z)$. Its restriction to real frequencies has [polynomial growth](../../../../../polynomial-growth.md). Define the inverse [tempered distribution](../../../../../tempered-distribution.md) $v$ by

$$
\langle v,\phi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}V(\xi)\widehat\phi(-\xi)\,d\xi,
\qquad\phi\in\mathcal S.
$$

Rapid decay of the [Schwartz function](../../../../../schwartz-function.md) transform proves convergence and continuity, and [Fourier inversion](../../../../../fourier-inversion-theorem.md) gives $\widehat v=V$ on real frequencies.

We prove its support directly by [contour shifting](../../../../../contour-shifting.md), rather than assuming the support conclusion of the [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md). Let $\omega$ be a real unit vector and take a [test function](../../../../../test-function.md) $\phi$ supported in $x\cdot\omega\ge\delta+\epsilon$ for some $\epsilon>0$. For every integer $M\ge0$, [integration by parts](../../../../../integration-by-parts.md) in the real-frequency Fourier integral gives

$$
\begin{aligned}
\widehat\phi(-\xi-it\omega)
&=\int e^{i\xi\cdot x}e^{-t\omega\cdot x}\phi(x)\,dx,\\
|\widehat\phi(-\xi-it\omega)|
&\le C_M(1+t)^{2M}(1+|\xi|^2)^{-M}
 e^{-t(\delta+\epsilon)},\qquad t\ge0.
\end{aligned}
$$

Indeed, move $(1-\Delta_x)^M$ from the oscillatory exponential to $e^{-t\omega\cdot x}\phi$; its derivatives supply at most $2M$ powers of $t$.

The product $V(z)\widehat\phi(-z)$ is entire. Rotate coordinates so that $\omega$ is the first coordinate vector and apply [Cauchy integral theorem](../../../../../cauchy-s-integral-theorem.md) to a rectangle in that one complex coordinate, integrating the remaining real coordinates afterwards. For fixed $t$, choose $2M>N+n+2$; the displayed decay estimate, uniformly on the intervening imaginary segment, makes the vertical faces vanish as the real rectangle width tends to infinity. The horizontal integrals are absolutely convergent. Hence

$$
\langle v,\phi\rangle=(2\pi)^{-n}\int_{\mathbb R^n}
 V(\xi+it\omega)\widehat\phi(-\xi-it\omega)\,d\xi.
$$

Using $(1+|\xi+it\omega|)^N\le C(1+t)^N(1+|\xi|)^N$ and the growth hypothesis bounds this pairing by

$$
C'(1+t)^{N+2M}e^{-\epsilon t}
\int_{\mathbb R^n}(1+|\xi|)^N(1+|\xi|^2)^{-M}\,d\xi.
$$

It tends to zero as $t\to\infty$, so the pairing vanishes. Every point outside the closed radius-$\delta$ ball lies in such a separating half-space; a finite [partition of unity](../../../../../partition-of-unity.md) for the support of a [test function](../../../../../test-function.md) outside the ball proves $\operatorname{supp}v\subset\overline B(0,\delta)$.

Translate this [compactly supported distribution](../../../../../compactly-supported-distribution.md) by $y$: define $\langle u,\phi\rangle=\langle v,\phi(\cdot+y)\rangle$. The [Translation property of the Fourier transform](../../../../../translation-property-of-the-fourier-transform.md) gives

$$
\widehat u(\xi)=e^{-i\xi\cdot y}V(\xi)=U(\xi),
\qquad\boxed{\operatorname{supp}u\subset\overline B(y,\delta).}
$$

The compact-support entire extension agrees with $U$ everywhere by the [identity theorem](../../../../../identity-theorem.md), applied successively in the complex coordinates. [Fourier inversion](../../../../../fourier-inversion-theorem.md) also gives uniqueness. This completes both directions of the ball version of the [Paley–Wiener–Schwartz theorem](../../../../../paley-wiener-schwartz-theorem.md).

For the [wave equation](../../../../../wave-equation-split.md), take a real constant $c\ne0$. The [Fourier transform method for the wave equation](../../../../../fourier-transform-method-for-the-wave-equation.md) gives

$$
\partial_t^2\widehat E_t(\xi)+c^2|\xi|^2\widehat E_t(\xi)=0,
\qquad\boxed{\widehat E_t(\xi)=\cos(ct|\xi|)\widehat f(\xi).}
$$

This inverse [tempered distribution](../../../../../tempered-distribution.md) is twice differentiable in $t$: time derivatives introduce [polynomial](../../../../../polynomial-split.md) frequency factors, still integrable against every [Schwartz function](../../../../../schwartz-function.md). It has the specified initial displacement and zero initial velocity and satisfies the equation distributionally.

To apply the support theorem, replace the real norm by the [entire wave cosine multiplier](../../../../../entire-wave-cosine-multiplier.md)

$$
C_t(z)=\sum_{j=0}^\infty\frac{(-1)^j(ct)^{2j}(z\cdot z)^j}{(2j)!}.
$$

This series is entire and equals $\cos(ct\sqrt{z\cdot z})$ regardless of the square-root choice. Write $z=a+ib$ and $q=\sqrt{z\cdot z}$. Since $|z\cdot z|\le|a|^2+|b|^2$,

$$
(\operatorname{Im}q)^2
=\frac{|z\cdot z|-(|a|^2-|b|^2)}2\le|b|^2.
$$

Together with $|\cos w|\le e^{|\operatorname{Im}w|}$, this yields $|C_t(z)|\le e^{|c|t|\operatorname{Im}z|}$. The forward estimate for the translated initial support now gives

$$
|e^{iz\cdot y}C_t(z)\widehat f(z)|
\le C(1+|z|)^N e^{(\delta+|c|t)|\operatorname{Im}z|}.
$$

The converse therefore proves **finite propagation with the stated speed**:

$$
\boxed{\operatorname{supp}E_t\subset\overline B(y,\delta+|c|t),\qquad t>0.}
$$

In particular, $\sqrt{z\cdot z}$ itself need not be entire; it is the even cosine series that provides the required entire extension.

For completeness this construction identifies the distributional Cauchy solution even without initially assuming spatial temperedness. The zero-displacement wave multiplier is $S_\tau(z)=\int_0^\tau C_s(z)\,ds$, entire with bound $|S_\tau(z)|\le\tau e^{|c|\tau|\operatorname{Im}z|}$. Given a compactly supported smooth $\phi$ and final time $T$, the backward solution $w(s)=\mathcal F^{-1}[S_{T-s}\widehat\phi]$ is smooth, has support in one compact ball for $0\le s\le T$ by the same support theorem, and satisfies $w(T)=0$, $w_s(T)=-\phi$. For the difference $h$ of two distributional solutions with zero initial data,

$$
\frac d{ds}\big(\langle h_s,w\rangle-\langle h,w_s\rangle\big)
=c^2\big(\langle\Delta h,w\rangle-\langle h,\Delta w\rangle\big)=0.
$$

All pairings use compactly supported [test functions](../../../../../test-function.md). The expression vanishes initially and equals $\langle h(T),\phi\rangle$ finally. Hence $h(T)=0$, establishing uniqueness in the usual time-differentiable distributional solution class.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 67](../../paper-67-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
