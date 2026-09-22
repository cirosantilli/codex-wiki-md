<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For the [driven two-state rotary motor](../../../../driven-two-state-rotary-motor.md), use positive [angular velocity](../../../../angular-velocity.md) $\omega>0$ and extend all angular functions with period $2\pi$. In the first half-turn the source figure has $k_{AB}=k_0$, $k_{BA}=0$, so the stationary equation is $\omega P_A'=-k_0P_A$. In the second half-turn the rates are interchanged, giving $\omega P_A'=k_0(1-P_A)$. Hence

$$
P_A(\theta)=\begin{cases}
\alpha e^{-\beta\theta},&0\le\theta\le\pi,\\
1-Ce^{-\beta(\theta-\pi)},&\pi\le\theta\le2\pi,
\end{cases}\qquad\beta=\frac{k_0}\omega.
$$

[Continuity](../../../../continuous-function.md) at $\pi$ gives $1-C=\alpha e^{-\beta\pi}$, while [periodicity](../../../../periodicity.md) gives $\alpha=1-Ce^{-\beta\pi}$. Solving the two linear conditions gives $C=\alpha$ and

$$
\boxed{\alpha=\frac1{1+e^{-\pi k_0/\omega}},\qquad
\beta=\frac{k_0}{\omega},\qquad
P_A(\theta+\pi)=1-P_A(\theta),\qquad P_B=1-P_A.}
$$

In particular $P_A(0)=P_A(2\pi)=\alpha$ and $P_A(\pi)=1-\alpha$, so the two pieces fill in the apparent endpoint gap in the printed piecewise formula. The [probability](../../../../probability.md) decreases exponentially during the detachment half-cycle and rises exponentially during the attachment half-cycle; $P_B$ is its complement. Both remain between zero and one. They are state [probabilities](../../../../probability.md) _conditional on rotor angle_, not separate angular densities normalized individually to one.

For $\omega\ll k_0$, attachment and detachment almost finish within their allotted half-turns: $P_A$ is nearly zero through most of $0<\theta<\pi$ and nearly one through most of $\pi<\theta<2\pi$, with angular [boundary layers](../../../../boundary-layer.md) of width $\omega/k_0$. For $\omega\gg k_0$, it stays near one half with a small nearly triangular modulation. The upper panels of the original figure in part (b) sketch both limits. At exactly zero speed the advective stationary problem is singular; these statements concern the positive-speed limit.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2018](../../../2018-split.md)
4. [Past exam of the biological physics course of the University of Oxford](../../../split.md)
5. [Biological physics course of the University of Oxford](../../../../biological-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
