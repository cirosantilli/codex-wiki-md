<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Write $T=\varepsilon t$ and $q(T)=2e^{-T}$. The forcing acts on the fast initial-time scale, so first remove a localized particular solution. Expanding the coefficient there gives

$$
u_p=e^{-2t}+\varepsilon p_1(t)+\cdots,
\qquad p_1''+4p_1=8t e^{-2t}.
$$

A particular choice is $p_1=(t+1/2)e^{-2t}$, hence

$$
u_p=e^{-2t}[1+\varepsilon(t+1/2)]+O(\varepsilon^2).
$$

Its initial value is $1+\varepsilon/2$ and its initial [derivative](../../../../../derivative.md) is $-2+O(\varepsilon^2)$. The [localized forcing determines WKB phase constants](../../../../../localized-forcing-determines-wkb-phase-constants.md); omitting it before imposing the [initial conditions](../../../../../initial-condition.md) would miss the permanent free oscillation.

For the homogeneous part, the slow-time equation is $\varepsilon^2u_{TT}+q^2u=0$. Write its [WKB approximation](../../../../../wkb-approximation.md) as $A(T)[C\cos\Phi+B\sin\Phi]$, normalizing $A(0)=1$. The leading amplitude transport equation gives $A=e^{T/2}$ and leading phase $\varepsilon^{-1}\int_0^Tq(s)\,ds=2(1-e^{-T})/\varepsilon$.

To include every $O(\varepsilon)$ contribution on bounded slow-time intervals, the first phase correction is needed. If the local phase wavenumber is $q+\varepsilon^2q_2$, the real part of the amplitude-phase equation gives $q_2=A_{TT}/(2qA)=e^T/16$. The [WKB phase correction for a slowly varying oscillator](../../../../../wkb-phase-correction-for-a-slowly-varying-oscillator.md), anchored to zero at the initial time, is therefore

$$
\boxed{\Phi(t)=\frac2\varepsilon(1-e^{-\varepsilon t})
+\frac\varepsilon{16}(e^{\varepsilon t}-1)}.
$$

There is no first-order bulk amplitude correction in this normalization. At $t=0$, the homogeneous initial value must be $-\varepsilon/2+O(\varepsilon^2)$ and its initial [derivative](../../../../../derivative.md) $1+O(\varepsilon^2)$. Since $A'_t(0)=\varepsilon/2$ and $\Phi'_t(0)=2+O(\varepsilon^2)$, these give $C=-\varepsilon/2+O(\varepsilon^2)$ and $B=1/2+O(\varepsilon^2)$. The requested forced approximation is

$$
\boxed{u(t)=e^{-2t}[1+\varepsilon(t+1/2)]
+e^{\varepsilon t/2}\left[\frac12\sin\Phi(t)-\frac\varepsilon2\cos\Phi(t)\right]
+O(\varepsilon^2)}
$$

for $0\le\varepsilon t\le T_0$ with fixed $T_0$. The approximate initial value is exactly one through this order and its [derivative](../../../../../derivative.md) is $-1+O(\varepsilon^2)$. The particular-solution residual is uniformly localized and $O(\varepsilon^2)$; the corrected homogeneous residual is $O(\varepsilon^3)$ on the long interval, producing $O(\varepsilon^2)$ solution error after integration over times of order $\varepsilon^{-1}$.

The [WKB approximation](../../../../../wkb-approximation.md) requires the relative frequency-change parameter

$$
\frac{|\dot q|}{q^2}=\frac\varepsilon2e^{\varepsilon t}\ll1.
$$

It therefore fails when $\varepsilon e^{\varepsilon t}=O(1)$, even though the coefficient has no finite-time zero. This is the [Bessel transition for an exponentially decaying oscillator](../../../../../bessel-transition-for-an-exponentially-decaying-oscillator.md). Introduce the shifted slow time and amplitude

$$
\boxed{\tau=\varepsilon t-\log(\varepsilon^{-1}),\qquad
u(t)=\varepsilon^{-1/2}U(\tau)}.
$$

The exact rescaled equation is

$$
U_{\tau\tau}+4e^{-2\tau}U
=8\varepsilon^{-3/2}
\exp\left[-\frac2\varepsilon\bigl(\log(\varepsilon^{-1})+\tau\bigr)\right].
$$

For fixed $\tau$ its right side is smaller than every algebraic power of $\varepsilon$. The leading transition problem is consequently

$$
\boxed{U_{0,\tau\tau}+4e^{-2\tau}U_0=0}.
$$

With $Z=2e^{-\tau}$ this becomes $Z^2U_{0,ZZ}+ZU_{0,Z}+Z^2U_0=0$, the order-zero [Bessel differential equation](../../../../../bessel-differential-equation.md). This identifies the governing equation without solving it.

The amplitude-phase series also supplies overlap data while $\varepsilon e^T\ll1$, although its bounded-$T$ absolute error estimate is not uniform up to the transition. For matching, combine the earlier sine and cosine terms into $\tfrac12\sin(\Phi-\varepsilon)$ through first order. In the overlap $\varepsilon\ll e^\tau\ll1$, their phase is

$$
\Phi-\varepsilon=\alpha_\varepsilon-2e^{-\tau}+\frac{e^\tau}{16},
\qquad\alpha_\varepsilon=\frac2\varepsilon-\frac{17\varepsilon}{16}
$$

to the retained order. Thus amplitude and phase matching as $\tau\to-\infty$ require

$$
\boxed{U_0\sim\frac12e^{\tau/2}\sin(\alpha_\varepsilon-2e^{-\tau}),
\qquad U_{0,\tau}\sim e^{-\tau/2}\cos(\alpha_\varepsilon-2e^{-\tau})}.
$$

These are oscillatory amplitude-phase conditions, rather than pointwise ratio statements at zeros. The smaller $e^\tau/16$ phase term records the first overlap correction if required. The rapidly varying matching constant $\alpha_\varepsilon$ must be retained as data; there is no single epsilon-independent limiting phase. The two matching conditions determine the leading transition solution, which is deliberately left unsolved.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
