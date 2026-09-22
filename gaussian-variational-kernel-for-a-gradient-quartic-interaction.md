# Gaussian variational kernel for a gradient quartic interaction

↑ **Parent:** [Gaussian variational approximation](gaussian-variational-approximation.md)

For $H=\int[a\phi^2/2+\kappa|\nabla\phi|^2/2+\gamma(\nabla^2\phi)^2/2+B\phi^2|\nabla\phi|^2]$ and an even positive trial kernel $J(q)$, define $S_0=\sum_q^+1/J(q)$ and $S_2=\sum_q^+q^2/J(q)$ using a [positive-wavevector sum for a real field](positive-wavevector-sum-for-a-real-field.md). [Isserlis theorem](isserlis-s-theorem.md) gives $\langle H_4\rangle_0=4BS_0S_2/V$. The [Feynman-Bogoliubov inequality](gibbs-bogoliubov-feynman-inequality.md) therefore has stationary kernels

$$
J(q)=a+\kappa q^2+\gamma q^4+\frac{4B}{V}(S_2+q^2S_0).
$$

Thus both the mass and gradient coefficient shift. In the [thermodynamic limit](thermodynamic-limit.md), their [self-consistency equations](self-consistency-equation.md) are

$$
\bar a=a+2B\int_{|k|<\Lambda}\frac{k^2}{\bar a+\bar\kappa k^2+\gamma k^4}\frac{d^dk}{(2\pi)^d},
\quad
\bar\kappa=\kappa+2B\int_{|k|<\Lambda}\frac1{\bar a+\bar\kappa k^2+\gamma k^4}\frac{d^dk}{(2\pi)^d}.
$$

A coarse-graining [ultraviolet cutoff](ultraviolet-cutoff.md) $\Lambda$ is necessary for the first integral in three dimensions: its large-$k$ radial integrand tends to a constant. Physical solutions require $J(q)>0$.

## ↑ Ancestors (9)

1. [Gaussian variational approximation](gaussian-variational-approximation.md)
2. [Gaussian field theory](gaussian-field-theory.md)
3. [Landau-Ginzburg theory](landau-ginzburg-theory.md)
4. [Landau theory](landau-theory.md)
5. [Critical phenomenon](critical-phenomenon-split.md)
6. [Statistical physics](statistical-physics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gradient-quartic Brazovskii model](gradient-quartic-brazovskii-model.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-344/1/e/solution.md)
