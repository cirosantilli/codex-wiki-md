# Delayed negative feedback model

↑ **Parent:** [Negative feedback](negative-feedback.md)

A [feedback delay](feedback-delay.md) is a time interval between an event and its returning influence. Multiple biochemical steps can introduce an effective lag; a fixed delay is an idealization, not a universal description of [signal transduction](signal-transduction-split.md). To isolate timing, let $x$ be a signed displacement from an [equilibrium point](equilibrium-point-of-a-dynamical-system.md) and use normalized [dimensionless variables](dimensionless-variable.md):

$$
\frac{dx}{dt}=-x(t)-2x(t-d),\qquad d\geq0.
$$

The local removal is $-x$ and the returning influence is negative at every delay. At $d=0$ the [ordinary differential equation](ordinary-differential-equation.md) reduces to the decay already illustrated under [signaling feedback](signaling-feedback.md). For $d>0$ a [delay differential equation](delay-differential-equation.md) requires a history on $[-d,0]$, not just an [initial condition](initial-condition.md) at one instant. Negative values of $x$ are displacements, not negative chemical [concentrations](concentration.md).

An [exponential function](exponential-function.md) $x=e^{\lambda t}$ gives the [characteristic equation of a delay differential equation](characteristic-equation-of-a-delay-differential-equation.md)

$$
\lambda+1+2e^{-\lambda d}=0.
$$

Putting $\lambda=i\omega$ and equating real and imaginary parts gives $\cos(\omega d)=-1/2$ and $\omega=2\sin(\omega d)$. The first crossing with $\omega>0$ therefore occurs at

$$
\omega=\sqrt3,\qquad d_c=\frac{2\pi}{3\sqrt3}\simeq1.20920.
$$

For this particular [mathematical model](mathematical-model.md), the [equilibrium point](equilibrium-point-of-a-dynamical-system.md) is [asymptotically stable](asymptotic-stability.md) for $0\leq d<d_c$. No nonnegative real [delayed feedback characteristic root](delayed-feedback-characteristic-root.md) can satisfy the equation; the first loss of [asymptotic stability](asymptotic-stability.md) is the indicated pair of imaginary [delayed feedback characteristic roots](delayed-feedback-characteristic-root.md). Differentiating the [characteristic equation of a delay differential equation](characteristic-equation-of-a-delay-differential-equation.md) along a root yields

$$
\frac{d\lambda}{dd}=-\frac{\lambda(\lambda+1)}{1+d(\lambda+1)},\qquad \operatorname{Re}\left(\frac{d\lambda}{dd}\right)_{d=d_c}=\frac{3}{(1+d_c)^2+3d_c^2}>0.
$$

Thus the pair moves into growth as the delay increases through $d_c$. The neutral mode at $d_c$ is a [periodic function](periodic-function.md), but its amplitude depends on history: this linear [mathematical model](mathematical-model.md) does not select an attracting [limit cycle](limit-cycle.md).

The figure plots $x(t)=e^{at}\cos(bt)$ using a [delayed feedback characteristic root](delayed-feedback-characteristic-root.md) $\lambda=a+ib$ and that same formula on the history interval. At $d=0.7$ the displayed mode decays; at $d=1.5$ it grows. These are exact modes up to numerical root accuracy, not step responses with identical histories. Molecular bounds and a changed return law would be needed to interpret what happens after an unstable biological response becomes large.

**Table of contents**

- [Delayed feedback characteristic root](delayed-feedback-characteristic-root.md)

## ↑ Ancestors (5)

1. [Negative feedback](negative-feedback.md)
2. [Signaling feedback](signaling-feedback.md)
3. [Signal transduction](signal-transduction-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Delay differential equation](delay-differential-equation.md)
- [Homeostatic temperature model](homeostatic-temperature-model.md)
- [Negative feedback](negative-feedback.md)
