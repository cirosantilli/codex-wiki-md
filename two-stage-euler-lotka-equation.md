# Two-stage Euler-Lotka equation

↑ **Parent:** [Euler-Lotka equation](euler-lotka-equation.md)

For serial stages with [survival functions](survival-function.md) $S_i(a)=\exp[-\int_0^a\Gamma_i(s)ds]$, set $H_i(r)=\int_0^\infty\Gamma_i(a)S_i(a)e^{-ra}da$. If completion of stage two produces $m$ new stage-one individuals, a common exponential mode requires $mH_1(r)H_2(r)=1$. Indeed its age profiles are $\phi_i(a)=\phi_i(0)e^{-ra}S_i(a)$, while the incoming [fluxes](flux.md) give $\phi_2(0)=H_1\phi_1(0)$ and $\phi_1(0)=mH_2\phi_2(0)$. Cancelling nonzero amplitudes proves the equation. Under ordinary positive residence-time assumptions a positive root exists exactly when $mH_1(0)H_2(0)>1$. The normalized profiles are $e^{-ra}S_i(a)/\int e^{-rs}S_i(s)ds$.

## ↑ Ancestors (6)

1. [Euler-Lotka equation](euler-lotka-equation.md)
2. [Age-structured population model](age-structured-population-model.md)
3. [Mathematical biology](mathematical-biology-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-further-mathematical-biology-course-of-the-university-of-oxford/2023/1/c/solution.md)
