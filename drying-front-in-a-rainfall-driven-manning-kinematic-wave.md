# Drying front in a rainfall-driven Manning kinematic wave

↑ **Parent:** [Kinematic wave](kinematic-wave.md)

Let $H(t)=\int_0^tE(r)\,dr$, increasing until $t^*$ and decreasing afterwards. For dry initial data and zero upstream depth, a [characteristic](characteristic-of-a-field.md) emitted at time $\tau$ has $h=H(t)-H(\tau)$ and position $s=\frac53\int_\tau^t[H(r)-H(\tau)]^{2/3}\,dr$, for as long as its depth stays nonnegative. The height follows by integrating the source along a [characteristic](characteristic-of-a-field.md), and the position follows from the [derivative](derivative.md) of the Manning flux.

When $E<0$ and $H(t)>0$, define the earlier emission time $\tau_d(t)\leq t^*$ by $H(\tau_d)=H(t)$. The front where this water is just exhausted has

$$
s_d(t)=\frac53\int_{\tau_d(t)}^t[H(r)-H(t)]^{2/3}\,dr.
$$

It moves downstream because $s_d'=-(10/9)E(t)\int_{\tau_d}^t[H(r)-H(t)]^{-1/3}\,dr>0$. Behind it depth is zero; ahead, unexhausted [characteristic](characteristic-of-a-field.md) labels determine the wet profile. This construction presumes removal limited by water availability: continuing a negative source unchanged at zero depth would violate nonnegativity. If $H$ reaches zero, the remaining initially generated water has also vanished.

## ↑ Ancestors (10)

1. [Kinematic wave](kinematic-wave.md)
2. [Characteristic speed](characteristic-speed.md)
3. [Flux Jacobian](flux-jacobian.md)
4. [System of conservation laws](system-of-conservation-laws.md)
5. [Transport equation](transport-equation-split.md)
6. [Partial differential equation](partial-differential-equation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford/2008/a/2/v/solution.md)
