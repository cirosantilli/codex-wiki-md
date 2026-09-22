<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E(\lambda)=\sqrt\pi\lambda e^{\lambda^2}\operatorname{erfc}(\lambda)$. The salt equation in the [saline Stefan problem](../../../../../../saline-stefan-problem.md) gives $C_i-C_0=E(\lambda)C_i$. Since the [complementary error function](../../../../../../complementary-error-function.md) is positive on the real axis and $C_i>0$, the signs of $C_i-C_0$ and $\lambda$ agree. Thus freezing is equivalent to $C_i>C_0$, or $T_i<T_0=-mC_0$. Using the leading thermal balance,

$$
T_i-T_0=\frac{\theta_+-\theta_-}{2}+O(\epsilon),\qquad \boxed{\lambda>0\quad\Longleftrightarrow\quad\theta_->\theta_+}
$$

at leading order away from a vanishing [temperature](../../../../../../temperature.md) difference. In fact the exact onset is also $\theta_-=\theta_+$: at $\lambda=0$ the salt balance forces $C_i=C_0$, and the [Stefan condition](../../../../../../stefan-condition.md) then forces $T_{-\infty}+T_\infty=2T_0$. The solution with $\lambda=0$ has a stationary interface and balancing conductive [heat fluxes](../../../../../../heat-flux-density.md), despite nontrivial diffusion of the initial [temperature](../../../../../../temperature.md) discontinuity. For completeness, the exact freezing criterion follows without relying on that local crossing. By the [salt-rejection function for a saline Stefan front](../../../../../../salt-rejection-function-for-a-saline-stefan-front.md), $T_i(\lambda)$ decreases continuously from $T_0$ to $-\infty$ as positive $\lambda$ increases. If $T_{-\infty}<T_0$, let $\lambda_s$ be where $T_i=T_{-\infty}$. On $[0,\lambda_s]$, the solid-side thermal term decreases, the liquid-side term increases, and the latent-heat term increases: the factors $e^{-\epsilon^2\lambda^2}/\operatorname{erfc}(-\epsilon\lambda)$ and $e^{-\epsilon^2\lambda^2}/\operatorname{erfc}(\epsilon\lambda)$ decrease and increase respectively. These monotonicities follow from the positive integral representation of $e^{v^2}\operatorname{erfc}v$. The thermal residual starts at $(\theta_--\theta_+)/\sqrt\pi$ and is negative at $\lambda_s$, so a positive root exists uniquely precisely when $\theta_->\theta_+$. Beyond $\lambda_s$ both thermal contributions to freezing are negative, so no further root is possible. If $T_{-\infty}\ge T_0$, the same sign argument excludes every positive root.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 332](../../../paper-332-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
