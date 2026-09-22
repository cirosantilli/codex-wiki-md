# SLE interior-point martingale

↑ **Parent:** [SLE angle process](sle-angle-process.md)

For $\kappa>0$, $\rho>0$, let $J_t=|g_t'(z)|$, $S_t=\sin\theta_t$ and $\Upsilon_t=Y_t/J_t$. Then

$$
M_t=J_t^{(8-\kappa+\rho)\rho/(4\kappa)}\Upsilon_t^{\rho(\rho+8)/(8\kappa)}S_t^{-\rho/\kappa}
$$

is a positive continuous [local martingale](local-martingale.md) before the [Loewner swallowing time](interior-point-swallowing-time-for-a-loewner-chain.md). Indeed the [Itô formula](ito-s-lemma.md) gives $d\log J_t=-2(X_t^2-Y_t^2)|Z_t|^{-4}dt$, $d\log\Upsilon_t=-4Y_t^2|Z_t|^{-4}dt$, and

$$
d\log S_t=\frac{(\kappa/2-4)X_t^2-\kappa Y_t^2/2}{|Z_t|^4}\,dt+\sqrt\kappa\frac{X_t}{|Z_t|^2}\,dB_t.
$$

Combining the exponents cancels the drift of $M_t$, including the quadratic-variation correction, leaving $dM_t/M_t=-\rho X_t/(\sqrt\kappa|Z_t|^2)\,dB_t$.

## ↑ Ancestors (8)

1. [SLE angle process](sle-angle-process.md)
2. [Schramm–Loewner evolution](schramm-loewner-evolution.md)
3. [Stochastic process](stochastic-process-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-203/3/c/solution.md)
- [Space-filling SLE above parameter eight](space-filling-sle-above-parameter-eight.md)
