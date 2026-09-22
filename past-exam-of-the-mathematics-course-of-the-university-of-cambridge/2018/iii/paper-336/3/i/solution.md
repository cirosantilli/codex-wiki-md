<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First remove the small damping term by writing

$$
y=e^{-(1-e^{-2\varepsilon t})/4}v.
$$

The transformed [linear ordinary differential equation](../../../../../../linear-ordinary-differential-equation.md) is

$$
v_{tt}+\left[e^{-2\varepsilon t}+\varepsilon^2e^{-2\varepsilon t}-\frac{\varepsilon^2}{4}e^{-4\varepsilon t}\right]v=0.
$$

The leading frequency is $\omega=e^{-\varepsilon t}$. Its [WKB approximation](../../../../../../wkb-approximation.md) has amplitude $\omega^{-1/2}$ and phase $\int_0^t\omega\,ds=(1-e^{-\varepsilon t})/\varepsilon$. The [initial conditions](../../../../../../initial-condition.md) select

$$
\boxed{y_{\rm WKB}=e^{\varepsilon t/2-(1-e^{-2\varepsilon t})/4}\sin\left(\frac{1-e^{-\varepsilon t}}{\varepsilon}\right).}
$$

This leading expression has $y(0)=0$ and $y_t(0)=1$. Its [WKB approximation for a slowly varying oscillator](../../../../../../wkb-approximation-for-a-slowly-varying-oscillator.md) requires $|\omega_t|/\omega^2=\varepsilon e^{\varepsilon t}\ll1$, so it fails around $t_*=\varepsilon^{-1}\log(\varepsilon^{-1})$.

To resolve the [Bessel transition for an exponentially decaying oscillator](../../../../../../bessel-transition-for-an-exponentially-decaying-oscillator.md), shift to $T=\varepsilon t-\log(\varepsilon^{-1})$, put $Z=e^{-T}$ and rescale $y=\varepsilon^{-1/2}e^{-1/4}Y(T)$. The exact transformed equation is

$$
Y_{TT}+e^{-2T}Y+\varepsilon^2e^{-2T}Y_T=0.
$$

For fixed $T$ its leading form is $Y_{TT}+e^{-2T}Y=0$. The substitution $Z=e^{-T}$ turns it into the order-zero [Bessel differential equation](../../../../../../bessel-differential-equation.md), so $Y=A_0J_0(Z)+B_0Y_0(Z)$. In the overlap $1\ll Z\ll\varepsilon^{-1}$, matching the large-argument [Bessel functions](../../../../../../bessel-function.md) to $Z^{-1/2}\sin(\varepsilon^{-1}-Z)$ gives, with $\theta=\varepsilon^{-1}-\pi/4$,

$$
\boxed{y\sim\varepsilon^{-1/2}e^{-1/4}\sqrt{\frac\pi2}\left[\sin\theta J_0(Z)-\cos\theta Y_0(Z)\right].}
$$

Here $J_0$ and $Y_0$ are the [Bessel function of the first kind](../../../../../../bessel-function-of-the-first-kind.md) and [Bessel function of the second kind](../../../../../../bessel-function-of-the-second-kind.md); the symbol $Y_0(Z)$ in this question is unrelated to the leading inner function in the preceding question.

At late times $T\gg1$, the small-argument expansions give

$$
\boxed{y\sim\varepsilon^{-1/2}e^{-1/4}\sqrt{\frac\pi2}\left[\sin\theta+\frac2\pi\cos\theta\bigl(T+\log2-\gamma\bigr)\right],}
$$

where $\gamma$ is the [Euler--Mascheroni constant](../../../../../../euler-s-constant.md). The solution becomes asymptotically linear rather than maintaining the exponentially growing WKB envelope. Its leading late-time slope is $\varepsilon^{1/2}e^{-1/4}\sqrt{2/\pi}\cos\theta$. These are leading asymptotic coefficients as $\varepsilon\to0$: near a zero of $\cos\theta$, higher-order phase corrections determine the small actual slope. The formula is not an absolute-error estimate uniform to arbitrarily late times. The [exact late slope of an exponentially damped oscillator](../../../../../../exact-late-slope-of-an-exponentially-damped-oscillator.md), obtained from a [Kummer function](../../../../../../confluent-hypergeometric-function-of-the-first-kind.md) and a [Wronskian](../../../../../../wronskian.md), provides a separate check even near those exceptional phases.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
