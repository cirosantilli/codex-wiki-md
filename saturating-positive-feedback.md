# Saturating positive feedback

↑ **Parent:** [Positive feedback](positive-feedback.md)

[Saturating positive feedback](saturating-positive-feedback.md) limits the reinforcing rate as activity increases. Here is an explicitly synthetic [ordinary differential equation](ordinary-differential-equation.md) for normalized nonnegative input $u$, response $x$, and return strength $\beta$:

$$
\frac{dx}{dt}=f(x;u,\beta)=u+\frac{\beta x^2}{1+x^2}-x,\qquad u\geq0,\quad\beta\geq0.
$$

The return is an increasing, nonproportional function of $x$, while removal is proportional to $x$. Time and activities are [dimensionless variables](dimensionless-variable.md). At $x=0$ the [vector field](vector-field.md) points into the nonnegative domain, and $dx/dt\leq u+\beta-x$ prevents unbounded growth there. This makes the toy useful for asking about a bounded switch; it supplies no molecular mechanism for the chosen rate law.

At an [equilibrium point](equilibrium-point-of-a-dynamical-system.md), $f=0$. For a simple [equilibrium point](equilibrium-point-of-a-dynamical-system.md), the sign of the [derivative](derivative.md)

$$
f_x=\frac{2\beta x}{(1+x^2)^2}-1
$$

determines local [asymptotic stability](asymptotic-stability.md). If $\beta=1$, the maximum reinforcing slope is $3\sqrt3/8<1$, so $f$ decreases strictly: every $u\geq0$ has one [asymptotically stable](asymptotic-stability.md) [equilibrium point](equilibrium-point-of-a-dynamical-system.md) despite [positive feedback](positive-feedback.md).

Three [equilibrium points](equilibrium-point-of-a-dynamical-system.md) become possible only if the reinforcing slope exceeds removal's slope somewhere. Its maximum is $3\sqrt3\beta/8$, at $x=1/\sqrt3$. Consequently this toy requires

$$
\beta>\frac{8}{3\sqrt3}\simeq1.53960
$$

for two distinct folds. This is a necessary threshold for a [bistability](bistability.md) interval in this toy, not a universal biochemical number. At a fold, both $f=0$ and $f_x=0$, giving

$$
(1+x^2)^2=2\beta x,\qquad u=x-\frac{\beta x^2}{1+x^2}.
$$

For $\beta=1.8$, the folds are at $(x,u)\simeq(0.350003,0.153563)$ and $(0.887240,0.094405)$. Between these input values there are two [asymptotically stable](asymptotic-stability.md) [equilibrium points](equilibrium-point-of-a-dynamical-system.md) separated by an unstable one. At $u=0.12$, the three activities are approximately $0.171331$, $0.621230$ and $1.127439$; the low and high ones are stable.

A sufficiently slow increasing sweep follows the low branch to $u_{\mathrm{on}}\simeq0.153563$ and then jumps upward. A decreasing sweep follows the high branch to $u_{\mathrm{off}}\simeq0.094405$ and then jumps downward: [hysteresis](hysteresis.md). These are limiting quasistatic thresholds, with relaxation between input changes and negligible perturbations that could cause earlier switching. Finite sweep rates and fluctuations can alter observed thresholds. A switchlike response with only one stable [equilibrium point](equilibrium-point-of-a-dynamical-system.md) does not have this equilibrium [hysteresis](hysteresis.md) mechanism.

## ↑ Ancestors (5)

1. [Positive feedback](positive-feedback.md)
2. [Signaling feedback](signaling-feedback.md)
3. [Signal transduction](signal-transduction-split.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Saturating positive feedback](saturating-positive-feedback.md)
