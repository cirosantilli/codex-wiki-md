<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the usual [saline Stefan problem](../../../../../saline-stefan-problem.md) approximation: no bulk flow, salt-free [ice](../../../../../ice.md) with negligible salt transport, constant properties, equal phase densities, and the same [thermal conductivity](../../../../../thermal-conductivity.md) $k_T$ and [thermal diffusivity](../../../../../thermal-diffusivity.md) $\kappa$ in both phases. Write $c_p$ for [specific heat capacity](../../../../../specific-heat-capacity.md), $L_f$ for [latent heat](../../../../../latent-heat.md) per unit mass, and $k_T=\rho c_p\kappa$. These thermal symmetries are needed for the arithmetic-mean interface [temperature](../../../../../temperature.md) requested in the paper; unequal phase conductivities would give a weighted balance instead.

Set $\eta=x/(2\sqrt{\kappa t})$, $\xi=x/(2\sqrt{Dt})$, $\epsilon=\sqrt{D/\kappa}$ and $a(t)=2\lambda\sqrt{Dt}$. The [heat equation](../../../../../heat-equation.md) and salt [diffusion equation](../../../../../diffusion-equation-split.md) reduce to $f''+2sf'=0$. Their [similarity solutions](../../../../../similarity-solution.md), in terms of the [complementary error function](../../../../../complementary-error-function.md), are

$$
\begin{aligned}
T_s(x,t)&=T_{-\infty}+(T_i-T_{-\infty})\frac{\operatorname{erfc}(-\eta)}{\operatorname{erfc}(-\epsilon\lambda)},&&x<a(t),\\
T_l(x,t)&=T_\infty+(T_i-T_\infty)\frac{\operatorname{erfc}(\eta)}{\operatorname{erfc}(\epsilon\lambda)},&&x>a(t),\\
C(x,t)&=C_0+(C_i-C_0)\frac{\operatorname{erfc}(\xi)}{\operatorname{erfc}(\lambda)},&&x>a(t).
\end{aligned}
$$

These have the required interface values and far-field limits. At each fixed $x\ne0$ they recover the initial data as $t\downarrow0$. The [liquidus](../../../../../liquidus.md) condition is $T_i=-mC_i$.

[Salt rejection](../../../../../salt-rejection.md) and the [Stefan condition](../../../../../stefan-condition.md) give, with [gradients](../../../../../gradient.md) evaluated on the appropriate sides of the interface,

$$
-D C_x(a^+,t)=\dot a\,C_i,\qquad \rho L_f\dot a=k_T[T_{s,x}(a^-,t)-T_{l,x}(a^+,t)].
$$

For example, [salt rejection](../../../../../salt-rejection.md) is obtained by differentiating the total salt on a moving liquid interval: the moving lower endpoint removes $\dot a C_i$, which must be supplied by diffusive transport away from the salt-free solid. Substitution, including the [salt-rejection function for a saline Stefan front](../../../../../salt-rejection-function-for-a-saline-stefan-front.md), gives the complete algebraic system for the [diffusion-controlled iceberg growth and ablation](../../../../../diffusion-controlled-iceberg-growth-and-ablation.md):

$$
\boxed{\begin{aligned}
C_i\left[1-\sqrt\pi\lambda e^{\lambda^2}\operatorname{erfc}(\lambda)\right]&=C_0,\\
T_i&=-mC_i,\\
\frac{L_f}{c_p}\epsilon\lambda&=\frac{e^{-\epsilon^2\lambda^2}}{\sqrt\pi}\left[\frac{T_i-T_{-\infty}}{\operatorname{erfc}(-\epsilon\lambda)}-\frac{T_\infty-T_i}{\operatorname{erfc}(\epsilon\lambda)}\right].
\end{aligned}}
$$

The sign of $\lambda$ distinguishes freezing from melting; neither sign should be excluded in the general [similarity solution](../../../../../similarity-solution.md).

For $\lambda=O(1)$, $\epsilon\ll1$, and fixed $L_f/c_p$ and far-field [temperatures](../../../../../temperature.md), the thermal equation has leading right-hand side $(2T_i-T_{-\infty}-T_\infty)/\sqrt\pi$, while its left-hand side is $O(\epsilon)$. Hence

$$
\boxed{T_i=\frac{T_\infty+T_{-\infty}}2+O(\epsilon).}
$$

This is a leading-order balance, not an exact cancellation of [latent heat](../../../../../latent-heat.md). The resulting $C_i=-T_i/m$ and the first algebraic equation determine the leading $\lambda$. A physical finite-$\lambda$ branch requires $C_i>0$; if the mean [temperature](../../../../../temperature.md) is positive, this salt-diffusion scaling cannot describe the leading solution. Likewise, a [latent-to-sensible heat ratio](../../../../../latent-to-sensible-heat-ratio.md) diverging as $1/\epsilon$ changes the leading thermal balance.

Define $\theta_-=-mC_0-T_{-\infty}$ and $\theta_+=T_\infty+mC_0$. Put $T_0=-mC_0$ and $\Delta\theta=\theta_--\theta_+$. Then $T_i=T_0-\Delta\theta/2+O(\epsilon)$, which will determine the freezing and [constitutional supercooling](../../../../../constitutional-supercooling.md) conditions below.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 332](../../paper-332-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
