# Delay stability of proportional integrator control

↑ **Parent:** [Feedback delay](feedback-delay.md)

For the constant-coefficient model $x'(t)=-kx(t-\tau)$ with $k>0$ and $\tau\ge0$, the zero [equilibrium point](equilibrium-point-of-a-dynamical-system.md) is [asymptotically stable](asymptotic-stability.md) if and only if $k\tau<\pi/2$. For positive $\tau$, perturbations are measured by the [supremum norm](supremum-norm.md) of the [initial history of delayed feedback](initial-history-of-delayed-feedback.md); in the stable regime, every continuous history produces a solution tending to zero. At equality, nondecaying [sinusoids](sinusoid.md) prevent [asymptotic stability](asymptotic-stability.md). For $k\tau>\pi/2$, growing oscillatory solutions exist. These statements concern this ideal [linear time-invariant system](linear-time-invariant-system.md), rather than an arbitrary [controlled plant](plant-control-theory.md). The corresponding linear equation and its threshold are developed in [Cain and Reynolds, section 6.4, pages 174–177](https://math1um.github.io/Teaching/cain-reynolds-odes.pdf#page=179).

Substitute the [exponential function](exponential-function.md) $x(t)=e^{st}$, allowing a [complex number](complex-number.md) $s$. The [characteristic equation](characteristic-equation-of-a-constant-coefficient-differential-equation.md) is

$$
s+k e^{-s\tau}=0.
$$

For positive [feedback delay](feedback-delay.md) this is not a [characteristic polynomial](characteristic-polynomial.md): it has infinitely many roots. A root's [real part](real-part.md) determines growth or decay of its exponential mode, and its [imaginary part](imaginary-part.md) determines the [angular frequency](angular-frequency.md). To find the first boundary, set $s=i\omega$ with $\omega>0$ and use [Euler's formula](euler-s-formula.md):

$$
k\cos(\omega\tau)=0,\qquad \omega-k\sin(\omega\tau)=0.
$$

The smallest positive crossing is $\omega=k$ and $\omega\tau=\pi/2$. Thus at $\tau_c=\pi/(2k)$ the [complex conjugate](complex-conjugate.md) roots are $s=\pm ik$. In fact, with the matching [initial history of delayed feedback](initial-history-of-delayed-feedback.md),

$$
x(t)=A\cos(kt)+B\sin(kt)
$$

solves the [delay differential equation](delay-differential-equation.md) exactly: a quarter-cycle [feedback delay](feedback-delay.md) turns the past displacement into precisely the current [derivative](derivative.md). Its cycle lasts $2\pi/k=4\tau_c$. The amplitude is arbitrary; this linear model does not select a finite-amplitude oscillation.

The roots cross toward growth as [feedback delay](feedback-delay.md) increases. Differentiating the [characteristic equation](characteristic-equation-of-a-constant-coefficient-differential-equation.md) at fixed $k$ gives

$$
\frac{ds}{d\tau}=-\frac{s^2}{1+s\tau},\qquad
\operatorname{Re}\left(\frac{ds}{d\tau}\right)_{s=ik,\,\tau=\tau_c}
=\frac{k^2}{1+(\pi/2)^2}>0.
$$

This calculation identifies the direction of the first destabilization. The full threshold also requires ruling out earlier unstable roots: if $s=\alpha+i\beta$ with $\alpha\ge0$ and $\beta>0$, the [characteristic equation](characteristic-equation-of-a-constant-coefficient-differential-equation.md) implies $\cos(\beta\tau)\le0$ and $0<\beta\le k$, hence $k\tau\ge\beta\tau\ge\pi/2$. A real nonnegative root is impossible because $s+k e^{-s\tau}>0$ there. This supplies the geometric reason the threshold is a quarter-cycle rather than an arbitrary fitting constant.

<a id="image-feedback-delay-separates-decay-persistent-oscillation-and-growth"></a>
![](feedback-delay-gain-stability.png)

**[Figure 8](#image-feedback-delay-separates-decay-persistent-oscillation-and-growth). Feedback delay separates decay, persistent oscillation, and growth**. Left: numerical solutions with the same constant [initial history of delayed feedback](initial-history-of-delayed-feedback.md) $x=1$ on $[-\tau,0]$, plotted against $q=t/\tau$ for $k\tau=0.8$, $\pi/2$, and $2$. The middle trajectory includes a transient because this history is not a pure [sinusoid](sinusoid.md); the dashed curve is a separate exact solution with history $\cos(\pi q/2)$. Each row has its own vertical scale. Right: the exact boundary $k=\pi/(2\tau)$ for positive [feedback gain](feedback-gain.md) and [feedback delay](feedback-delay.md). Toy responses are not measured data. The generator uses the [classical fourth-order Runge-Kutta method](classical-fourth-order-runge-kutta-method.md) with [linear interpolation](linear-interpolation.md) of delayed values and $\Delta q=1/2000$, checked against a separately evaluated exact finite sum and two coarser steps.

The tradeoff is concrete. Without [feedback delay](feedback-delay.md), increasing $k$ shortens the [exponential decay](exponential-decay.md) [time constant](time-constant.md) $1/k$. With known $\tau>0$, the same [proportional control](proportional-control.md) must satisfy $k<\pi/(2\tau)$. For $\tau=0.2\,\mathrm{s}$, the threshold is $k\approx7.854\,\mathrm{s}^{-1}$: $k=5\,\mathrm{s}^{-1}$ is stable and $k=8\,\mathrm{s}^{-1}$ is unstable. A design close to the boundary leaves little room for additional [feedback delay](feedback-delay.md); reducing $k$ or reducing measurement latency increases that room. The zero-delay [time constant](time-constant.md) is only a comparison scale, not the decay time of the delayed response. Frank discusses the gain–delay compromise in [Control Theory Tutorial, section 13.4 and figure 13.3](https://stevefrank.org/control/controlBook.pdf#page=101).

## ↑ Ancestors (6)

1. [Feedback delay](feedback-delay.md)
2. [Closed-loop control](closed-loop-control.md)
3. [Control theory](control-theory-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Feedback delay](feedback-delay.md)
